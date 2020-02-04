---
title: Strategies
order: 3
---

**Note:** Strategy configuration heavily mimics the [public API](https://github.com/SerenityEnterprises/paramorphism-site-content/blob/master/dokka/paramorphism/site.hackery.paramorphism.api.config/-paramorphism-config/index.md) for the obfuscator.

All strategies have the same built-in configuration variables.

- `enabled` - Whether to use this strategy in obfuscation
- `mask` - The set of elements uppon which to operate
- `override_global_mask` - Whether the strategy's local mask overrides the configuration's global mask.

The default value of `enabled` varies between each strategy, but most non-dangerous strategies will be enabled by default.

`override_global_mask` will always default to false, where `mask` is the empty mask (allowing all elements). This means that by default an obfuscation strategy will apply to the global mask.

<!-- TODO: override_global_mask example -->

```yml
{strategy name}:
  enabled: true
  mask:
    include:
      - com/example/
    exclude:
      - com/example/myproject/api/
```

## Remapper

The remapping strategy alters the names of elements in a JAR file. This includes package and class names, field names, and method names.

In the `remapper` configuration block, there are some strategy-specific values:

Their defaults are depicted below:

```yml
remapper:
  exclude_enums: true
  flat: false
  prefix: null

  name_generation:
    shuffle: false
    dictionaries:
      packages: ALPHABET
      classes: ALPHABET
      methods: ALPHABET
      fields: ALPHABET

  manifest_entries:
    - "Main-Class"
    - "Agent-Class"
    - "Premain-Class"
```

### Pitfalls

The remapper **needs** to have every class in the class hierarchy graph known to the obfuscator. This is because when remapping a member element of a class (a field or a method), it needs to do two things.

Given two classes, `LibraryClass` and `MyClass`, where `LibraryClass` is contained in an external library:

```java
class LibraryClass {
  boolean a;

  void doSomething() {
    System.out.println("Hello!");
  }
}
```

```java
class MyClass extends LibraryClass {
  boolean myBoolean;

  void myMethod() {
    doSomething();
  }

  @Override // @Override does not exist in bytecode, only source code. Also, it's optional in source code.
  void doSomething() {
    System.out.println("Something else!");
  }
}
```

If we remapped `MyClass` naïvely, without knowledge of the parent class (as it is contained in a library), we produce the following class:

```java
class A extends LibraryClass {
  boolean a;

  void a() {
    b();
  }

  void b() {
    System.out.println("Something else!");
  }
}
```

Here, we have encountered two issues:

1. `MyClass`'s boolean `myBoolean` now overlaps with `LibraryClass`'s boolean `a`.
2. `MyClass`'s override of `doSomething` is no longer held. If `doSomething` were abstract, we would encounter a runtime exception, but here, it changes the semantics of the program if `LibraryClass l = new MyClass(); l.doSomething()` is called.
