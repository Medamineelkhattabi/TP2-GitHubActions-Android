# TP2 · GitHub Actions for Android

Practical exercise: a continuous integration pipeline with GitHub Actions for an Android app
written in Kotlin (Jetpack Compose).

## CI

[`.github/workflows/android-ci.yml`](.github/workflows/android-ci.yml) runs on every push and pull
request to `main`:

1. Set up JDK 17.
2. Build the project: `./gradlew build`.
3. Run the unit tests: `./gradlew :app:testDebugUnitTest`.

## Run it locally

```bash
./gradlew build
./gradlew :app:testDebugUnitTest
```

Open the project in Android Studio to run the app on an emulator or a device.
