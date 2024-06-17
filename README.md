# DartDemoApp
A demo application to show support for Dart in Meterian


[![security status](https://www.meterian.io/badge/pb/39a141e3-c78c-4e87-ab3e-43554a6e612b/security?branch=main)](https://www.meterian.io/projects/?pid=39a141e3-c78c-4e87-ab3e-43554a6e612b)
[![stability status](https://www.meterian.io/badge/pb/39a141e3-c78c-4e87-ab3e-43554a6e612b/stability?branch=main)](https://www.meterian.io/projects/?pid=39a141e3-c78c-4e87-ab3e-43554a6e612b)
[![licensing status](https://www.meterian.io/badge/pb/39a141e3-c78c-4e87-ab3e-43554a6e612b/licensing?branch=main)](https://www.meterian.io/projects/?pid=39a141e3-c78c-4e87-ab3e-43554a6e612b)




## Meterian Scanner pipeline specification

The [Meterian Scanner GitHub action](https://github.com/MeterianHQ/meterian-github-action) is configured to perform a vulnerability scan of the demo app.

The configuration employs version v1.0.17 which does not include the Dart SDK and generates security insights by consulting the `pubspec.lock` and as a results offers lower build times.

For a more accurate result you can uncomment the line below in the [configuration](.github/workflows/main.yml) to use a dedicated variant of the action which includes the Dart SDK.

```
uses: MeterianHQ/meterian-github-action@latest-dart
```
