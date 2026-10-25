# Concepts and naming

## Core and plugins

Core provides foundational styling, layout, forms, utilities and browser behavior. Optional plugins are separate projects with independent versions. Core documentation should not promise the presence of a plugin's classes or APIs.

## Polaris Naming Rules (PNR)

The historical Polaris manual describes four conventions:

| Concept | Typical shape | Purpose |
| --- | --- | --- |
| Component | `component` | Primary class |
| Modifier | `key-modifier` | Variant of a component |
| Child | `key--child` | Element associated with a component |
| Templating | `key_sibling`, `key__parent` | Sibling/parent relationships |

These are *conventions*, not a claim that every component uses every shape. For example, `.btn` is a component class. Always verify a particular class against the SCSS source or compiled CSS before using it.

## CSS and JavaScript

Many components are CSS-only. Interactive behavior is implemented in the TypeScript modules and compiled browser bundle. Include the JavaScript bundle and initialize `Polaris` when using interactive features.

## Responsive layouts

The historical manual describes responsive breakpoints and prefixed classes. Refer to the current Sass variables and layout sources for actual values; do not assume every 2023 example remains unchanged.
