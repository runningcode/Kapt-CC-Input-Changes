# Kapt Configuration Cache Input changes in Gradle 8.1

## Reproduction steps

1. `rm -rf .gradle/configuration-cache/*`
2. `./gradlew clean`
3. `./gradlew assDebg`
4. `./gradlew assDebug`