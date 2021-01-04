An example of running appium_dart

## Setup
Install Android SDK
Install Flutter SDK (automatically installs DART SDK)

## To run
* Start emulator or attach mobile (ensure device name is in helper.dart, e.g. emulator-5554)
* Start appium server (Appium desktop is OK, the flutter appium driver in a Dart package specified in pubspec.yaml)
* From command line in repo root:
```
$ flutter pub get
$ dart run appium_dart_android_test.dart
```
This process will unpack apk zipfile in the `app` folder, and install apk on device, then run tests
