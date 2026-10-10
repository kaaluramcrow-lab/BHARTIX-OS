# BhartiX OS — Android app (Capacitor)

`www/index.html` is the whole BhartiX OS (all BhartiX programs).
GitHub builds the APK for you — no PC or Android Studio needed.

## Get the APK (phone is enough)
1. Make a free account on github.com and create a **new repository**.
2. Upload all files from this folder (use "Add file > Upload files"; the hidden `.github` folder must go too).
3. Open the **Actions** tab > **Build BhartiX OS APK** > **Run workflow**.
4. After ~5–8 minutes open the finished run > **Artifacts** > **BhartiX-OS-apk** (a zip) > extract `app-debug.apk`.
5. Install it on your phone (allow "Install unknown apps" for your browser / file manager).

## Update the app later
Replace `www/index.html` with the new BhartiX OS file and run the workflow again.

## Notes
* Files you save (Word, Excel, Paint, downloads) open Android's share sheet — choose "Save to device / Files / Drive".
* `window.print` does not exist in Android WebView, so use the PDF/Export commands inside the programs.
* For the Play Store you need a signed release (your own keystore) — the debug APK is for installing and testing.
