[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [ElementMask](./index.md)

# ElementMask

`interface ElementMask`

Determines which elements to let through based on its 'include' and 'exclude' values.

When [include](include.md) is empty, all values are let through **except** values which match [exclude](exclude.md).
Otherwise, values are only let through when they match any rule in [include](include.md) and do not match any rule in [exclude](exclude.md).

Given a rule `rule` and a string to match `element`, the following logic applies:

* If the `rule` ends in a forward-slash (`/`), it matches when `element` starts with `rule`. (Package-match)
* If the `rule` ends in an asterisk (`*`), it matches when `element` starts with `rule` minus the asterisk. (Wildcard-match)
* Otherwise, the rule matches when it is the same as `element`.

### Properties

| Name | Summary |
|---|---|
| [exclude](exclude.md) | Defines the exclude set for this element mask.`open val exclude: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |
| [include](include.md) | Defines the include set for this element mask.`open val include: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |

### Inheritors

| Name | Summary |
|---|---|
| [EmptyElementMask](../../site.hackery.paramorphism.api.config.util/-empty-element-mask/index.md) | An empty [ElementMask](./index.md). Filters no values.`class EmptyElementMask : `[`ElementMask`](./index.md) |
