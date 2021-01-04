An example of running appium_dart

## Setup
Install Android SDK
Install Flutter SDK (automatically installs DART SDK)

## To run
* Start emulator or attach mobile (ensure device name is in helper.dart, e.g. emulator-5554)
* Start appium server
* From command line in repo root:
```
$ flutter pub get
$ dart run appium_dart_android_test.dart
```
