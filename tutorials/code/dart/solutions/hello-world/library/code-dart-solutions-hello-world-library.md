[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Dart](../../../code-dart.md) > [Solutions](../../code-dart-solutions.md) > [Hello World](../code-dart-solutions-hello-world.md) > Library

# Code Dart Solutions Hello World Library

## Library

```bash
mkdir -p lib test
touch lib/hello_world.dart test/hello_world_test.dart
printf '%s\n' \
  'String helloWorld() {' \
  '  return "Hello, world!";' \
  '}' \
  | tee lib/hello_world.dart > /dev/null
printf '%s\n' \
  'import "package:test/test.dart";' \
  'import "package:cli/hello_world.dart";' \
  '' \
  'void main() {' \
  '  test("returns Hello, world!", () {' \
  '    expect(helloWorld(), "Hello, world!");' \
  '  });' \
  '}' \
  | tee test/hello_world_test.dart > /dev/null
```
