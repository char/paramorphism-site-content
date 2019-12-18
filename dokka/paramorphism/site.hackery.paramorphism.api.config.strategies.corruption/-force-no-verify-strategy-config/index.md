[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.strategies.corruption](../index.md) / [ForceNoVerifyStrategyConfig](./index.md)

# ForceNoVerifyStrategyConfig

`interface ForceNoVerifyStrategyConfig : `[`StrategyConfiguration`](../../site.hackery.paramorphism.api.config/-strategy-configuration/index.md)

Contains settings for the "Force No Verify" strategy.
Enabled by default when 'Main-Class' is detected in the manifest.

### Properties

| Name | Summary |
|---|---|
| [irregularities](irregularities.md) | Used internally to determine special treatment of strategies. Do not override for configuration implementations.`open val irregularities: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`StrategyIrregularity`](../../site.hackery.paramorphism.api.config/-strategy-irregularity.md)`>` |
