========================================
  SAI KRUSHNA STONE SUPPLIERS - PWA SETUP
========================================

FILES INCLUDED:
  ✅ index.html     → Updated with PWA support
  ✅ manifest.json  → App name, icon, theme settings
  ✅ sw.js          → Service worker (offline support)
  ✅ README.txt     → This file

---

STEPS TO SET UP:

1. COPY these 3 files into your website folder:
   → index.html  (replace your old one)
   → manifest.json
   → sw.js

2. CREATE an "icons" folder in your website folder
   Add these icon sizes (PNG format):
   → icon-72x72.png
   → icon-96x96.png
   → icon-128x128.png
   → icon-144x144.png
   → icon-152x152.png
   → icon-192x192.png  ← most important
   → icon-384x384.png
   → icon-512x512.png  ← most important

   💡 FREE TOOL to generate all sizes:
      https://realfavicongenerator.net
      Just upload one 512x512 logo image → download all sizes

3. HOST on HTTPS (required for PWA):
   Free options:
   → GitHub Pages  (github.com/pages)
   → Netlify       (netlify.com)
   → Vercel        (vercel.com)

4. DONE! Open site on Android Chrome → browser will show
   "Add to Home Screen" or your yellow install banner 📲

---

ALSO UPDATE sw.js if you have more pages/images:
  const ASSETS_TO_CACHE = [
    '/index.html',
    '/materials.html',   ← add your pages
    '/gallery.html',
    '/your-image.jpg',   ← add your images
    ...
  ];

---

TESTING:
  Open Chrome DevTools → Application → Service Workers
  Check: "Manifest" and "Service Workers" are both ✅ green

========================================
