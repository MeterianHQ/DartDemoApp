# DartDemoApp
A demo application to show support for Dart in Meterian

## Meterian Scanner pipeline specification

The [Meterian Scanner GitHub action](https://github.com/MeterianHQ/meterian-github-action) is configured to perform a vulnerability scan of the demo app.

The default configuration employ version v1.0.17 which does not include the Dart SDK and generates security insights by consulting the `pubspec.lock`.

For a more accurate result you can uncomment the line below in the [configuration](.github/workflows/main.yml) to use a dedicated variant of the action which includes the Dart SDK.

```
uses: MeterianHQ/meterian-github-action@latest-dart
```
