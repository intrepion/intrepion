[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Rust](../../../../code-rust.md) > [Solutions](../../../code-rust-solutions.md) > [Hello World](../../code-rust-solutions-hello-world.md) > [Adapters](../code-rust-solutions-hello-world-adapters.md) > CLI

# Code Rust Solutions Hello World Adapters CLI

## Requirements

- [Tools Rust Install macOS](../../../../../../tools/rust/install/macos/tools-rust-install-macos.md)

## Code

### Create application

```bash
cargo new cli
cd cli
```

### Add .gitignore snippet

- [Code Rust Snippets .gitignore](../../../../snippets/gitignore/code-rust-snippets-gitignore.md)

### Add Hello World library

- [Code Rust Solutions Hello World Library](../../library/code-rust-solutions-hello-world-library.md)

### Add main function

```bash
touch src/main.rs
vi src/main.rs
```

```rust
fn main() {
    println!("{}", cli::hello_world());
}
```

### Add CLI test

```bash
mkdir -p tests
touch tests/cli.rs
vi tests/cli.rs
```

```rust
use std::process::Command;

#[test]
fn prints_hello_world() {
    let output = Command::new(env!("CARGO_BIN_EXE_cli"))
        .output()
        .expect("failed to run cli");

    assert!(output.status.success());
    assert_eq!(String::from_utf8_lossy(&output.stdout), "Hello, world!\n");
    assert_eq!(String::from_utf8_lossy(&output.stderr), "");
}
```

### Check if builds

```bash
cargo check
```

### Check formatting

```bash
cargo fmt --check
```

### Correct formatting

```bash
cargo fmt
```

### Run tests

```bash
cargo test
```

### Build for development

```bash
cargo build
```
### Build for production

```bash
cargo build --release
```

### Run locally

```bash
cargo run
```
