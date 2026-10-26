# Sci-Fi SFX Lab: deploy notes
Made by Zack Spakowski / Spaktacular Things.

Static site. Upload this folder as-is to any HTTPS static host (GitHub Pages, Netlify Drop, Cloudflare Pages, S3...).

Required: index.html, manifest.json, sw.js, icon-180.png, icon-192.png, icon-512.png, icon-maskable-512.png
Optional: examples/ (sample WAVs + params.json), README.md

- After changing index.html, bump VERSION in sw.js so installed copies update.
- index.html also works on its own (even from file://), without install or offline support.
- iPhone: open the HTTPS URL in Safari, then Share > Add to Home Screen.
- Library data lives in the browser's localStorage, so it is per device and per site address. Use Library > Export library to back it up.
