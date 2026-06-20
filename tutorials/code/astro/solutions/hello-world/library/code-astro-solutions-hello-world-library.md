[Tutorials](../../../../../tutorials.md) > [Code](../../../../code.md) > [Astro](../../../code-astro.md) > [Solutions](../../code-astro-solutions.md) > [Hello World](../code-astro-solutions-hello-world.md) > Library

# Code Astro Solutions Hello World Library

## Library

```bash
mkdir -p src/components
touch src/components/HelloWorld.astro
printf '%s\n' \
  '---' \
  'const message = "Hello, world!";' \
  '---' \
  '' \
  '<p>{message}</p>' \
  | tee src/components/HelloWorld.astro > /dev/null
```
