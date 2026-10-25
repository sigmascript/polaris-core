# Development and verification

## Requirements

Use Node.js and npm compatible with the project's pinned build dependencies. Development dependencies are defined in `package.json` and locked in `package-lock.json`.

```bash
npm ci
npm run css
npm run css-rtl
npm run js
npx tsc --project tsconfig.json
npm audit
npm audit --omit=dev
npm pack --dry-run
```

The current `npm test` script is a placeholder that exits with an error; it is **not** a working test suite. Do not report it as a passing test.

## Development commands

- `npm run css-dev` — watch standard Sass
- `npm run css-rtl-dev` — watch RTL Sass
- `npm run js-dev` — development Webpack build
- `npm run js-mod` — watch modular TypeScript compilation

Watch commands run until stopped; they are not release checks.

## Release discipline

Keep compatibility and generated assets under review. Verify both stylesheets, browser bundle, declarations, security audit, and package contents before tagging. Update [the release index](../CHANGELOG.md) and version-specific changelog. Do not tag or publish until the release is approved.
