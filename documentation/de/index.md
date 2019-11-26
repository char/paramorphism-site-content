---
title: Einführung
order: 1
---

Paramorphism ist ein Obfuscator für JVM (Java Virtual Machine) Bytecode.

Paramorphism unterstützt (und wurde getestet mit) Java 8, Java 13, Kotlin, und Groovy, aber sollte mit anderen Sprachen auch funktionieren, solange sie nicht schwer auf By-Name Dynamic Dispatch bzw. Reflection angewiesen sind.

## Quick Start

Um Paramorphism zu benutzen, mach einfach folgendes:

1. Erstelle dein Java-Projekt
2. Builde das Projekt als JAR-Datei
3. Erstelle eine Konfiguration in YAML oder JSON
4. Führe Paramorphism mit der Konfiguration aus

In dieser Dokumentation verwenden alle Konfigurationsbeispiele YAML. Hier ist eine Beispielkonfiguration für ein simples 'Hello, world!' Programm:

```yml
input: hello-world.jar
```

Falls ausgeführt mit `java -jar paramorphism-$version.jar config.yml`, dann wird eine obfuscatetes 'Hello, world!' Programm neben der `hello-world.jar` Datei mit dem Namen `hello-world.obf.jar` ausgegeben.

## Community

Du kannst unseren [Discord server](https://discord.gg/DT5NfYT) für informativen Support und Diskussion über Java Obfuscation beitreten.

Falls du ein zahlender Kunde bist, dann schreibe den leitenden Programmier an, um die 'Customer' Rolle zu bekommen (die Automatisierung dieses Prozesses ist geplannt), damit du in anderen Orten als in den 'off-topic' Channel zu schreiben kannst.

If you wish to report issues that occur during obfuscation (e.g. program behaviour breaks or the obfuscator crashes when trying to parse a project), please head on over to the project's [GitHub issue tracker](https://github.com/SerenityEnterprises/paramorphism-issues/).

Falls du das Verlangen hast ein Problem, das während der Obfuscation auftritt (z.B. Programmverhalten fehlerhaft oder der Obfuscator crasht beim Versuch das Projekt zu parsen), zu melden, dann gehe zum [GitHub issue tracker](https://github.com/SerenityEnterprises/paramorphism-issues/) des Projekts.