# Component reference

Polaris Core groups Sass sources by purpose. This index is a **verified source inventory**, not a claim that every component already has a complete usage guide.

| Category | Source directory | Examples of source files |
| --- | --- | --- |
| Basics | `src/scss/basics/` | Base framework styles |
| Typography | `src/scss/typography/` | Links, lists, images, tables, code |
| Layout | `src/scss/layout/` | Grid, containers, flexbox, visibility |
| Appearance | `src/scss/appearance/` | Colors, backgrounds, shadows, radius |
| Effects | `src/scss/effects/` | Animation, transitions, ripple |
| Forms | `src/scss/forms/` | Fields, switches, validation, ranges |
| Utilities | `src/scss/utilities/` | Buttons, alerts, modals, tabs, accordions |

Component class names, modifiers and required markup should be taken from the corresponding SCSS source. Interactive components may additionally depend on `src/ts/modules/Components.ts`, `Defaults.ts`, or `Blueprints.ts`.

## Documentation roadmap

Expand this index with source-verified examples for buttons, grids, fields, alerts, modals, tabs and accordions. Keep examples compatible with both the default and RTL builds where applicable. The 2023 PDF is useful for identifying missing topics, but not as an unquestioned API reference.
