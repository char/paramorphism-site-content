[paramorphism](../index.md) / [site.hackery.paramorphism.api.resources](./index.md)

## Package site.hackery.paramorphism.api.resources

### Types

| Name | Summary |
|---|---|
| [BufferResource](-buffer-resource/index.md) | A BufferResource is a [Resource](-resource/index.md) that contains a byte array`class BufferResource : `[`Resource`](-resource/index.md) |
| [ClassInfo](-class-info/index.md) | Information about a class contained in a [ClassSet](-class-set/index.md).`data class ClassInfo` |
| [ClassSet](-class-set/index.md) | A set of [ClassInfo](-class-info/index.md) objects identified by name.`interface ClassSet : `[`Closeable`](https://docs.oracle.com/javase/6/docs/api/java/io/Closeable.html) |
| [ClassSetGroup](-class-set-group/index.md) | A collected group of ClassSets, using a linear search for lookup.`class ClassSetGroup` |
| [EmptyClassNode](-empty-class-node.md) | An empty ClassNode — Used for deleting classes from a [ClassSet](-class-set/index.md).`object EmptyClassNode : ClassNode` |
| [ManifestResource](-manifest-resource/index.md) | A ManifestResource is a [Resource](-resource/index.md) that represents a JAR file's META-INF/MANIFEST.MF file`class ManifestResource : `[`Resource`](-resource/index.md) |
| [Resource](-resource/index.md) | A [Resource](-resource/index.md) is used to represent data inside a JAR file.`sealed class Resource` |
| [ResourceSet](-resource-set/index.md) | A set of [resources](-resource/index.md), e.g. from the contents of a JAR file.`interface ResourceSet : `[`Closeable`](https://docs.oracle.com/javase/6/docs/api/java/io/Closeable.html) |
