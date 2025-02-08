### 1  android\app\build.gradle:
```
android {
  ndkVersion = "25.1.8937393"

compileOptions {
  sourceCompatibility = JavaVersion.VERSION_17
  targetCompatibility = JavaVersion.VERSION_17
}
kotlinOptions {
  jvmTarget = 17
}
```

### 2 android\settings.gradle:
```
id "com.android.application" version "8.3.2" apply false
id "org.jetbrains.kotlin.android" version "2.0.20" apply false
```

### 3   android\gradle\wrapper\gradle-wrapper.properties
```
distributionUrl=https\://services.gradle.org/distributions/gradle-8.10.2-all.zip
```

### 3 Clean Gradle Build Files(Open terminal and run)
```
cd android
./gradlew clean
```

### 4 Restart Android Studio and run(Optional)
```
flutter clean
flutter pub get
flutter run
```