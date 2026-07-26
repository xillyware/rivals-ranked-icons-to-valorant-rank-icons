# Assets

This page documents the icon assets used by this project and provides a simple gallery and usage examples. Add your PNG files to the `assets/icons/` directory (one flat directory) and they will appear here.

## Where to put images

- Put all PNG images under `assets/icons/` in the repository root.
- Filenames should be lowercase, use hyphens for spaces, and include the rank name if applicable (example: `iron-1.png`, `bronze-3.png`).

## Gallery (example)

Below is a sample gallery table. Replace the placeholders and add rows that match your actual filenames. When you commit the PNGs to `assets/icons/`, the previews will render on GitHub.

| Rank | File | Preview |
|---|---:|:---|
| Iron I | `icons/iron-1.png` | ![iron-1](icons/iron-1.png)
| Bronze III | `icons/bronze-3.png` | ![bronze-3](icons/bronze-3.png)
| Placeholder | `icons/placeholder.png` | ![placeholder](icons/placeholder.png)


To add an entry use this Markdown row pattern:

`| Rank name | `icons/filename.png` | ![filename](icons/filename.png) |`

If you prefer an automatic gallery, we can add a small script that enumerates files and generates the Markdown table — tell me if you'd like that.

## Usage examples

HTML:

```html
<img src="/assets/icons/iron-1.png" alt="Iron I" width="64" height="64">
```

Markdown (in this repo):

```markdown
![Iron I](icons/iron-1.png)
```

CSS (to use as background):

```css
.rank-icon { width: 64px; height: 64px; background-size: contain; background-repeat: no-repeat; }
.rank-iron-1 { background-image: url('/assets/icons/iron-1.png'); }
```

React (JSX):

```jsx
import React from 'react';
import iron1 from '../assets/icons/iron-1.png';

export default function Icon(){
  return <img src={iron1} alt="Iron I" width={64} height={64} />;
}
```

## Filenames & variants

If you have multiple variants (color, outline, white-on-transparent), include them in the filename, e.g. `gold-1--white.png` or `gold-1--color.png` so they stay grouped.

## License & attribution

If these icons are derived from or licensed under a particular license, add a short note here with the license name and any attribution required. Example:

> Icons licensed under the CC BY 4.0 — please attribute "Author Name".

(If no special license applies, you can keep the repository license as the source of truth.)

## How I can help next

- I can add a script to auto-generate the gallery table from `assets/icons/`.
- I can also create an HTML page (`assets/index.html` or `docs/assets.html`) for a browsable gallery.

If you'd like me to also create one of those, tell me which and I'll add it.
