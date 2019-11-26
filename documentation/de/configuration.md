---
title: Konfiguration
order: 2
---

## Input & Output

`input` definiert den Pfad, auf dem das Zielartefakt gefunden werden kann, währenddessen `output` deklariert wo der obfuscatete Output ausgegeben wird.

Diese Pfade sind entweder relativ zu dem Standort der Konfigurationsdatei oder absolut, ausgenommen absolute Basispfade (z.B. `/` in den meisten Betriebssystem, oder ein Laufwerksbuchstabe, wie z.B. `C:/` in Windows).

**Beispiel:**

```yml
input: path/to/application.jar
output: obfuscated-application.jar
```

## Libraries

`libraries` ist eine einfache Liste von JAR-Datien (oder Verzeichnisse von JAR-Dateien). Um `libraries` zu benutzen, liste die JAR-Dateien und/oder Verzeichnisse, die du einbinden willst, auf. Genau wie `input` und `output`, diese Pfade sind relativ zu dem Standort der Konfigurationsdatei.

**Note**: Damit der Remapper korrekt funktioniert müssen alle Libraries, die die Applikation benötigt, in der Konfigurationsdatei deklariert werden.

Dies liegt daran, dass der Obfuscator die Vererbungshierarchie der Klassen verarbeiten muss, um überschriebene Methoden in Klassen korrekt zuzuordnen. Auf diese Weise wird sichergestellt, dass die Member, die Superklassen von Drittanbietern überschreiben, nicht erneut zugeordnet werden. (Ansonsten würde das zu `AbstractMethodError`s führen, wenn man den Code ausführt.)

## Element Masks

An element mask defines which elements are to be included and excluded in an obfuscation pass. The global mask is defined by the `mask` entry in the configuration file, and controls which classes **any** obfuscation strategy can touch.

Eine Element Mask definiert welche Elemente von dem Obfuscation Prozess ein- und ausgeschlossen werden. Die globale Maske wird von dem `mask` Eintrag in der Konfigurationsdatei definiert und kontrolliert welche Klassen von **irgendeiner** Obfuscation Strategie angefasst werden können.

```yml
input: myproject-1.0.0.jar

mask: # Definiere die globale Maske für den Obfuscator
  include:                             # We want to limit the scope of obfuscations to only:
                                       # Wir möchten den Umfang der Obfuscations zu:
    - com/example/myproject/           # - unser eigenes Projekt,
    - org/business/proprietarylibrary/ # - und eine Drittanbieterversion einer Library, die an uns vergeben wurde limitieren.
  exclude:
                                       # Und von denen wollen wir folgendes ausschließen:
    - com/example/myproject/api/       # - unsere öffentlich-gerichtete API.

    # Da wir über diese Klasse serialisieren (z.B. über Gson), wollen wir nicht die Feldnamen obfuscaten, deswegen werden wir es auch ausschließen:
    - com/example/myproject/config/ConfigurationJSONBean
```

### Übereinstimmungsregeln

In einer Element Mask, `include` und `exclude` und eine Liste von *Übereinstimmungsregeln*.

- **Package:** Falls die Regel mit `/` endet, dann wird es alles, was mit der Regel anfängt, übereinstimmen. Zum Beispiel, die Regel `path/rule` stimmt mit `path/rule/One`, `path/rule/Two`, aber nicht mit `other/path/MyClass` überein.
- **Wildcard:** Falls eine Regel mit `*` endet, dann wird es alles, was mit der Regel anfängt (ausgenommen das Sternchen), übereinstimmen. Zum Beispiel, die Regel `wildcard/rule*` stimmt mit `wildcard/rule/one`, `wildcard/ruletwothreefour/five`, aber nicht mit `wildcard/notrule/anythingelse` überein.
- **Literal:** Ansonsten wird die Regel alles übereinstimmen, was identisch zu sich selbst ist.
