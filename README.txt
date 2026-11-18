OTA bundle 0.1.4

1) Upload ALL files from this folder to a free HTTPS host
   (GitHub Pages, Cloudflare Pages, Netlify…).
2) Make updates.json publicly readable.
3) Put the real URL of updates.json into .env as:
   VITE_OTA_MANIFEST_URL=https://YOUR_HOST/updates.json
4) Rebuild the base APK once (npm run cap:sync + assembleDebug)
   so the app knows where to ask for updates.
5) Later updates: only re-upload a new zip + updates.json
   (bump version). Clients get a prompt — no new APK.

checksum sha256: 0854630ffcf9144bc458f858e131303bf58b14927c9268f8d9b7e3beba952d50
zip: cozy-tag-0.1.4.zip
