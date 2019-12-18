[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [ParamorphismConfig](./index.md)

# ParamorphismConfig

`interface ParamorphismConfig`

Contains global configuration values to define the behaviour of the program as a whole.

### Properties

| Name | Summary |
|---|---|
| [branding](branding.md) | Defines whether to declare an `Obfuscated-By` entry in the resulting JAR's manifest.`open val branding: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [customTransformers](custom-transformers.md) | Custom transformers. Only available for custom configurations.`open val customTransformers: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`CustomTransformer`](../../site.hackery.paramorphism.api.custom/-custom-transformer/index.md)`>` |
| [deeplyNestedClassInjection](deeply-nested-class-injection.md) | `open val deeplyNestedClassInjection: `[`DeeplyNestedClassInjectionStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.corruption/-deeply-nested-class-injection-strategy-config/index.md) |
| [forceNoVerify](force-no-verify.md) | `open val forceNoVerify: `[`ForceNoVerifyStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.corruption/-force-no-verify-strategy-config/index.md) |
| [input](input.md) | The input JAR file to act upon.`open val input: `[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html) |
| [jumpReplacement](jump-replacement.md) | `open val jumpReplacement: `[`JumpReplacementStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.flow/-jump-replacement-strategy-config/index.md) |
| [kotlinDelegatedPropertiesConcealing](kotlin-delegated-properties-concealing.md) | `open val kotlinDelegatedPropertiesConcealing: `[`KotlinDelegatedPropertiesConcealingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-delegated-properties-concealing-strategy-config.md) |
| [kotlinIntrinsicsConcealing](kotlin-intrinsics-concealing.md) | `open val kotlinIntrinsicsConcealing: `[`KotlinIntrinsicsConcealingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-intrinsics-concealing-strategy-config.md) |
| [kotlinMetadataStripping](kotlin-metadata-stripping.md) | `open val kotlinMetadataStripping: `[`KotlinMetadataStrippingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-metadata-stripping-strategy-config.md) |
| [libraries](libraries.md) | An array of JAR files defining the searched class path of the obfuscator.`open val libraries: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html)`>` |
| [lineNumberStripping](line-number-stripping.md) | `open val lineNumberStripping: `[`LineNumberStrippingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-line-number-stripping-strategy-config.md) |
| [localVariableStripping](local-variable-stripping.md) | `open val localVariableStripping: `[`LocalVariableStrippingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-local-variable-stripping-strategy-config.md) |
| [mask](mask.md) | Defines which elements any obfuscation strategy is allowed to visit.`open val mask: `[`ElementMask`](../-element-mask/index.md) |
| [methodIndirection](method-indirection.md) | `open val methodIndirection: `[`MethodIndirectionStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.concealment/-method-indirection-strategy-config.md) |
| [nullByteNaming](null-byte-naming.md) | `open val nullByteNaming: `[`NullByteNamingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.corruption/-null-byte-naming-strategy-config/index.md) |
| [output](output.md) | The output location to emit the resulting obfuscated JAR file.`open val output: `[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html) |
| [packer](packer.md) | `open val packer: `[`PackingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.packing/-packing-strategy-config/index.md) |
| [remapper](remapper.md) | `open val remapper: `[`RemappingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.remapper/-remapping-strategy-config/index.md) |
| [shadedLibraries](shaded-libraries.md) | Defines which elements in the class file should be treated as 'shaded libraries', which are untouched by any obfuscation strategy.`open val shadedLibraries: `[`ElementMask`](../-element-mask/index.md)`?` |
| [sourceFileStripping](source-file-stripping.md) | `open val sourceFileStripping: `[`SourceFileStrippingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-source-file-stripping-strategy-config/index.md) |
| [spigotRemapPluginYML](spigot-remap-plugin-y-m-l.md) | `open val spigotRemapPluginYML: `[`SpigotRemapPluginYMLStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.scenarios.spigot/-spigot-remap-plugin-y-m-l-strategy-config.md) |
| [stringConcealing](string-concealing.md) | `open val stringConcealing: `[`StringConcealingStrategyConfig`](../../site.hackery.paramorphism.api.config.strategies.concealment/-string-concealing-strategy-config.md) |
| [useJavaRuntime](use-java-runtime.md) | Defines whether to implicitly include the runtime classes of the currently-running Java instance in the searched class path of the obfuscator.`open val useJavaRuntime: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [workingDirectory](working-directory.md) | The working directory of this configuration. Usually the parent directory of the configuration file.`abstract val workingDirectory: `[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html) |

### Companion Object Functions

| Name | Summary |
|---|---|
| [of](of.md) | Utility function.`fun of(config: `[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html)`): `[`ParamorphismConfig`](./index.md) |
