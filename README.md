# NMBSE Workshop — Natural Materials and Biomimetics for Sustainable Engineering

A simple Hugo website for the workshop at Imperial College London, 17 June 2026.

## Features

- Lightweight Hugo site — **no external themes, no modules, no Sass**
- Plain CSS only
- Responsive design
- Ready for GitHub Pages deployment

## Local Development

### Prerequisites

- [Hugo](https://gohugo.io/installation/) (any recent version, extended or standard)

### Run locally

```bash
hugo server
```

Open [http://localhost:1313](http://localhost:1313) in your browser.

### Build

```bash
hugo --minify
```

Output goes to `./public/`.

## Deploy to GitHub Pages

### Option 1: GitHub Actions (Recommended)

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select **GitHub Actions**
4. The included `.github/workflows/hugo.yml` workflow will build and deploy automatically on every push to `main`

### Option 2: Manual Deploy

1. Build the site: `hugo --minify`
2. Push the contents of `./public/` to a `gh-pages` branch, or configure GitHub Pages to serve from the `docs/` folder

## Project Structure

```
.
├── content/
│   ├── _index.md          # Home page content
│   ├── speakers.md        # Speakers page
│   ├── registration.md    # Registration page
│   └── organisers.md      # Organisers page
├── layouts/
│   ├── _default/
│   │   ├── baseof.html    # Base template
│   │   └── single.html    # Single page template
│   ├── partials/
│   │   ├── head.html
│   │   ├── header.html
│   │   └── footer.html
│   └── index.html         # Home page template
├── static/
│   ├── css/style.css      # All styles (plain CSS)
│   └── images/banner.png  # Workshop banner
├── hugo.toml              # Hugo configuration
└── README.md
```

## Licence

Content © 2026 EENG / Imperial College London.
