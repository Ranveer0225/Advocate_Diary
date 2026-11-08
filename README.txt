ADVOCATE DIARY — WEB VERSION (INITIAL WORKING BUILD)

FILES
- index.html: application interface and functionality
- manifest.webmanifest: installable web-app metadata
- sw.js: offline app-shell cache

HOW TO RUN
1. Extract the ZIP.
2. Upload the contents of this folder to a static website host (for example, GitHub Pages, Netlify, or another HTTPS host).
3. Open the hosted index.html URL in Chrome on Android.
4. In Chrome, use the browser menu > Add to Home screen / Install app.

You can also open index.html directly for basic local testing. Offline installation and service-worker caching require an HTTPS website (or localhost).

CURRENT FEATURES
- Daily Referencer is the first screen.
- Daily date selector, notes/reminders, matter list, previous/next day navigation.
- Customisable diary columns: add, rename, remove and reorder.
- Case register with CNR, court, parties, dates, stage, status, priority and client links.
- Hearing history and proceedings; updating a hearing moves the case to the new next date.
- Cases without a next date remain visible on the hearing date; daily closing warns and preserves unresolved matters.
- Client register, multiple linked clients per case, and optional additional contact persons.
- Quick Orders section in each case: record order details and official source URL; open official eCourts portal.
- Calendar, reminders, CSV export of daily list, JSON backup/restore.
- Mobile responsive layout and basic offline app-shell support.

IMPORTANT LIMITATIONS — READ BEFORE USING REAL CLIENT DATA
This is a functional browser-based first build, not yet a production multi-user legal case management service. Records are stored in local browser storage on this device. Clearing browser data, changing browser/device, or some private-browsing modes can remove or isolate records. Download backups regularly and store them securely.

There is currently no cloud database, server-side account/login, multi-device synchronisation, server-side encryption, or direct eCourts API integration. Do not treat the app as a secure cloud repository for confidential client material yet. The Quick Orders module stores order metadata and a URL; a selected PDF is not uploaded into secure storage in this build. eCourts search/import is assisted: it opens the official portal, and the user must complete CAPTCHA and verify/copy information. The app does not bypass CAPTCHA, scrape restricted content, or claim automatic live sync.

NEXT PRODUCTION STEPS
- Add secure backend database, authentication and access controls.
- Add encrypted file storage and secure document upload.
- Implement verified eCourts-assisted import workflow and duplicate checking.
- Add robust offline synchronisation and conflict handling.
- Test on target Android browsers and deploy to a production HTTPS domain.
