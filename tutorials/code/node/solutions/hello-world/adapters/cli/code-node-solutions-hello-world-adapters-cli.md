[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Node](../../../../code-node.md) > [Solutions](../../../code-node-solutions.md) > [Hello World](../../code-node-solutions-hello-world.md) > [Adapters](../code-node-solutions-hello-world-adapters.md) > CLI

# Code Node Solutions Hello World Adapters CLI

## Requirements

- [Tools nvm Install macOS](../../../../../../tools/nvm/install/macos/tools-nvm-install-macos.md)

## Code

### Create application

```bash
mkdir cli
cd cli
npm init -y
npm pkg set type=module
npm pkg set scripts.check="node --check src/*.js test/*.js"
npm pkg set scripts.test="node --test"
npm pkg set scripts.start="node src/main.js"
```

### Add .gitignore snippet

- [Code Node Snippets .gitignore](../../../../snippets/gitignore/code-node-snippets-gitignore.md)

### Add Hello World library

- [Code Node Solutions Hello World Library](../../library/code-node-solutions-hello-world-library.md)

### Add main function

```bash
touch src/main.js
printf '%s\n' \
  'import { helloWorld } from "./hello-world.js";' \
  '' \
  'console.log(helloWorld());' \
  | tee src/main.js > /dev/null
```

### Add CLI test

```bash
touch test/cli.test.js
printf '%s\n' \
  'import assert from "node:assert/strict";' \
  'import { execFile } from "node:child_process";' \
  'import test from "node:test";' \
  'import { promisify } from "node:util";' \
  '' \
  'const execFileAsync = promisify(execFile);' \
  '' \
  'test("prints Hello, world!", async () => {' \
  '  const { stdout, stderr } = await execFileAsync("node", ["src/main.js"]);' \
  '' \
  '  assert.equal(stdout, "Hello, world!\n");' \
  '  assert.equal(stderr, "");' \
  '});' \
  | tee test/cli.test.js > /dev/null
```

### Check if builds

```bash
npm run check
```

### Run tests

```bash
npm test
```

### Run locally

```bash
npm start
```
