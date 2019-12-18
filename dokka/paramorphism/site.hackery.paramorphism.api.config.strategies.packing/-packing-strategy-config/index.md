[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.strategies.packing](../index.md) / [PackingStrategyConfig](./index.md)

# PackingStrategyConfig

`interface PackingStrategyConfig : `[`StrategyConfiguration`](../../site.hackery.paramorphism.api.config/-strategy-configuration/index.md)

Contains settings for the "Packer" strategy.
The packer hides all classes inside a binary blob, and decodes and loads the classes at runtime.

### Properties

| Name | Summary |
|---|---|
| [irregularities](irregularities.md) | Used internally to determine special treatment of strategies. Do not override for configuration implementations.`open val irregularities: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`StrategyIrregularity`](../../site.hackery.paramorphism.api.config/-strategy-irregularity.md)`>` |
| [packedExtension](packed-extension.md) | A suffix to apply to the names of all packed resources`open val packedExtension: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
| [packedPrefix](packed-prefix.md) | A prefix to apply to the names of all packed resources`open val packedPrefix: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html) |
