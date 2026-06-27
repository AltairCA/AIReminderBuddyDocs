# AIReminderBuddy Docs

Published site for [AIReminderBuddy](https://github.com/AltairCA/AIReminderBuddy), hosted on GitHub Pages for store listings and support.

## Live URLs (after GitHub Pages is enabled)

| Page | URL |
|------|-----|
| **Home** | `https://altairca.github.io/AIReminderBuddyDocs/` |
| **Privacy Policy** | `https://altairca.github.io/AIReminderBuddyDocs/privacy-policy.html` |

Use the **home URL** as the app website in Google Play Console. Use the **privacy policy URL** in the Data safety / Privacy policy field.

## Enable GitHub Pages

1. Open this repo on GitHub: **AltairCA/AIReminderBuddyDocs**
2. Go to **Settings → Pages**
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**
4. Choose branch **`main`**, folder **`/ (root)`**
5. Save — the site deploys in 1–3 minutes

## Site structure

```
AIReminderBuddyDocs/
├── index.html              ← Landing page
├── privacy-policy.html     ← Privacy policy (Play Console link)
├── privacy-policy.md       ← Source copy (keep in sync when editing policy)
├── styles.css
├── scripts/
│   └── capture-screenshot.sh  ← Capture Android screenshots via adb
├── assets/
│   ├── icon.png
│   ├── splash-icon.png
│   └── screenshots/        ← Real app screenshots for phone mockups
│       ├── home.png
│       ├── review-suggestions.png
│       ├── reminder-detail.png
│       ├── library.png
│       └── list-detail.png
└── .nojekyll               ← Serves static HTML as-is
```

## Updating content

- **Home page:** edit `index.html` and `styles.css`
- **Privacy policy:** edit `privacy-policy.md`, then mirror changes in `privacy-policy.html`
- **App icon:** replace `assets/icon.png` (copied from `apps/mobile/assets/images/icon.png`)

## Refreshing app screenshots

Phone mockups on the landing page use real captures from a connected Android device.

1. Connect one Android device with USB debugging enabled and open AIReminderBuddy on the screen you want.
2. From this repo root, run:

```bash
chmod +x scripts/capture-screenshot.sh   # first time only
./scripts/capture-screenshot.sh home.png
```

3. Repeat for each file under `assets/screenshots/`:

| File | Screen to show |
|------|----------------|
| `home.png` | Home tab with upcoming reminders |
| `review-suggestions.png` | Scanned object detail (AI labels + reminders) |
| `reminder-detail.png` | Reminder detail |
| `library.png` | Library tab, Scanned view |
| `list-detail.png` | List detail with checklist items |

**Deep links** (optional navigation aid):

```bash
adb shell am start -a android.intent.action.VIEW -d "aireminderbuddy://library" com.aireminderbuddy.app
adb shell am start -a android.intent.action.VIEW -d "aireminderbuddy://reminder/<id>" com.aireminderbuddy.app
adb shell am start -a android.intent.action.VIEW -d "aireminderbuddy://list/<id>" com.aireminderbuddy.app
adb shell am start -a android.intent.action.VIEW -d "aireminderbuddy://object/<id>" com.aireminderbuddy.app
```

Screenshots are full-device PNGs (1080×2340). The site scales them inside CSS phone frames.

## Google Play Console

| Field | Value |
|-------|-------|
| Website | `https://altairca.github.io/AIReminderBuddyDocs/` |
| Privacy policy | `https://altairca.github.io/AIReminderBuddyDocs/privacy-policy.html` |
| Contact email | altairserver@gmail.com |
