[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [StrategyConfiguration](./index.md)

# StrategyConfiguration

`interface StrategyConfiguration`

Contains base values needed for all obfuscation strategies.

### Properties

| Name | Summary |
|---|---|
| [enabled](enabled.md) | Defines whether this strategy should be used.`open val enabled: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)`?` |
| [irregularities](irregularities.md) | Used internally to determine special treatment of strategies. Do not override for configuration implementations.`open val irregularities: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`StrategyIrregularity`](../-strategy-irregularity.md)`>` |
| [mask](mask.md) | Defines which elements this specific strategy can act upon. Elements usually must be in **both** the global and strategy-local masks to be transformed.`open val mask: `[`ElementMask`](../-element-mask/index.md) |
| [overrideGlobalMask](override-global-mask.md) | Defines whether the [strategy-local mask](mask.md) should override the [global mask](../-paramorphism-config/mask.md).`open val overrideGlobalMask: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [DeeplyNestedClassInjectionStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.corruption/-deeply-nested-class-injection-strategy-config/index.md) | Contains settings for the "Deeply Nested Class Injection" strategy. Disabled by default.`interface DeeplyNestedClassInjectionStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [ForceNoVerifyStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.corruption/-force-no-verify-strategy-config/index.md) | Contains settings for the "Force No Verify" strategy. Enabled by default when 'Main-Class' is detected in the manifest.`interface ForceNoVerifyStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [JumpReplacementStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.flow/-jump-replacement-strategy-config/index.md) | Contains settings for the "Jump Replacement" strategy. Disabled by default.`interface JumpReplacementStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [KotlinDelegatedPropertiesConcealingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-delegated-properties-concealing-strategy-config.md) | Contains settings for the "Kotlin Delegated Properties Concealing" strategy.`interface KotlinDelegatedPropertiesConcealingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [KotlinIntrinsicsConcealingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-intrinsics-concealing-strategy-config.md) | Contains settings for the "Kotlin Intrinsics Concealing" obfuscation strategy.`interface KotlinIntrinsicsConcealingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [KotlinMetadataStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-metadata-stripping-strategy-config.md) | Contains settings for the "Kotlin Metadata Stripping" obfuscation strategy.`interface KotlinMetadataStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [LineNumberStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-line-number-stripping-strategy-config.md) | Contains settings for the "Line Number Stripping" obfuscation strategy.`interface LineNumberStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [LocalVariableStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-local-variable-stripping-strategy-config.md) | Contains settings for the "Local Variable Stripping" strategy.`interface LocalVariableStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [MethodIndirectionStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.concealment/-method-indirection-strategy-config.md) | Contains settings for the "Method Indirection" obfuscation strategy. "Method Indirection" uses concealing instructions to hide the original receiver of a method call.`interface MethodIndirectionStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [NullByteNamingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.corruption/-null-byte-naming-strategy-config/index.md) | Contains settings for the "Null Byte Naming" obfuscation strategy.`interface NullByteNamingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [PackingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.packing/-packing-strategy-config/index.md) | Contains settings for the "Packer" strategy. The packer hides all classes inside a binary blob, and decodes and loads the classes at runtime.`interface PackingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [RemappingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.remapper/-remapping-strategy-config/index.md) | Contains settings for the "Remapper" obfuscation strategy.`interface RemappingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [SourceFileStrippingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-source-file-stripping-strategy-config/index.md) | Contains settings for the "Source File Stripping" obfuscation strategy.`interface SourceFileStrippingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [SpigotRemapPluginYMLStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.scenarios.spigot/-spigot-remap-plugin-y-m-l-strategy-config.md) | Contains settings for the "Spigot Remap 'plugin.yml'" strategy.`interface SpigotRemapPluginYMLStrategyConfig : `[`StrategyConfiguration`](./index.md) |
| [StringConcealingStrategyConfig](../../site.hackery.paramorphism.api.config.strategies.concealment/-string-concealing-strategy-config.md) | Contains settings for the "string concealing" obfuscation strategy. "String Concealing" uses accessor methods to hide the original string constants of a class`interface StringConcealingStrategyConfig : `[`StrategyConfiguration`](./index.md) |
