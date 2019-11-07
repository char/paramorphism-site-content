---
title: Introduction
order: 1
---

Paramorphism is an obfuscator for JVM (Java Virtual Machine) bytecode.

Paramorphism supports (and is tested with) Java 8, Java 13, Kotlin, and Groovy, but should work on other languages as long as they do not heavily rely on by-name dynamic dispatch (i.e. reflection).

## Quick Start

To use Paramorphism, simply:

1. Create your Java project
2. Build it as a JAR file
3. Create a configuration in YAML or JSON
4. Run Paramorphism against the configuration

In this documentation, all configuration examples will use YAML. Here is an example configuration for a simple 'Hello, world!' program:

```yml
input: hello-world.jar
```

When run with `java -jar paramorphism-$version.jar config.yml`, this will emit an obfuscated 'Hello, world!' program next to `hello-world.jar` named `hello-world.obf.jar`.

## Community

You can join the [Discord server](https://discord.gg/DT5NfYT) for informal support and discussion of Java obfuscation.

If you are a paying customer, message the lead developer to be allocated the Customer role
(automation of this is planned), and be able to talk in places other than the 'off-topic' channel.

If you wish to report issues that occur during obfuscation (e.g. program behaviour breaks or the obfuscator crashes when trying to parse a project), please head on over to the project's [GitHub issue tracker](https://github.com/SerenityEnterprises/paramorphism-issues/).
