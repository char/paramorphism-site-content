[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [StrategyConfiguration](./index.md)

# StrategyConfiguration

`interface StrategyConfiguration`

Contains base values needed for all obfuscation strategies.

### Properties

| Name | Summary |
|---|---|
| [enabled](enabled.md) | Defines whether this strategy should be used.`open val enabled: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [mask](mask.md) | Defines which elements this specific strategy can act upon. Elements usually must be in **both** the global and strategy-local masks to be transformed.`open val mask: `[`ElementMask`](../-element-mask/index.md) |
| [overrideGlobalMask](override-global-mask.md) | Defines whether the [strategy-local mask](mask.md) should override the [global mask](../-paramorphism-config/mask.md).`open val overrideGlobalMask: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [ClassZipEntryManglingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.corruption/-class-zip-entry-mangling-strategy-config.md) | Contains settings for the "Class Zip Entry Mangling" obfuscation strategy.`interface ClassZipEntryManglingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [KotlinIntrinsicsConcealingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation/-kotlin-intrinsics-concealing-strategy-config.md) | Contains settings for the "Kotlin Intrinsics Concealing" obfuscation strategy.`interface KotlinIntrinsicsConcealingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [KotlinMetadataStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation/-kotlin-metadata-stripping-strategy-config.md) | Contains settings for the "Kotlin Metadata Stripping" obfuscation strategy.`interface KotlinMetadataStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [LineNumberStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation/-line-number-stripping-strategy-config.md) | Contains settings for the "Line Number Stripping" obfuscation strategy.`interface LineNumberStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [NullByteNamingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.corruption/-null-byte-naming-strategy-config.md) | Contains settings for the "Null Byte Naming" obfuscation strategy.`interface NullByteNamingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [RemappingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation/-remapping-strategy-config/index.md) | Contains settings for the "Remapper" obfuscation strategy.`interface RemappingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [SourceFileStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation/-source-file-stripping-strategy-config/index.md) | Contains settings for the "Source File Stripping" obfuscation strategy.`interface SourceFileStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
