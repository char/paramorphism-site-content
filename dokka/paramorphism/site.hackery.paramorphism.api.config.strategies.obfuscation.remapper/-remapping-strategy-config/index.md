[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.strategies.obfuscation.remapper](../index.md) / [RemappingStrategyConfig](./index.md)

# RemappingStrategyConfig

`interface RemappingStrategyConfig : `[`StrategyConfiguration`](../../site.hackery.paramorphism.api.config/-strategy-configuration/index.md)

Contains settings for the "Remapper" obfuscation strategy.

### Properties

| Name | Summary |
|---|---|
| [excludeEnums](exclude-enums.md) | Defines whether to remap enum class' simple names. Fixes a crash when using Google's Gson serialization library.`open val excludeEnums: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [flat](flat.md) | Determines whether to place all remapped classes into the default package.`open val flat: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [manifestEntries](manifest-entries.md) | Defines which values to remap in the JAR's manifest file.`open val manifestEntries: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`>` |
| [nameGeneration](name-generation.md) | `open val nameGeneration: `[`NameGenerationConfig`](../../site.hackery.paramorphism.api.config.naming/-name-generation-config/index.md) |
| [prefix](prefix.md) | A global prefix to apply to all class names. Packages are delimited by slashes. Useful when using [flat](flat.md) mapping.`open val prefix: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?` |
