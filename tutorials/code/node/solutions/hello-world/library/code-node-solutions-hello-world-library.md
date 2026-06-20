[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Node](../../../code-node.md) > [Solutions](../../code-node-solutions.md) > [Hello World](../code-node-solutions-hello-world.md) > Library

# Code Node Solutions Hello World Library

## Library

```bash
mkdir -p src test
touch src/hello-world.js test/hello-world.test.js
printf '%s\n' \
  'export function helloWorld() {' \
  '  return "Hello, world!";' \
  '}' \
  | tee src/hello-world.js > /dev/null
printf '%s\n' \
  'import assert from "node:assert/strict";' \
  'import test from "node:test";' \
  'import { helloWorld } from "../src/hello-world.js";' \
  '' \
  'test("returns Hello, world!", () => {' \
  '  assert.equal(helloWorld(), "Hello, world!");' \
  '});' \
  | tee test/hello-world.test.js > /dev/null
```
