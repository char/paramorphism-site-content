[paramorphism](../../index.md) / [site.hackery.paramorphism.api.custom](../index.md) / [CustomTransformer](./index.md)

# CustomTransformer

`interface CustomTransformer`

A custom transformer. Applied through [ParamorphismConfig](../../site.hackery.paramorphism.api.config/-paramorphism-config/index.md).

### Functions

| Name | Summary |
|---|---|
| [initialize](initialize.md) | `abstract fun initialize(classes: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`ClassInfo`](../../site.hackery.paramorphism.api.resources/-class-info/index.md)`>): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [injectClasses](inject-classes.md) | `open fun injectClasses(): `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`ClassInfo`](../../site.hackery.paramorphism.api.resources/-class-info/index.md)`>?` |
| [visitClass](visit-class.md) | `abstract fun visitClass(info: `[`ClassInfo`](../../site.hackery.paramorphism.api.resources/-class-info/index.md)`): `[`ClassInfo`](../../site.hackery.paramorphism.api.resources/-class-info/index.md) |
