# Cozy Tag OTA (GitHub Pages)

Free update channel for the Android app.

Public manifest:

`https://vadoimichi83.github.io/cozytag-ota/updates.json`

## Enable GitHub Pages (one-time)

1. Create empty repo **cozytag-ota** under account **vadoimichi83** (if it does not exist yet).
2. Push this folder to `main`.
3. On GitHub: **Settings → Pages → Branch: `main` / folder: `/ (root)` → Save**.
4. Wait 1–2 minutes, open the manifest URL above.

## Publish a new update later

From the app folder:

```powershell
$env:OTA_PUBLIC_BASE="https://vadoimichi83.github.io/cozytag-ota"
npm run ota:pack -- 0.1.1 "What changed"
Copy-Item .\ota-release\* ..\..\cozytag-ota\ -Force
# then commit + push cozytag-ota
```
