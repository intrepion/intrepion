[Tutorials](../../../../../../tutorials.md) > [Code](../../../../../code.md) > [Astro](../../../../code-astro.md) > [Solutions](../../../code-astro-solutions.md) > [Hello World](../../code-astro-solutions-hello-world.md) > [Adapters](../code-astro-solutions-hello-world-adapters.md) > Web

# Code Astro Solutions Hello World Adapters Web

## Requirements

- [Tools nvm Install macOS](../../../../../../tools/nvm/install/macos/tools-nvm-install-macos.md)

## Code

### Create application

```bash
npm create astro@latest web -- --template minimal --install --no-git --yes --skip-houston
cd web
npm install --save-dev prettier prettier-plugin-astro
```

### Add .gitignore snippet

- [Code Astro Snippets .gitignore](../../../../snippets/gitignore/code-astro-snippets-gitignore.md)

### Add Hello World library

- [Code Astro Solutions Hello World Library](../../library/code-astro-solutions-hello-world-library.md)

### Add web page

```bash
mkdir -p src/pages
touch src/pages/index.astro
printf '%s\n' \
  '---' \
  'import HelloWorld from "../components/HelloWorld.astro";' \
  '---' \
  '' \
  '<html lang="en">' \
  '  <head>' \
  '    <meta charset="utf-8" />' \
  '    <meta name="viewport" content="width=device-width" />' \
  '    <title>Hello World</title>' \
  '  </head>' \
  '  <body>' \
  '    <main>' \
  '      <HelloWorld />' \
  '    </main>' \
  '  </body>' \
  '</html>' \
  | tee src/pages/index.astro > /dev/null
```

### Check if builds

```bash
npm run build
```

### Check formatting

```bash
npx prettier --check .
```

### Correct formatting

```bash
npx prettier --write .
```

### Build for production

```bash
npm run build
```

### Run locally

```bash
npm run dev
```
