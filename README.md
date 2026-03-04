# saproot-theme

Shared CSS design system for all [saproot.org](https://saproot.org) properties.

Used as a **Git submodule** in:
- [`reading-class-site`](https://github.com/joel/reading-class-site) — Gatsby static site at `reading.saproot.org`
- [`english-class-app`](https://github.com/joel/english-class-app) — Flask writing tool at `writing.saproot.org`

---

## Files

| File | Purpose |
|---|---|
| `tokens.css` | CSS variables: colors, fonts, spacing, radii |
| `components.css` | Base reset, layout, header, buttons, forms, cards |

---

## Usage

### In Gatsby (JavaScript import)
```js
// src/components/layout.js or layout.css
import "../../saproot-theme/tokens.css";
import "../../saproot-theme/components.css";
```

### In Flask (CSS import)
```css
/* app/static/style.css */
@import url('../saproot-theme/tokens.css');
@import url('../saproot-theme/components.css');
/* App-specific styles below */
```

---

## Contributing

1. Edit design tokens in `tokens.css` or shared components in `components.css`.
2. Commit and push to this repo.
3. In each consumer repo: `git submodule update --remote`
