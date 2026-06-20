[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Dart](../../../../code-dart.md) > [Solutions](../../../code-dart-solutions.md) > [Hello World](../../code-dart-solutions-hello-world.md) > [Adapters](../code-dart-solutions-hello-world-adapters.md) > CLI

# Code Dart Solutions Hello World Adapters CLI

## Requirements

- [Tools Flutter Install macOS](../../../../../../tools/flutter/install/macos/tools-flutter-install-macos.md)

## Code

### Create application

```bash
dart create -t console-simple cli
cd cli
dart pub add --dev test
```

### Add .gitignore snippet

- [Code Dart Snippets .gitignore](../../../../snippets/gitignore/code-dart-snippets-gitignore.md)

### Add Hello World library

- [Code Dart Solutions Hello World Library](../../library/code-dart-solutions-hello-world-library.md)

### Add main function

```bash
touch bin/cli.dart
printf '%s\n' \
  'import "package:cli/hello_world.dart";' \
  '' \
  'void main(List<String> arguments) {' \
  '  print(helloWorld());' \
  '}' \
  | tee bin/cli.dart > /dev/null
```

### Add CLI test

```bash
touch test/cli_test.dart
printf '%s\n' \
  'import "dart:io";' \
  '' \
  'import "package:test/test.dart";' \
  '' \
  'void main() {' \
  '  test("prints Hello, world!", () async {' \
  '    final result = await Process.run("dart", ["run", "bin/cli.dart"]);' \
  '' \
  '    expect(result.exitCode, 0);' \
  '    expect(result.stdout, "Hello, world!\n");' \
  '    expect(result.stderr, "");' \
  '  });' \
  '}' \
  | tee test/cli_test.dart > /dev/null
```

### Check if builds

```bash
dart analyze
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
dart test
```

### Run locally

```bash
dart run
```
