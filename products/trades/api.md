---
icon: gears
---

# Developer API

#### Gradle (Kotlin DSL)

```kotlin
repositories {
    maven("https://repo.runith.net/")
}

dependencies { 
    compileOnly("net.runith:trades-api:1.0.0")
}
```

#### Gradle (Groovy DSL)

```groovy
repositories {
    maven {
        url "https://repo.runith.net/"
    }
}

dependencies { 
    compileOnly "net.runith:trades-api:1.0.0"
}
```

### Maven

```xml
<repositories>
    <repository>
        <id>runith-repo</id>
        <url>https://repo.runith.net/</url>
    </repository>
</repositories>

<dependencies>
    <dependency>
      <groupId>net.runith</groupId>
      <artifactId>trades-api</artifactId>
      <version>1.0.0</version>
      <scope>compile</scope>
    </dependency>
</dependencies>
```
