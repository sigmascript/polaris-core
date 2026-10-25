# JavaScript

## Browser bundle

The production Webpack build exposes the default-exported Core class as the browser global `Polaris`.

```html
<script src="/assets/polaris/js/polaris.min.js"></script>
<script>
  const polaris = new Polaris();
  polaris.init();
</script>
```

Run this after the bundle is loaded and after the page's relevant markup exists. The public `init()` method in `src/ts/modules/Core.ts` enables configured blueprints and defaults, including optional backdrop, alert and modal blueprints, and configured interactions such as tabs and accordions.

## TypeScript source

`src/ts/polaris.ts` exports `Core` as the default `Polaris` class. Supporting modules live under `src/ts/modules/`:

- `Core.ts` — construction and initialization
- `Config.ts` — configuration
- `Defaults.ts` — default behaviors
- `Blueprints.ts` — blueprint generation
- `Components.ts` — interactive components
- `Animations.ts` — animation behavior
- `Helpers.ts` — helper methods

Use the generated declarations and current source signatures for method arguments. This overview intentionally does not reproduce unverified examples from the older manual.

## Important package-entry distinction

The root `index.js` returns a package version message when loaded through CommonJS. It is **not** a JavaScript UI API. For browser usage, load `dist/js/polaris.min.js` or integrate the TypeScript entry into your own build.
