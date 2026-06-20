[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Flutter](../../../code-flutter.md) > [Solutions](../../code-flutter-solutions.md) > [Hello World](../code-flutter-solutions-hello-world.md) > Library

# Code Flutter Solutions Hello World Library

## Library

```bash
mkdir -p lib test
touch lib/hello_world_app.dart test/hello_world_app_test.dart
printf '%s\n' \
  'import "package:flutter/material.dart";' \
  '' \
  'class HelloWorldApp extends StatelessWidget {' \
  '  const HelloWorldApp({super.key});' \
  '' \
  '  @override' \
  '  Widget build(BuildContext context) {' \
  '    return const MaterialApp(' \
  '      home: Scaffold(' \
  '        body: Center(' \
  '          child: Text("Hello, world!"),' \
  '        ),' \
  '      ),' \
  '    );' \
  '  }' \
  '}' \
  | tee lib/hello_world_app.dart > /dev/null
printf '%s\n' \
  'import "package:flutter_test/flutter_test.dart";' \
  'import "package:app/hello_world_app.dart";' \
  '' \
  'void main() {' \
  '  testWidgets("shows Hello, world!", (tester) async {' \
  '    await tester.pumpWidget(const HelloWorldApp());' \
  '' \
  '    expect(find.text("Hello, world!"), findsOneWidget);' \
  '  });' \
  '}' \
  | tee test/hello_world_app_test.dart > /dev/null
```
