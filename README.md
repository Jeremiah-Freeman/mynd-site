# mynd-site — privacy / terms / support pages

A tiny static site for the App Store-required public URLs.

## Publish on GitHub Pages (free, ~3 minutes)

1. Create a new GitHub repo (suggested name: `mynd-site`) — make it **Public**.
2. From your Mac, in the project:
   ```bash
   cd ~/Developer/mynd/site
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/mynd-site.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save.**
4. Wait ~1 minute. Your URLs are now live at:
   - `https://<your-username>.github.io/mynd-site/` → landing
   - `https://<your-username>.github.io/mynd-site/privacy.html` → Privacy Policy
   - `https://<your-username>.github.io/mynd-site/terms.html` → Terms
   - `https://<your-username>.github.io/mynd-site/support.html` → Support

Paste those three URLs into `docs/APP_STORE_LISTING.md` (replacing `[YOUR_HOST]`) and into App Store Connect when you fill the listing.

## What's here

- `index.html` — minimal landing page
- `privacy.html` — Privacy Policy (matches `docs/PRIVACY_POLICY.md`, no draft callout)
- `terms.html` — Terms of Service (matches `docs/TERMS.md`)
- `support.html` — Support page + tiny FAQ (App Store requires a working Support URL)
- `style.css` — shared styling
