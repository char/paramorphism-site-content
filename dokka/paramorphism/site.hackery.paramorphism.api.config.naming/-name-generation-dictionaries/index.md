[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.naming](../index.md) / [NameGenerationDictionaries](./index.md)

# NameGenerationDictionaries

`interface NameGenerationDictionaries`

Contains dictionaries to use on different elements

### Properties

| Name | Summary |
|---|---|
| [classes](classes.md) | The dictionary to use for class names`abstract val classes: `[`MappingDictionary`](../../site.hackery.paramorphism.api.naming/-mapping-dictionary/index.md) |
| [fields](fields.md) | The dictionary to use for field names`abstract val fields: `[`MappingDictionary`](../../site.hackery.paramorphism.api.naming/-mapping-dictionary/index.md) |
| [methods](methods.md) | The dictionary to use for method names`abstract val methods: `[`MappingDictionary`](../../site.hackery.paramorphism.api.naming/-mapping-dictionary/index.md) |
| [packages](packages.md) | The dictionary to use for package segments`abstract val packages: `[`MappingDictionary`](../../site.hackery.paramorphism.api.naming/-mapping-dictionary/index.md) |

### Inheritors

| Name | Summary |
|---|---|
| [UniformNameGenerationDictionaries](../-uniform-name-generation-dictionaries/index.md) | An implementation of [NameGenerationConfig](../-name-generation-config/index.md). Uses one dictionary and applies it to every element type.`class UniformNameGenerationDictionaries : `[`NameGenerationDictionaries`](./index.md) |
