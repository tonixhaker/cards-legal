# Kodnyk — legal pages (GitHub Pages)

Static site with the privacy policy and terms of use (EN + UA).

GitHub Pages on the **free plan only publishes from public repos**, so this
folder is designed to be pushed to a small public repo while the app repos
stay private:

```bash
# one-time
gh repo create tonixhaker/cards-legal --public   # or create via the web UI
cd legal
git init -b main
git add .
git commit -m "Kodnyk legal pages"
git remote add origin git@github.com:tonixhaker/cards-legal.git
git push -u origin main
```

Then on GitHub: **cards-legal → Settings → Pages → Source: Deploy from a
branch → main / (root) → Save.**

The site appears at:

- https://tonixhaker.github.io/cards-legal/          (landing)
- https://tonixhaker.github.io/cards-legal/privacy.html
- https://tonixhaker.github.io/cards-legal/terms.html

Use those URLs in App Store Connect / Play Console listings and in the
Firebase project settings.
