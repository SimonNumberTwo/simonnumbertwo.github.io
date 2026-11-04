# simonnumbertwo.github.io

Simon Blum's website: who I am and my apps, served with GitHub Pages from `main` (root) at
https://simonnumbertwo.github.io/.

| Page | Path | Used for |
| --- | --- | --- |
| About me and my apps | `index.html` | |
| Privacy of this website | `privacy/index.html` | |
| Tilla | `tilla/index.html` | Marketing URL in App Store Connect |
| Tilla support | `tilla/support/index.html` | Support URL in App Store Connect |
| Tilla privacy policy | `tilla/privacy/index.html` | Privacy policy URL in App Store Connect and TestFlight |
| Tilla Apple Pay shortcut | `tilla/shortcut/index.html` | The app's "Kurzbefehl hinzufügen" (`tilla/shortcut/?go` forwards to the iCloud link) |

A new app gets its own folder like `tilla/` (start, `support/`, `privacy/`, its icon), a card on the
start page and a link in the website's privacy page.

Each page is a standalone HTML file with all five languages (de, en, es, fr, it). A small script shows
the language of the URL's hash (`tilla/support/#fr`) or else the browser's; without JavaScript every
language is shown. Light and dark mode follow the system. No cookies, analytics or external resources.

The shortcut page's "Kurzbefehl hinzufügen" buttons (all five, `a.shortcut`) carry the iCloud link of the shared
shortcut "Tilla - Apple Pay"; opened with `?go` (as the app does) the page forwards to it at once. A newly shared
shortcut only needs a new link there – no app update.

Contact address: `simonblum.apps@icloud.com` (an iCloud alias). `tilla/icon.png` and
`tilla/apple-touch-icon.png` are the app icon (from the app repo's `AppIcon.png`); `tilla/screens/<lang>/` are the raw app screens (`fastlane/store_frames/raw`, 600 px JPEG) that Tilla's page shows in drawn iPhone frames.
