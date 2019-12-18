

Paramorphism is a JVM bytecode obfuscator for Java SE 8 and above.

### All Types

| Name | Summary |
|---|---|
|

##### [site.hackery.paramorphism.api.resources.BufferResource](../site.hackery.paramorphism.api.resources/-buffer-resource/index.md)

A BufferResource is a [Resource](../site.hackery.paramorphism.api.resources/-resource/index.md) that contains a byte array


|

##### [site.hackery.paramorphism.api.resources.ClassInfo](../site.hackery.paramorphism.api.resources/-class-info/index.md)

Information about a class contained in a [ClassSet](../site.hackery.paramorphism.api.resources/-class-set/index.md).


|

##### [site.hackery.paramorphism.api.resources.ClassSet](../site.hackery.paramorphism.api.resources/-class-set/index.md)

A set of [ClassInfo](../site.hackery.paramorphism.api.resources/-class-info/index.md) objects identified by name.


|

##### [site.hackery.paramorphism.api.resources.ClassSetGroup](../site.hackery.paramorphism.api.resources/-class-set-group/index.md)

A collected group of ClassSets, using a linear search for lookup.


|

##### [site.hackery.paramorphism.api.config.ConfigurationException](../site.hackery.paramorphism.api.config/-configuration-exception/index.md)

Thrown when there is an issue parsing a configuration.


|

##### [site.hackery.paramorphism.api.custom.CustomTransformer](../site.hackery.paramorphism.api.custom/-custom-transformer/index.md)

A custom transformer. Applied through [ParamorphismConfig](../site.hackery.paramorphism.api.config/-paramorphism-config/index.md).


|

##### [site.hackery.paramorphism.api.config.strategies.corruption.DeeplyNestedClassInjectionStrategyConfig](../site.hackery.paramorphism.api.config.strategies.corruption/-deeply-nested-class-injection-strategy-config/index.md)

Contains settings for the "Deeply Nested Class Injection" strategy.
Disabled by default.


|

##### [site.hackery.paramorphism.api.naming.Dictionaries](../site.hackery.paramorphism.api.naming/-dictionaries/index.md)

The built-in dictionaries to the obfuscator.


|

##### [site.hackery.paramorphism.api.config.ElementMask](../site.hackery.paramorphism.api.config/-element-mask/index.md)

Determines which elements to let through based on its 'include' and 'exclude' values.


|

##### [site.hackery.paramorphism.api.resources.EmptyClassNode](../site.hackery.paramorphism.api.resources/-empty-class-node.md)

An empty ClassNode — Used for deleting classes from a [ClassSet](../site.hackery.paramorphism.api.resources/-class-set/index.md).


|

##### [site.hackery.paramorphism.api.config.util.EmptyElementMask](../site.hackery.paramorphism.api.config.util/-empty-element-mask/index.md)

An empty [ElementMask](../site.hackery.paramorphism.api.config/-element-mask/index.md). Filters no values.


|

##### [site.hackery.paramorphism.api.config.strategies.corruption.ForceNoVerifyStrategyConfig](../site.hackery.paramorphism.api.config.strategies.corruption/-force-no-verify-strategy-config/index.md)

Contains settings for the "Force No Verify" strategy.
Enabled by default when 'Main-Class' is detected in the manifest.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.flow.JumpReplacementStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.flow/-jump-replacement-strategy-config/index.md)

Contains settings for the "Jump Replacement" strategy.
Disabled by default.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin.KotlinDelegatedPropertiesConcealingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-delegated-properties-concealing-strategy-config.md)

Contains settings for the "Kotlin Delegated Properties Concealing" strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin.KotlinIntrinsicsConcealingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-intrinsics-concealing-strategy-config.md)

Contains settings for the "Kotlin Intrinsics Concealing" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin.KotlinMetadataStrippingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.kotlin/-kotlin-metadata-stripping-strategy-config.md)

Contains settings for the "Kotlin Metadata Stripping" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.stripping.LineNumberStrippingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-line-number-stripping-strategy-config.md)

Contains settings for the "Line Number Stripping" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.stripping.LocalVariableStrippingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-local-variable-stripping-strategy-config.md)

Contains settings for the "Local Variable Stripping" strategy.


|

##### [site.hackery.paramorphism.api.resources.ManifestResource](../site.hackery.paramorphism.api.resources/-manifest-resource/index.md)

A ManifestResource is a [Resource](../site.hackery.paramorphism.api.resources/-resource/index.md) that represents a JAR file's META-INF/MANIFEST.MF file


|

##### [site.hackery.paramorphism.api.naming.MappingDictionary](../site.hackery.paramorphism.api.naming/-mapping-dictionary/index.md)

A 'Mapping Dictionary' data class.


|

##### [site.hackery.paramorphism.api.config.strategies.concealment.MethodIndirectionStrategyConfig](../site.hackery.paramorphism.api.config.strategies.concealment/-method-indirection-strategy-config.md)

Contains settings for the "Method Indirection" obfuscation strategy.
"Method Indirection" uses concealing instructions to hide the original receiver of a method call.


|

##### [site.hackery.paramorphism.api.config.naming.NameGenerationConfig](../site.hackery.paramorphism.api.config.naming/-name-generation-config/index.md)

Contains preferences about configuration of the name generation.


|

##### [site.hackery.paramorphism.api.config.naming.NameGenerationDictionaries](../site.hackery.paramorphism.api.config.naming/-name-generation-dictionaries/index.md)

Contains dictionaries to use on different elements


|

##### [site.hackery.paramorphism.api.config.strategies.corruption.NullByteNamingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.corruption/-null-byte-naming-strategy-config/index.md)

Contains settings for the "Null Byte Naming" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.packing.PackingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.packing/-packing-strategy-config/index.md)

Contains settings for the "Packer" strategy.
The packer hides all classes inside a binary blob, and decodes and loads the classes at runtime.


|

##### [site.hackery.paramorphism.api.config.ParamorphismConfig](../site.hackery.paramorphism.api.config/-paramorphism-config/index.md)

Contains global configuration values to define the behaviour of the program as a whole.


|

##### [site.hackery.paramorphism.api.ParamorphismRelease](../site.hackery.paramorphism.api/-paramorphism-release/index.md)

Contains constant information about the current Paramorphism release.
Can potentially be queried by plugins to determine whether the current version is supported.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.remapper.RemappingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.remapper/-remapping-strategy-config/index.md)

Contains settings for the "Remapper" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.resources.Resource](../site.hackery.paramorphism.api.resources/-resource/index.md)

A [Resource](../site.hackery.paramorphism.api.resources/-resource/index.md) is used to represent data inside a JAR file.


|

##### [site.hackery.paramorphism.api.resources.ResourceSet](../site.hackery.paramorphism.api.resources/-resource-set/index.md)

A set of [resources](../site.hackery.paramorphism.api.resources/-resource/index.md), e.g. from the contents of a JAR file.


|

##### [site.hackery.paramorphism.api.config.strategies.obfuscation.stripping.SourceFileStrippingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.obfuscation.stripping/-source-file-stripping-strategy-config/index.md)

Contains settings for the "Source File Stripping" obfuscation strategy.


|

##### [site.hackery.paramorphism.api.config.strategies.scenarios.spigot.SpigotRemapPluginYMLStrategyConfig](../site.hackery.paramorphism.api.config.strategies.scenarios.spigot/-spigot-remap-plugin-y-m-l-strategy-config.md)

Contains settings for the "Spigot Remap 'plugin.yml'" strategy.


|

##### [site.hackery.paramorphism.api.config.StrategyConfiguration](../site.hackery.paramorphism.api.config/-strategy-configuration/index.md)

Contains base values needed for all obfuscation strategies.


|

##### [site.hackery.paramorphism.api.config.StrategyIrregularity](../site.hackery.paramorphism.api.config/-strategy-irregularity.md)

For internal use. Some irregularities can determine the default [StrategyConfiguration.enabled](../site.hackery.paramorphism.api.config/-strategy-configuration/enabled.md) state.


|

##### [site.hackery.paramorphism.api.config.strategies.concealment.StringConcealingStrategyConfig](../site.hackery.paramorphism.api.config.strategies.concealment/-string-concealing-strategy-config.md)

Contains settings for the "string concealing" obfuscation strategy.
"String Concealing" uses accessor methods to hide the original string constants of a class


|

##### [site.hackery.paramorphism.api.config.naming.UniformNameGenerationDictionaries](../site.hackery.paramorphism.api.config.naming/-uniform-name-generation-dictionaries/index.md)

An implementation of [NameGenerationConfig](../site.hackery.paramorphism.api.config.naming/-name-generation-config/index.md). Uses one dictionary and applies it to every element type.


