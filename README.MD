# JarSplitter-Gradle

**JarSplitter-Gradle** - аналог [`Cutter`](https://forum.mcmodding.ru/resources/vyrezalka-2.198/) от JustAGod с полной поддержкой распила на клиент, сервер и дев билды.

# Пример подключения в `build.gradle`
```groovy
//TODO: пример подключения самого плагина

repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.github.LuxinfineTeam:JarSplitterGradle:v1.0.0'
}
```

# Плагин предоставит Gradle таски:
- `buildClient` - сборка клиентской версии Jar
- `buildServer` - сборка серверной версии Jar
- `buildDev` - сборка DEV версии Jar. По сути, это сборка мода БЕЗ распила с деобфускацией майнкрафт маппингов. Да, можно получить такой jar и вручную, но таск чисто для удобства
- `buildAll` - сборка всех 3 версий Jar