[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [C#](../../../../code-csharp.md) > [Solutions](../../../code-csharp-solutions.md) > [Hello World](../../code-csharp-solutions-hello-world.md) > [Adapters](../code-csharp-solutions-hello-world-adapters.md) > CLI

# Code C# Solutions Hello World Adapters CLI

## Requirements

- [Tools .NET Install macOS](../../../../../../tools/dotnet/install/macos/tools-dotnet-install-macos.md)

## Code

### Create application

```bash
dotnet new console --name Cli
cd cli
```

### Add .gitignore snippet

- [Code C# Snippets .gitignore](../../../../snippets/gitignore/code-csharp-snippets-gitignore.md)

### Add Hello World library

- [Code C# Solutions Hello World Library](../../library/code-csharp-solutions-hello-world-library.md)

### Add main function

```bash
touch bin/cli.csharp
printf '%s\n' \
  'import "package:cli/hello_world.csharp";' \
  '' \
  'void main(List<String> arguments) {' \
  '  print(helloWorld());' \
  '}' \
  | tee bin/cli.csharp > /dev/null
```

### Add CLI test

```bash
touch test/cli_test.csharp
printf '%s\n' \
  'import "csharp:io";' \
  '' \
  'import "package:test/test.csharp";' \
  '' \
  'void main() {' \
  '  test("prints Hello, world!", () async {' \
  '    final result = await Process.run("csharp", ["run", "bin/cli.csharp"]);' \
  '' \
  '    expect(result.exitCode, 0);' \
  '    expect(result.stdout, "Hello, world!\n");' \
  '    expect(result.stderr, "");' \
  '  });' \
  '}' \
  | tee test/cli_test.csharp > /dev/null
```

### Check if builds

```bash
csharp analyze
```

### Check formatting

```bash
csharp format --output=none --set-exit-if-changed .
```

### Correct formatting

```bash
csharp format .
```

### Run tests

```bash
csharp test
```

### Run locally

```bash
csharp run
```
