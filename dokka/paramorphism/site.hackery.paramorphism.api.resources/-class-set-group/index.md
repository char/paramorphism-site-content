[paramorphism](../../index.md) / [site.hackery.paramorphism.api.resources](../index.md) / [ClassSetGroup](./index.md)

# ClassSetGroup

`class ClassSetGroup`

A collected group of ClassSets, using a linear search for lookup.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | A collected group of ClassSets, using a linear search for lookup.`ClassSetGroup(classSets: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`ClassSet`](../-class-set/index.md)`>)` |

### Properties

| Name | Summary |
|---|---|
| [classSets](class-sets.md) | `val classSets: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`ClassSet`](../-class-set/index.md)`>` |

### Functions

| Name | Summary |
|---|---|
| [all](all.md) | All classes from every class set.`fun all(): `[`Sequence`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.sequences/-sequence/index.html)`<`[`ClassInfo`](../-class-info/index.md)`>` |
| [exists](exists.md) | Determine whether the class exists in the class sets`fun exists(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [lookup](lookup.md) | Look up a class by its name.`fun lookup(name: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`ClassInfo`](../-class-info/index.md)`?` |
