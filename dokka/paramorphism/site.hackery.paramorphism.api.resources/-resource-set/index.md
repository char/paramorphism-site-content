[paramorphism](../../index.md) / [site.hackery.paramorphism.api.resources](../index.md) / [ResourceSet](./index.md)

# ResourceSet

`interface ResourceSet : `[`Closeable`](https://docs.oracle.com/javase/6/docs/api/java/io/Closeable.html)

A set of [resources](../-resource/index.md), e.g. from the contents of a JAR file.

### Functions

| Name | Summary |
|---|---|
| [all](all.md) | `abstract fun all(): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`Pair`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-pair/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`Resource`](../-resource/index.md)`>>` |
| [contains](contains.md) | `abstract fun contains(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [get](get.md) | `abstract fun get(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Resource`](../-resource/index.md)`?` |
| [names](names.md) | `abstract fun names(): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |
| [put](put.md) | `abstract fun put(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, data: `[`Resource`](../-resource/index.md)`?): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
