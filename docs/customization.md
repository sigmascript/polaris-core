# Customization

Polaris Core maintains its styles in Sass and its interactive behavior in TypeScript.

## Source map

- `src/scss/polaris.scss` — standard Sass entry point
- `src/scss/polaris-rtl.scss` — RTL Sass entry point
- `src/scss/_variables/` and `src/scss/_mixins/` — configuration and shared building blocks
- `src/scss/` category directories — components and utilities
- `src/ts/polaris.ts` — TypeScript entry point
- `src/ts/modules/` — framework classes and behavior

## Build

From a clean clone:

```bash
npm ci
npm run css
npm run css-rtl
npm run js
npx tsc --project tsconfig.json
```

`css` and `css-rtl` build compressed stylesheets. `js` creates the bundled browser JavaScript. TypeScript compilation also generates modular output and declarations according to `tsconfig.json`.

## Customization guidance

Prefer configuring a copy or a consuming project's build instead of editing installed files under `node_modules/`. If you change Sass naming or component configuration, verify corresponding JavaScript selectors/configuration before shipping. Keep CSS and JavaScript builds compatible.

For local watch commands, see [development](development.md).
