[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Go](../../../code-go.md) > [Solutions](../../code-go-solutions.md) > [Hello World](../code-go-solutions-hello-world.md) > Library

# Code Go Solutions Hello World Library

## Library

```bash
touch hello_world.go
printf '%s\n' \
  'package hello_world' \
  '' \
  'func HelloWorld() string {' \
  '	return "Hello, world!"' \
  '}' \
  | tee hello_world.go > /dev/null
touch hello_world_test.go
printf '%s\n' \
  'package hello_world_test' \
  '' \
  'import (' \
  '	"testing"' \
  '' \
  '	hello_world "."' \
  ')' \
  '' \
  'func TestReturnsHelloWorld(t *testing.T) {' \
  '	got := hello_world.HelloWorld()' \
  '	want := "Hello, world!"' \
  '	if got != want {' \
  '		t.Errorf("got %q, want %q", got, want)' \
  '	}' \
  '}' \
  | tee hello_world_test.go > /dev/null
```
