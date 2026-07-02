[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Go](../../../../code-go.md) > [Solutions](../../../code-go-solutions.md) > [Hello World](../../code-go-solutions-hello-world.md) > [Adapters](../code-go-solutions-hello-world-adapters.md) > CLI

# Code Go Solutions Hello World Adapters CLI

## Requirements

- [Tools Go Install macOS](../../../../../../tools/go/install/macos/tools-go-install-macos.md)

## Code

### Create application

```bash
mkdir cli
cd cli
go mod init cli
```

### Add .gitignore snippet

- [Code Go Snippets .gitignore](../../../../snippets/gitignore/code-go-snippets-gitignore.md)

### Add Hello World library

- [Code Go Solutions Hello World Library](../../library/code-go-solutions-hello-world-library.md)

### Add main function

```bash
touch main.go
printf '%s\n' \
  'package main' \
  '' \
  'import (' \
  '	"fmt"' \
  '' \
  '	hello_world "."' \
  ')' \
  '' \
  'func main() {' \
  '	fmt.Println(hello_world.HelloWorld())' \
  '}' \
  | tee main.go > /dev/null
```

### Add CLI test

```bash
mkdir -p cmd
touch cmd/cli_test.go
printf '%s\n' \
  'package cmd_test' \
  '' \
  'import (' \
  '	"os/exec"' \
  '	"testing"' \
  ')' \
  '' \
  'func TestPrintsHelloWorld(t *testing.T) {' \
  '	cmd := exec.Command("go", "run", ".")' \
  '	output, err := cmd.CombinedOutput()' \
  '	if err != nil {' \
  '		t.Fatalf("command failed: %v\n%s", err, output)' \
  '	}' \
  '	got := string(output)' \
  '	want := "Hello, world!\n"' \
  '	if got != want {' \
  '		t.Errorf("got %q, want %q", got, want)' \
  '	}' \
  '}' \
  | tee cmd/cli_test.go > /dev/null
```

### Check if builds

```bash
go build ./...
```

### Check formatting

```bash
gofmt -l .
```

### Correct formatting

```bash
gofmt -w .
```

### Run tests

```bash
go test ./...
```

### Build for production

```bash
go build -o cli .
```

### Run locally

```bash
go run .
```
