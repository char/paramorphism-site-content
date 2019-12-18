[paramorphism](../index.md) / [site.hackery.paramorphism.api.config](./index.md)

## Package site.hackery.paramorphism.api.config

Contains classes used for configuring the behaviour of Paramorphism.

### Types

| Name | Summary |
|---|---|
| [ElementMask](-element-mask/index.md) | Determines which elements to let through based on its 'include' and 'exclude' values.`interface ElementMask` |
| [ParamorphismConfig](-paramorphism-config/index.md) | Contains global configuration values to define the behaviour of the program as a whole.`interface ParamorphismConfig` |
| [StrategyConfiguration](-strategy-configuration/index.md) | Contains base values needed for all obfuscation strategies.`interface StrategyConfiguration` |
| [StrategyIrregularity](-strategy-irregularity.md) | For internal use. Some irregularities can determine the default [StrategyConfiguration.enabled](-strategy-configuration/enabled.md) state.`interface StrategyIrregularity` |

### Exceptions

| Name | Summary |
|---|---|
| [ConfigurationException](-configuration-exception/index.md) | Thrown when there is an issue parsing a configuration.`class ConfigurationException : `[`Exception`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-exception/index.html) |
