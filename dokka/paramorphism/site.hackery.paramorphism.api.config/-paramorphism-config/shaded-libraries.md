[paramorphism](../../index.md) / [site.hackery.paramorphism.api.config](../index.md) / [ParamorphismConfig](index.md) / [shadedLibraries](./shaded-libraries.md)

# shadedLibraries

`open val shadedLibraries: `[`ElementMask`](../-element-mask/index.md)`?`

Defines which elements in the class file should be treated as 'shaded libraries', which are untouched by any
obfuscation strategy.

Shaded libraries are assumed to not have any dependency on any of the target application's internal classes.

