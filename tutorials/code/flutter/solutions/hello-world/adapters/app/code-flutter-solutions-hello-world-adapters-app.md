[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Flutter](../../../../code-flutter.md) > [Solutions](../../../code-flutter-solutions.md) > [Hello World](../../code-flutter-solutions-hello-world.md) > [Adapters](../code-flutter-solutions-hello-world-adapters.md) > App

# Code Flutter Solutions Hello World Adapters App

## Requirements

- [Tools Flutter Install macOS](../../../../../../tools/flutter/install/macos/tools-flutter-install-macos.md)

## Code

### Create application

```bash
flutter create app
cd app
```

### Add .gitignore snippet

- [Code Flutter Snippets .gitignore](../../../../snippets/gitignore/code-flutter-snippets-gitignore.md)

### Add Hello World library

- [Code Flutter Solutions Hello World Library](../../library/code-flutter-solutions-hello-world-library.md)

### Add main function

```bash
touch lib/main.dart
printf '%s\n' \
  'import "package:app/hello_world_app.dart";' \
  'import "package:flutter/widgets.dart";' \
  '' \
  'void main() {' \
  '  runApp(const HelloWorldApp());' \
  '}' \
  | tee lib/main.dart > /dev/null
```

### Check if builds

```bash
flutter analyze
```

### Check formatting

```bash
dart format --output=none --set-exit-if-changed .
```

### Correct formatting

```bash
dart format .
```

### Run tests

```bash
flutter test
```

### Run locally

```bash
flutter run
```
