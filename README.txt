OTA bundle 0.1.2

1) Upload ALL files from this folder to a free HTTPS host
   (GitHub Pages, Cloudflare Pages, Netlify…).
2) Make updates.json publicly readable.
3) Put the real URL of updates.json into .env as:
   VITE_OTA_MANIFEST_URL=https://YOUR_HOST/updates.json
4) Rebuild the base APK once (npm run cap:sync + assembleDebug)
   so the app knows where to ask for updates.
5) Later updates: only re-upload a new zip + updates.json
   (bump version). Clients get a prompt — no new APK.

checksum sha256: 6630b4f4e518d841968e604b90f95e582268512c368f4e979a56801fb7b1d909
zip: cozy-tag-0.1.2.zip
