# Introduction

Paramorphism is an obfuscator for JVM (Java Virtual Machine) bytecode. Paramorphism supports (and is tested with) Java 8, Java 13, Kotlin, and Groovy, but should work on other languages as long as they do not heavily rely on by-name dynamic dispatch (i.e. reflection)

## Quick Guide

To use Paramorphism, simply:

1. Create your Java project
2. Build it as a JAR file
3. Create a configuration in YAML or JSON
4. Run Paramorphism against the configuration

In this documentation, all configuration examples will use YAML. Here is an example configuration for a 'Hello, world!' example.

```yml
input: hello-world.jar
```

This will emit an obfuscated 'Hello, world!' program next to `hello-world.jar` named `hello-world.obf.jar`.
