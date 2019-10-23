[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config.strategies.obfuscation](../index.md) / [SourceFileStrippingStrategyConfig](index.md) / [sourceFile](./source-file.md)

# sourceFile

`open fun sourceFile(internalName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`?`

Maps a class' *internal name* to a value of the SourceFile attribute.
Returning `null` wipes the SourceFile attribute.

For instance, to mimic the default `javac` behaviour, one would return the simple name of the class, plus `".java"`

