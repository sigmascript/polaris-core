# Polaris UI — Core

Polaris Core is an open-source front-end framework for building responsive web interfaces with HTML, CSS and JavaScript. It provides reusable styles, components and optional JavaScript behavior, with a focus on simplicity and customization.

**Core** contains the shared foundation. **Plugins** add independently maintained features and are versioned separately.

## Get started

Install the package:

```bash
npm install polaris-core
```

For a plain HTML project, copy the compiled files you need from `node_modules/polaris-core/dist/` into your application's public assets. Reference those *served* asset paths (not the package directory directly):

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Polaris example</title>
  <link rel="stylesheet" href="/assets/polaris/css/polaris.min.css">
</head>
<body>
  <button class="btn">Hello Polaris</button>
  <script src="/assets/polaris/js/polaris.min.js"></script>
  <script>
    const polaris = new Polaris();
    polaris.init();
  </script>
</body>
</html>
```

The example assumes you copied `dist/css/polaris.min.css` and `dist/js/polaris.min.js` to the paths shown. Copy any referenced font or image assets as needed. JavaScript initialization is needed for interactive features, not for basic CSS styling.

For right-to-left layouts, use `polaris-rtl.min.css` **instead of** the standard CSS build; see [RTL and themes](docs/rtl-and-themes.md).

## Documentation

Start with the [documentation index](docs/README.md), then explore [components](docs/components/README.md), [customization](docs/customization.md), and the [JavaScript guide](docs/javascript.md).

## Develop from source

```bash
git clone https://github.com/sigmascript/polaris-core.git
cd polaris-core
npm ci
npm run css
npm run css-rtl
npm run js
npx tsc --project tsconfig.json
```

See [development and verification](docs/development.md) for build details. The root `index.js` is a package/version message; it is **not** the browser `Polaris` constructor. Use the browser distribution or the TypeScript sources for UI behavior.

## Releases and links

- [Release history](CHANGELOG.md) · [Detailed changelogs](changelog/)
- [GitHub repository](https://github.com/sigmascript/polaris-core)
- [Issue tracker](https://github.com/sigmascript/polaris-core/issues)
- [Polaris website](https://polarisui.com/)

Licensed under the [MIT License](LICENSE).
