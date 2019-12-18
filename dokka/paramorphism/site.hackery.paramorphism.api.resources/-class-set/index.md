[paramorphism](../../index.md) / [site.hackery.paramorphism.api.resources](../index.md) / [ClassSet](./index.md)

# ClassSet

`interface ClassSet : `[`Closeable`](https://docs.oracle.com/javase/6/docs/api/java/io/Closeable.html)

A set of [ClassInfo](../-class-info/index.md) objects identified by name.

### Functions

| Name | Summary |
|---|---|
| [all](all.md) | `abstract fun all(): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`ClassInfo`](../-class-info/index.md)`>` |
| [contains](contains.md) | `abstract fun contains(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [get](get.md) | `abstract fun get(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`ClassInfo`](../-class-info/index.md)`?` |
| [names](names.md) | `abstract fun names(): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |
| [put](put.md) | `abstract fun put(info: `[`ClassInfo`](../-class-info/index.md)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
