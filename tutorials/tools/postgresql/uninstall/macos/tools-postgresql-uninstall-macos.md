[Tutorials](../../../../tutorials.md) > [Tools](../../../tools.md) > [PostgreSQL](../../tools-postgresql.md) > [Uninstall](../tools-postgresql-uninstall.md) > macOS

# Tools PostgreSQL Uninstall macOS

## Uninstall

```bash
brew services stop postgresql@18
brew uninstall postgresql@18
```

## Remove User Data

```bash
rm -rf /opt/homebrew/var/postgresql@18
```

## Check Location

```bash
test ! -e /opt/homebrew/opt/postgresql@18/bin/psql
```

should print nothing

```text
$ test ! -e /opt/homebrew/opt/postgresql@18/bin/psql
```
