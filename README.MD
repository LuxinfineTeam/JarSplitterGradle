# JarSplitter-Gradle

**JarSplitter-Gradle** - аналог [`Cutter`](https://forum.mcmodding.ru/resources/vyrezalka-2.198/) от JustAGod с полной поддержкой распила на клиент, сервер и дев билды.

# Пример подключения в `build.gradle`
```groovy
buildscript {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
    dependencies {
        ...
        // Замените ${VERSION} на актуальную версию
        classpath "com.github.LuxinfineTeam:JarSplitterGradle:${VERSION}"
    }
}

repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.LuxinfineTeam:JarSplitterGradle:api'
}
```

# Плагин предоставит Gradle таски:
- `buildClient` - сборка клиентской версии Jar
- `buildServer` - сборка серверной версии Jar
- `buildDev` - сборка DEV версии Jar. По сути, это сборка мода БЕЗ распила с деобфускацией майнкрафт маппингов. Да, можно получить такой jar и вручную, но таск чисто для удобства
- `buildAll` - сборка всех 3 версий Jar

# Актуальная версия плагина: [![](https://jitpack.io/v/LuxinfineTeam/JarSplitterGradle.svg)](https://jitpack.io/#LuxinfineTeam/JarSplitterGradle)