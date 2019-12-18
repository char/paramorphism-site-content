[paramorphism](../../index.md) / [site.hackery.paramorphism.api.resources](../index.md) / [Resource](./index.md)

# Resource

`sealed class Resource`

A [Resource](./index.md) is used to represent data inside a JAR file.

### Properties

| Name | Summary |
|---|---|
| [data](data.md) | `abstract val data: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html) |
| [order](order.md) | `val order: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [BufferResource](../-buffer-resource/index.md) | A BufferResource is a [Resource](./index.md) that contains a byte array`class BufferResource : `[`Resource`](./index.md) |
| [ManifestResource](../-manifest-resource/index.md) | A ManifestResource is a [Resource](./index.md) that represents a JAR file's META-INF/MANIFEST.MF file`class ManifestResource : `[`Resource`](./index.md) |
