# Website Updates - Complete! ✓

## Changes Applied:

### 1. Home Page (index.markdown)
- ✅ Removed redundant "RAÚL FRANCISCO NAVAS" heading
- ✅ Removed "Inicio" page title
- ✅ Removed "HOME" section header
- ✅ Styled the two quotes elegantly:
  - Centered text
  - Larger font size (1.3em)
  - Italic style
  - No left border
  - Clean, professional appearance
- ✅ Kept specialties section
- ✅ Kept navigation section

### 2. Internal Files Excluded (_config.yml)
- ✅ CONTENT_GUIDE.md - Won't appear on site
- ✅ DEPLOYMENT.md - Won't appear on site
- ✅ THEME_FIX.md - Won't appear on site
- ✅ download-nighthawks.sh - Won't appear on site
- ✅ README.md - Won't appear on site

### 3. Background Image (assets/main.scss)
- ✅ Fixed CSS path to use Jekyll's relative_url
- ✅ Added stronger styling to ensure background displays
- ✅ Enhanced quote styling
- ✅ Hidden empty page heading

## To see all changes:

```bash
cd /Users/diego/Documents/raulnavas
bundle exec jekyll build --force
bundle exec jekyll serve
```

Then open: **http://localhost:4000**

## What you should see:

✅ **Home page:**
  - Clean layout without redundant titles
  - Two beautiful centered quotes in italic
  - Specialties section
  - Navigation links

✅ **Dark theme:**
  - Nighthawks painting as background
  - Dark overlay for readability
  - Light text on dark background

✅ **No internal docs:**
  - Guide files won't show in navigation or pages

## Deploy:

```bash
git add .
git commit -m "Clean up home page, add dark theme, exclude internal docs"
git push origin main
```

## Troubleshooting:

If background still doesn't show:
1. Hard refresh: Cmd+Shift+R (Mac) or Ctrl+Shift+R
2. Check browser console (F12) for errors
3. Verify image exists: `ls -lh assets/images/nighthawks.jpg`
4. Clear Jekyll cache: `rm -rf _site .jekyll-cache`
