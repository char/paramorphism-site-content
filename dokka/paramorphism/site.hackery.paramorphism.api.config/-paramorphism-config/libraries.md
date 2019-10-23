[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [ParamorphismConfig](index.md) / [libraries](./libraries.md)

# libraries

`open val libraries: `[`Array`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-array/index.html)`<`[`File`](https://docs.oracle.com/javase/6/docs/api/java/io/File.html)`>`

An array of JAR files defining the searched class path of the obfuscator.

All classes that are referenced in hierarchy should be included, since the remapper needs access to information
about which parent classes contain which methods.

Defaults to an empty array.

