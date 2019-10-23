[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.strategies.obfuscation](../index.md) / [SourceFileStrippingStrategyConfig](./index.md)

# SourceFileStrippingStrategyConfig

`interface SourceFileStrippingStrategyConfig : `[`StrategyConfiguration`](../../site.hackery.paramorphism.api.config/-strategy-configuration/index.md)

Contains settings for the "Source File Stripping" obfuscation strategy.

### Functions

| Name | Summary |
|---|---|
| [sourceFile](source-file.md) | Maps a class' *internal name* to a value of the SourceFile attribute. Returning `null` wipes the SourceFile attribute.`open fun sourceFile(internalName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?` |
