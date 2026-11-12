# jltorresgit.github.io

Public space for the applications I've created: one page per app, plus its privacy policy.

Live site: <https://jltorresgit.github.io/>

## How it's built

GitHub Pages builds the **`docs/`** folder of `main` with Jekyll (Settings › Pages › *Deploy from a branch* ›
`main` / `/docs`). No theme gem, no build step, no GitHub Actions: just push.

```
docs/
├── _config.yml            Site title, author, contact links
├── _apps/                 ONE FILE PER APP: the app page (front matter + description)
│   ├── GasControl.md          → /GasControl/
│   ├── AccountsManager.md     → /AccountsManager/
│   └── Rota.md                → /Rota/
├── GasControl/privacy/index.md       → /GasControl/privacy/   (privacy policy)
├── AccountsManager/privacy/index.md  → /AccountsManager/privacy/
├── Rota/privacy/index.md             → /Rota/privacy/
├── index.html             Home page: lists every app in _apps/, sorted by `order`
├── 404.html
├── _layouts/              default · app · privacy
├── _includes/             header, footer, app card, app icon
└── assets/
    ├── css/style.css      All styling (light and dark mode)
    ├── img/favicon.svg
    └── apps/<Slug>/       Icons and screenshots for each app
templates/                 Not published. Copy these to add an app
├── app.md
└── privacy.md
```

## Add a new app

1. Pick a slug with no spaces, e.g. `MyApp`. It becomes the URL, so keep it once published.
2. Copy `templates/app.md` to `docs/_apps/MyApp.md` and fill it in.
3. Copy `templates/privacy.md` to `docs/MyApp/privacy/index.md` and write the policy.
4. Optional: put `icon.png` (512×512) and screenshots in `docs/assets/apps/MyApp/` and reference them in step 2.
5. Commit and push. The app appears on the home page within a minute or two.

The privacy policy URL to give Google Play Console is `https://jltorresgit.github.io/MyApp/privacy/`.

## Preview locally (optional)

Requires Ruby. From `docs/`:

```
gem install jekyll jekyll-seo-tag jekyll-sitemap
jekyll serve
```

Then open <http://localhost:4000>.
