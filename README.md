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
├── assets/
│   ├── icon.png
│   └── splash-icon.png
└── .nojekyll               ← Serves static HTML as-is
```

## Updating content

- **Home page:** edit `index.html` and `styles.css`
- **Privacy policy:** edit `privacy-policy.md`, then mirror changes in `privacy-policy.html`
- **App icon:** replace `assets/icon.png` (copied from `apps/mobile/assets/images/icon.png`)

## Google Play Console

| Field | Value |
|-------|-------|
| Website | `https://altairca.github.io/AIReminderBuddyDocs/` |
| Privacy policy | `https://altairca.github.io/AIReminderBuddyDocs/privacy-policy.html` |
| Contact email | altairserver@gmail.com |
