[paramorphism](../../index.md) / [site.hackery.paramorphism.api.naming](../index.md) / [Dictionaries](./index.md)

# Dictionaries

`object Dictionaries`

The built-in dictionaries to the obfuscator.

### Properties

| Name | Summary |
|---|---|
| [ALPHABET](-a-l-p-h-a-b-e-t.md) | Contains the letters 'a' to 'z' as individual mapping elements`val ALPHABET: `[`MappingDictionary`](../-mapping-dictionary/index.md) |
| [ALPHABET_UPPER](-a-l-p-h-a-b-e-t_-u-p-p-e-r.md) | Contains the letters 'A' to 'Z' as individual mapping elements`val ALPHABET_UPPER: `[`MappingDictionary`](../-mapping-dictionary/index.md) |
| [dictionaryMap](dictionary-map.md) | For internal use. Maps dictionary names to the built-in [MappingDictionaries](../-mapping-dictionary/index.md).`val dictionaryMap: `[`Map`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-map/index.html)`<`[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, `[`MappingDictionary`](../-mapping-dictionary/index.md)`>` |
| [JAVA_KEYWORDS](-j-a-v-a_-k-e-y-w-o-r-d-s.md) | Contains every reserved keyword in Java`val JAVA_KEYWORDS: `[`MappingDictionary`](../-mapping-dictionary/index.md) |
| [LOOKALIKES](-l-o-o-k-a-l-i-k-e-s.md) | Contains 'lookalike' characters - 'L', 'I', '1', 'i', and 'l'.`val LOOKALIKES: `[`MappingDictionary`](../-mapping-dictionary/index.md) |
