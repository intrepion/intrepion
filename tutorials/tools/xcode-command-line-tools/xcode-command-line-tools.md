[Tutorials](../../tutorials.md) > Xcode Command Line Tools

# Xcode Command Line Tools

## Links

- [Website](https://developer.apple.com/xcode/)
- [Documentation](https://developer.apple.com/documentation/xcode/installing-the-command-line-tools)
- [Downloads](https://developer.apple.com/download/all/)
- [Releases](https://appledb.dev/device/Command-Line-Tools-for-Xcode.html)

## Versions

```bash
xcode-select --version
pkgutil --pkg-info=com.apple.pkg.CLTools_Executables
```

should be something like

```text
$ xcode-select --version
xcode-select version 2416.
$ pkgutil --pkg-info=com.apple.pkg.CLTools_Executables
package-id: com.apple.pkg.CLTools_Executables
version: 26.5.0.0.1777544298
volume: /
location: /
install-time: 1778955493
```

### Current

- 26.5 (May 11, 2026)

### Previous

- 16.4 (May 27, 2025)

## Navigation

- [Xcode Command Line Tools Install](./install/xcode-command-line-tools-install.md)
