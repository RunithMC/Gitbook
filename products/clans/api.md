---
icon: gears
---

# Developer API

#### Gradle (Kotlin DSL)

```kotlin
repositories {
    maven("https://raw.githubusercontent.com/RunithMC/maven/main/")
}

dependencies { 
    compileOnly("net.runith:clans-api:1.6.0")
}
```

#### Gradle (Groovy DSL)

```groovy
repositories {
    maven {
        url "https://raw.githubusercontent.com/RunithMC/maven/main/"
    }
}

dependencies { 
    compileOnly "net.runith:clans-api:1.6.0"
}
```

### Maven

```xml
<repositories>
    <repository>
        <id>runith-repo</id>
        <url>https://raw.githubusercontent.com/RunithMC/maven/main/</url>
    </repository>
</repositories>

<dependencies>
    <dependency>
      <groupId>net.runith</groupId>
      <artifactId>clans-api</artifactId>
      <version>1.6.0</version>
      <scope>compile</scope>
    </dependency>
</dependencies>
```
