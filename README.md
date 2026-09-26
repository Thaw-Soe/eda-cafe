# Eda's Cafe - GitHub Pages Deployment

Static HTML version of the cafe website.

## Deploying to GitHub Pages

1. Create repository: `github.com/thawsoe7/eda-cafe`
2. Push files to `main` branch
3. Enable GitHub Pages in Settings → Pages → Source: `main` branch → `/ (root)`

## Custom Domain

To point `eda-cafe.co.uk` to this GitHub Pages site:
- Add CNAME record: `www` → `thawsoe7.github.io`
- Add A records for apex domain:
  ```
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
  ```

## Files

- `index.html` - Main site
- `404.html` - SPA fallback for client-side routing
- `assets/` - Images and static assets
- `favicon.svg` - Site icon
- `robots.txt` - Search engine permissions

## Testing Locally

```bash
cd ~/Documents/eda-cafe-deploy
python3 -m http.server 3000
# Visit http://localhost:3000
```