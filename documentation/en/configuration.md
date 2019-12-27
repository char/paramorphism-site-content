---
title: Configuration
order: 2
---

## Input & Output

`input` defines the path where the target artifact can be found, while `output` declares where the obfuscated output will be emitted.

These paths are either relative to the location of the configuration file or absolute, except in the case of an absolute base path (e.g. `/` on most operating systems, or a drive letter root like `C:/` on Windows).

**Example:**

```yml
input: path/to/application.jar
output: obfuscated-application.jar
```

## Libraries

`libraries` is a simple list of JAR files (or directories of JAR files). To use `libraries`, simply list the JAR files and/or directories that you wish to include. Just like `input` and `output`, these paths are relative to the location of the configuration file.

**Note**: In order for the remapper to function correctly, all libraries upon which the application depends need to be declared in the configuration file.
This is because in order to correctly map overridden methods in classes, the obfuscator must process the classes' inheritance hierarchy to ensure that members that override third-party superclasses are not remapped. (Otherwise, this would lead to `AbstractMethodError`s when running the code.)

By default, `libraries` implicitly includes the Java runtime classes of the JRE used to execute Paramorphism. In the unlikely event you want to override this behaviour, you can set the `use_java_runtime` entry to `false`.

## Element Masks

An element mask defines which elements are to be included and excluded in an obfuscation pass.

The global mask is defined by the `mask` entry in the configuration file, and controls which classes **any** obfuscation strategy can touch.

```yml
input: myproject-1.0.0.jar

mask: # Define the global mask for the obfuscator
  include:                             # We want to limit the scope of obfuscations to only:
    - com/example/myproject/           # - our own project,
    - org/business/proprietarylibrary/ # - and another vendor's library that has been contracted to us.
  exclude:                             # And out of these, we don't want to include:
    - com/example/myproject/api/       # - our public-facing API.

    # Since we're serializing via this class (e.g. via Gson), we don't want to have its field names obfuscated, so we also put it in exclude:
    - com/example/myproject/config/ConfigurationJSONBean
```

There are also other element masks that can be specified in the configuration file:

- `shaded_libraries` controls which classes inside the JAR should be treated like entries in the `libraries` list - **Note:** Correctly defining the shaded libraries can lead to notable improvements to obfuscation speed.
- All obfuscation strategies have a strategy-specific `mask` entry, which can optionally override the global mask.

### Matching Rules

In an element mask, `include` and `exclude` and lists of *matching rules*.

- **Package:** If a rule ends with `/`, it will match anything starting with the rule. For instance, the rule `path/rule/` matches `path/rule/One`, `path/rule/Two`, but not `other/path/MyClass`
- **Wildcard:** If a rule ends with `*`, it will match anything starting with the rule (except the asterisk). For instance, the rule `wildcard/rule*` matches `wildcard/rule/one`, `wildcard/ruletwothreefour/five`, but not `wildcard/notrule/anythingelse`
- **Literal:** Otherwise, a rule will only match anything identical to itself.

## Miscellaneous

There are a few individual configuration flags that don't fit into any general category:

- `branding` is a boolean, defaults to `true`, and specifies whether to include 'Paramorphism' identifiers inside the output JAR.
- `disable_progress_bars` is a boolean, defaults to `false`, and specifies whether to show real-time progress in the obfuscator. Real-time progress is known to cause performance issues on some Windows builds. (?)
