# UNAWAIN — GitHub Pages Site

This directory contains the static HTML files for the UNAWAIN support website.

**Live URLs (after deployment):**
- Landing: https://ralph-mattew.github.io/unawain-app/
- Privacy: https://ralph-mattew.github.io/unawain-app/privacy
- Support: https://ralph-mattew.github.io/unawain-app/support
- Terms:   https://ralph-mattew.github.io/unawain-app/terms

## How to Deploy

### Option A: New Repository (Recommended)

1. Create a new GitHub repo named `unawain-app`:
   ```bash
   # From this site/ directory:
   cd docs/site
   git init
   git add .
   git commit -m "UNAWAIN support site — privacy, terms, support pages"
   git branch -M main
   git remote add origin https://github.com/ralph-mattew/unawain-app.git
   git push -u origin main
   ```

2. Enable GitHub Pages:
   - Go to https://github.com/ralph-mattew/unawain-app/settings/pages
   - Source: Deploy from a branch
   - Branch: `main`, folder: `/ (root)`
   - Click Save

3. Wait 1-2 minutes, then verify all URLs are live.

### Option B: GitHub Pages from Existing Repo

1. Copy the site/ files to a `docs/` folder in the main unawain repo
2. Enable GitHub Pages from `docs/` folder on `main` branch
3. Note: The URL would be `ralph-mattew.github.io/unawain/` not `/unawain-app/`
   — you'd need to update all URL references in APP_STORE_METADATA.md and APPLE_REVIEW_CHECKLIST.md

## File Structure

```
site/
  index.html          — Landing page
  privacy/index.html  — Privacy Policy
  support/index.html  — Support & FAQ & Troubleshooting
  terms/index.html    — Terms of Use
```

## Design

The site uses UNAWAIN's brand colors (teal, gold, cream, narra brown) and is fully responsive. No JavaScript, no frameworks, no external dependencies — just clean HTML/CSS that loads instantly.
