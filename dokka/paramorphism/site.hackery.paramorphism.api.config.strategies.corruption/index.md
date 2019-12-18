[paramorphism](../index.md) / [site.hackery.paramorphism.api.config.strategies.corruption](./index.md)

## Package site.hackery.paramorphism.api.config.strategies.corruption

Contains configuration objects for obfuscation strategies in the "corruption" category.

### Types

| Name | Summary |
|---|---|
| [DeeplyNestedClassInjectionStrategyConfig](-deeply-nested-class-injection-strategy-config/index.md) | Contains settings for the "Deeply Nested Class Injection" strategy. Disabled by default.`interface DeeplyNestedClassInjectionStrategyConfig : `[`StrategyConfiguration`](../site.hackery.paramorphism.api.config/-strategy-configuration/index.md) |
| [ForceNoVerifyStrategyConfig](-force-no-verify-strategy-config/index.md) | Contains settings for the "Force No Verify" strategy. Enabled by default when 'Main-Class' is detected in the manifest.`interface ForceNoVerifyStrategyConfig : `[`StrategyConfiguration`](../site.hackery.paramorphism.api.config/-strategy-configuration/index.md) |
| [NullByteNamingStrategyConfig](-null-byte-naming-strategy-config/index.md) | Contains settings for the "Null Byte Naming" obfuscation strategy.`interface NullByteNamingStrategyConfig : `[`StrategyConfiguration`](../site.hackery.paramorphism.api.config/-strategy-configuration/index.md) |
