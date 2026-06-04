[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [Rust](../../tools-rust.md) > [Install](../tools-rust-install.md) > macOS

# Rust Install macOS

## Requirements

- [Xcode Command Line Tools](../../../xcode-command-line-tools/install/macos/tools-xcode-command-line-tools-install-macos.md)

## Install

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Update

```bash
rustup update
```

## Check Location

```bash
which cargo
which rustc
which rustfmt
```

should be something like

```text
$ which cargo
/Users/oliverforral/.cargo/bin/cargo
$ which rustc
/Users/oliverforral/.cargo/bin/rustc
$ which rustfmt
/Users/oliverforral/.cargo/bin/rustfmt
```
