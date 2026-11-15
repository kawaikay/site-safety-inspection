SITE SAFETY INSPECTION PWA

FILES
- index.html: mobile application shell
- app.js: checklist, IndexedDB photos/reports, offline PDF preview
- styles.css: responsive mobile and print layout
- sw.js: offline application cache
- manifest.webmanifest: installable PWA configuration
- icons/: installation icons

DEPLOYMENT
1. Upload the entire folder to an HTTPS web host, preserving the folder structure.
2. Open index.html in Safari or Chrome once while online.
3. iPhone/iPad: Share > Add to Home Screen.
4. Android: Chrome menu > Install app or Add to Home screen.
5. Open the installed app once, then it operates offline.

IMPORTANT
- Do not open index.html directly as a file:// URL. Service workers and camera access require HTTPS (or localhost for testing).
- Photos and reports are stored only in that browser profile using IndexedDB.
- Clearing browser/site data deletes locally stored reports and photos.
- Use Save Inspection regularly.

OFFLINE PDF
- Tap Offline PDF.
- The app builds the bilingual report from selected PASS/FAIL/N/A items only.
- Unselected items and empty categories are omitted.
- iPhone/iPad: in the print preview, pinch outward to open the PDF, then Share > Save to Files.
- Android/Chrome: choose Save as PDF in the print destination.
- PDF creation uses the browser print engine and works offline; no external PDF library or server is required.
