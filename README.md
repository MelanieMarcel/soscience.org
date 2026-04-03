# soscience.org — farewell page

Static one-page site built with [Eleventy](https://www.11ty.dev/) (v3).

## Structure

```
soscience.org/
├── eleventy.config.js       # build config
├── package.json
├── SoScience - Color.png    # source logo (copied to _site/assets/logo.png)
├── src/
│   ├── index.njk            # page content
│   ├── _includes/
│   │   └── base.njk         # HTML shell
│   └── assets/
│       ├── style.css        # all styles
│       └── fonts/           # self-hosted Proxima Nova Alt (OTF)
└── _site/                   # built output — deploy this folder
```

## Setup

```bash
npm install
```

## Development

```bash
npm start        # build + local server at http://localhost:8080 with live reload
```

## Build

```bash
npm run build    # outputs to _site/
```

## Deploy

Upload the contents of `_site/` to any static host (Netlify, GitHub Pages, S3, etc.).

## Fonts

- **Roboto Condensed** — loaded from Google Fonts (body text)
- **Mrs Saint Delafield** — loaded from Google Fonts (signature)
- **Proxima Nova Alt Bold** — self-hosted OTF in `src/assets/fonts/` (labels, tagline)
