# Kapt Configuration Cache Input changes in Gradle 8.1

## Reproduction steps

1. `rm -rf .gradle/configuration-cache/*`
2. `./gradlew clean`
3. `./gradlew assDebg`
4. `./gradlew assDebug`

On the second build you will see: `Calculating task graph as configuration cache cannot be reused because an input to plugin 'com.android.internal.library' has changed.`

Bug filed here: https://youtrack.jetbrains.com/issue/KT-58167/Applying-KAPT-plugin-to-Gradle-8.1-causes-configuration-cache-miss
