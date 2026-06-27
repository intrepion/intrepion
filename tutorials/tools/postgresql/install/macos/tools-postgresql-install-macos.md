[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [PostgreSQL](../../tools-postgresql.md) > [Install](../tools-postgresql-install.md) > macOS

# Tools PostgreSQL Install macOS

## Requirements

- [Homebrew](../../../homebrew/install/macos/tools-homebrew-install-macos.md)

## Install

```bash
brew install postgresql@18
brew services start postgresql@18
```

## Update

```bash
brew upgrade postgresql@18
brew services restart postgresql@18
```

## Check Location

```bash
ls /opt/homebrew/opt/postgresql@18/bin/psql
```

should be something like

```text
$ ls /opt/homebrew/opt/postgresql@18/bin/psql
/opt/homebrew/opt/postgresql@18/bin/psql
```

## Check Service

```bash
brew services list
```

## Connect

```bash
/opt/homebrew/opt/postgresql@18/bin/psql postgres
```
