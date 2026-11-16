# MichaelJHla.github.io

Public website for MichaelJHla's apps, served by GitHub Pages at <https://michaeljhla.github.io/>.

| URL | File | Used for |
| --- | --- | --- |
| `/` | `index.html` | Developer home page: the App Store "developer website" |
| `/party-pose/` | `party-pose/index.html` | Party Pose page: App Store Connect **Marketing URL** (optional) |
| `/party-pose/privacy/` | `party-pose/privacy/index.html` | App Store Connect **Privacy Policy URL** |
| `/party-pose/support/` | `party-pose/support/index.html` | App Store Connect **Support URL** |
| `/app-ads.txt` | `app-ads.txt` | AdMob authorized-seller file (must stay at the site root) |

Plain HTML and CSS (`assets/style.css`) with no build step. `.nojekyll` tells GitHub Pages to serve the files as they are.

## Publishing

Settings → Pages → Build and deployment → **Deploy from a branch**, branch `main`, folder `/ (root)`. Changes go live a minute or two after they're pushed to `main`.

## Updating

- **Privacy policy:** if the app starts collecting anything new, update `party-pose/privacy/index.html` and its "Effective" date. It must match the App Privacy answers in App Store Connect.
- **app-ads.txt:** if AdMob shows a different line under Apps → app-ads.txt, replace the contents with it.
- **Icons:** `party-pose/icon.png`, `apple-touch-icon.png` and `favicon.png` are resized from the app's icon (`DuoPose/Assets.xcassets/AppIcon.appiconset/AppIcon.png` in the app repo).
