[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Rust](../../../code-rust.md) > [Solutions](../../code-rust-solutions.md) > [Hello World](../code-rust-solutions-hello-world.md) > Library

# Code Rust Solutions Hello World Library

## Library

```bash
touch src/lib.rs
vi src/lib.rs
```

```rust
pub fn hello_world() -> &'static str {
    "Hello, world!"
}

#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn returns_hello_world() {
        assert_eq!(hello_world(), "Hello, world!");
    }
}
```

