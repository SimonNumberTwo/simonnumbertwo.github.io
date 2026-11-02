# Tilla websites

The public pages for the Tilla iOS app, served with GitHub Pages from `main` (root):

| Page | Path | Used for |
| --- | --- | --- |
| Start | `index.html` | Marketing URL |
| Support | `support/index.html` | Support URL in App Store Connect |
| Privacy policy | `privacy/index.html` | Privacy policy URL in App Store Connect and TestFlight |

Each page is a standalone HTML file with all five app languages (de, en, es, fr, it). A small script
shows the language of the URL's hash (`support/#fr`) or else the browser's; without JavaScript every
language is shown. Light and dark mode follow the system.

The contact address appears as `TILLA_EMAIL` until it is set:

```sh
grep -rl TILLA_EMAIL --include=*.html . | xargs sed -i '' 's/TILLA_EMAIL/name@icloud.com/g'
```

`icon.png` and `apple-touch-icon.png` are the app icon (from the app repo's `AppIcon.png`).
