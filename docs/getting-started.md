# Getting started

## Install

```bash
npm install polaris-core
```

For a traditional HTML site, copy the compiled CSS and JavaScript from the installed package's `dist/` directory into a directory served by your application. The exact public URLs depend on your application and build system.

## Minimal page

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Polaris</title>
  <link rel="stylesheet" href="/assets/polaris/css/polaris.min.css">
</head>
<body>
  <button class="btn">Example button</button>
  <script src="/assets/polaris/js/polaris.min.js"></script>
  <script>
    const polaris = new Polaris();
    polaris.init();
  </script>
</body>
</html>
```

The example assumes you copied the relevant distribution files into `/assets/polaris/`. The browser bundle exposes `Polaris`; calling `init()` activates its configured defaults and blueprints. Plain CSS components do not require initialization.

## Next steps

Learn [Polaris naming](concepts.md), browse [component categories](components/README.md), or read about [RTL](rtl-and-themes.md).
