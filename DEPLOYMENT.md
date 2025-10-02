# Deployment Notes

## Dark Theme Applied ✓

The website now has a dark/night mode theme with the Nighthawks painting as background.

### Files Created/Modified:

1. **`assets/css/style.scss`** - Custom dark theme CSS
   - Dark background (#1a1a1a)
   - Light text (#e0e0e0)
   - Nighthawks painting as fixed background
   - Semi-transparent overlay for readability
   - Dark header and footer
   - Adjusted link colors for dark theme
   - Responsive design maintained

2. **`assets/images/nighthawks.jpg`** - Background image (8.1 MB)
   - Downloaded from Wikimedia Commons (public domain)
   - High resolution version of Edward Hopper's famous painting

## Testing Locally

If you have issues with bundle/Jekyll, try:

```bash
# Option 1: Using Docker (recommended)
docker run --rm -v "$PWD":/srv/jekyll -p 4000:4000 jekyll/jekyll jekyll serve --watch

# Option 2: Fix bundle issues
rm Gemfile.lock
bundle install
bundle exec jekyll serve

# Option 3: Use Ruby version manager
# Install rbenv or rvm, then:
rbenv install 3.0.0
rbenv local 3.0.0
bundle install
bundle exec jekyll serve
```

Then open: http://localhost:4000

## Deployment to GitHub Pages

The CSS and images will be automatically deployed when you push to GitHub:

```bash
git add .
git commit -m "Add dark theme with Nighthawks background"
git push origin main
```

GitHub Pages will build and deploy the site with the new theme at raulnavas.com.ar (once DNS is configured).

## Theme Features

- **Dark background**: Easier on the eyes, professional look
- **Nighthawks painting**: Iconic artwork creates sophisticated atmosphere
- **Readable text**: White/light gray text on dark background
- **Overlay**: Semi-transparent dark overlay ensures text readability
- **Consistent styling**: All pages use the same dark theme
- **Mobile responsive**: Works well on all screen sizes

## Customization

To adjust the theme, edit `assets/css/style.scss`:

- Change overlay opacity: `background-color: rgba(0, 0, 0, 0.7);` (last number is opacity)
- Change text color: `color: #e0e0e0;`
- Change background color: `background-color: #1a1a1a;`
- Adjust link colors: `a { color: #7eb8e5; }`

## Notes

- The Nighthawks painting is in the public domain
- Image is optimized for web but you can replace it with a smaller version if needed
- The theme overrides the default Minima theme while maintaining compatibility
