[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [SpaceTimeDB](../../../../code-spacetimedb.md) > [Solutions](../../../code-spacetimedb-solutions.md) > [Hello World](../../code-spacetimedb-solutions-hello-world.md) > [Adapters](../code-spacetimedb-solutions-hello-world-adapters.md) > Server

# Code SpaceTimeDB Solutions Hello World Adapters Server

## Requirements

- [Tools Rust Install macOS](../../../../../../tools/rust/install/macos/tools-rust-install-macos.md)
- [Tools SpaceTimeDB Install macOS](../../../../../../tools/spacetimedb/install/macos/tools-spacetimedb-install-macos.md)

## Code

### Create application

```bash
spacetime dev --template basic-rs
```

### Add .gitignore snippet

- [Code Rust Snippets .gitignore](../../../../../rust/snippets/gitignore/code-rust-snippets-gitignore.md)
- [Code SpaceTimeDB Snippets .gitignore](../../../../snippets/gitignore/code-spacetimedb-snippets-gitignore.md)

### Add Hello World library

- [Code SpaceTimeDB Solutions Hello World Library](../../library/code-spacetimedb-solutions-hello-world-library.md)

### Check if builds

```bash
spacetime build
```

### Publish locally

```bash
spacetime publish hello-world
```

### Call reducer

```bash
spacetime call add Alice
```

### Query table

```bash
spacetime sql "SELECT * FROM person"
```

### View logs

```bash
spacetime call say_hello
spacetime logs
```
