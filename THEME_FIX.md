# Dark Theme Fix - Applied! ✓

## What was fixed:

The custom dark theme CSS is now properly configured. The issue was that Jekyll's Minima theme uses `/assets/main.scss` as the main stylesheet, not `/assets/css/style.scss`.

## Files created/updated:

1. **`/assets/main.scss`** - Main stylesheet with dark theme (CORRECT location)
   - Imports Minima base styles
   - Adds dark background (#1a1a1a)
   - Sets Nighthawks painting as background image
   - Creates semi-transparent overlay for readability
   - Styles all elements for dark mode

2. **`/assets/css/style.scss`** - (This file exists but isn't used by Minima)

## To see the changes:

You need to rebuild the Jekyll site. Choose one of these options:

### Option 1: Clean rebuild (Recommended)
```bash
cd /Users/diego/Documents/raulnavas
rm -rf _site .jekyll-cache
bundle exec jekyll build
bundle exec jekyll serve
```

### Option 2: Force rebuild
```bash
cd /Users/diego/Documents/raulnavas
bundle exec jekyll build --force
bundle exec jekyll serve
```

### Option 3: Use Docker (if bundle issues persist)
```bash
cd /Users/diego/Documents/raulnavas
docker run --rm -v "$PWD":/srv/jekyll -p 4000:4000 jekyll/jekyll jekyll serve --watch --force_polling
```

Then open: **http://localhost:4000**

## What you should see:

✅ Dark background (near black - #1a1a1a)
✅ Nighthawks painting visible behind content
✅ Semi-transparent dark overlay making text readable
✅ White/light text on dark background
✅ Blue-ish links (#7eb8e5)
✅ Dark header and footer

## Troubleshooting:

If you still see a white background:
1. **Hard refresh** your browser: Cmd+Shift+R (Mac) or Ctrl+Shift+R (Windows)
2. **Clear browser cache**
3. Check browser console (F12) for any CSS loading errors
4. Verify `/assets/images/nighthawks.jpg` exists (8.1 MB file)

## Deploy to GitHub Pages:

Once it looks good locally:
```bash
git add .
git commit -m "Apply dark theme with Nighthawks background"
git push origin main
```

GitHub Pages will automatically rebuild with the new theme!
