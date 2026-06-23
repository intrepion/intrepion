[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [SpaceTimeDB](../../../code-spacetimedb.md) > [Solutions](../../code-spacetimedb-solutions.md) > [Hello World](../code-spacetimedb-solutions-hello-world.md) > Library

# Code SpaceTimeDB Solutions Hello World Library

## Library

```bash
touch spacetimedb/src/lib.rs
printf '%s\n' \
  'use spacetimedb::{ReducerContext, Table};' \
  '' \
  '#[spacetimedb::table(accessor = person, public)]' \
  'pub struct Person {' \
  '    name: String,' \
  '}' \
  '' \
  '#[spacetimedb::reducer]' \
  'pub fn add(ctx: &ReducerContext, name: String) {' \
  '    ctx.db.person().insert(Person { name });' \
  '}' \
  '' \
  '#[spacetimedb::reducer]' \
  'pub fn say_hello(ctx: &ReducerContext) {' \
  '    for person in ctx.db.person().iter() {' \
  '        log::info!("Hello, {}!", person.name);' \
  '    }' \
  '' \
  '    log::info!("Hello, world!");' \
  '}' \
  | tee spacetimedb/src/lib.rs > /dev/null
```
