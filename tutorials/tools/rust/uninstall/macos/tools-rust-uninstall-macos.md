[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Rust](../../tools-rust.md) > [Uninstall](../tools-rust-uninstall.md) > macOS

# Tools Rust Uninstall macOS

## Check Active Rust

```bash
rustc --version
which -a rustc
which -a cargo
rustup which rustc
```

If `which -a rustc`, `which -a cargo`, or `which -a rustfmt` prints a path outside `~/.cargo/bin`, another Rust install is still on your `PATH`.

## Uninstall rustup Rust

```bash
rustup self uninstall
```

## Uninstall Homebrew Rust

```bash
brew uninstall rust
```

## Uninstall MacPorts Rust

```bash
sudo port uninstall cargo
sudo port uninstall rust
```

## Remove User Data

```bash
rm -rf ~/.cargo
rm -rf ~/.rustup
```

## Check Location

```bash
which -a rustc
which -a cargo
which -a rustfmt
```

should print no paths

```text
$ which -a rustc
$ which -a cargo
$ which -a rustfmt
```

If `cargo` still resolves to `/opt/local/bin/cargo`, uninstall the MacPorts package or remove `/opt/local/bin` from your `PATH`.
