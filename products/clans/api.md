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
    compileOnly("net.runith:clans-api:1.2.4")
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
    compileOnly "net.runith:clans-api:1.2.4"
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
      <artifactId>clans-api</artifactId>
      <version>1.2.4</version>
      <scope>compile</scope>
    </dependency>
</dependencies>
```
