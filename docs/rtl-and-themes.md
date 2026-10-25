# RTL and color schemes

## Right-to-left styles

Polaris provides a dedicated RTL stylesheet at `dist/css/polaris-rtl.min.css`. Use it **instead of** the regular `polaris.min.css` for RTL pages unless your own build intentionally combines them.

```html
<html lang="ar" dir="rtl">
<head>
  <link rel="stylesheet" href="/assets/polaris/css/polaris-rtl.min.css">
</head>
```

This assumes the stylesheet was copied into the application's public assets. Verify actual direction-specific component behavior in your application.

## Light and dark

The original manual describes light/dark schemes and component-level colors. Current implementation details live in the Sass variables, appearance and basics sources, and JavaScript defaults. Do not assume that every legacy scheme or automatic behavior works identically without testing the specific component.

## Validation

Build both variants with `npm run css` and `npm run css-rtl`. Check representative components in both LTR and RTL pages, including interactive components where JavaScript is involved.
