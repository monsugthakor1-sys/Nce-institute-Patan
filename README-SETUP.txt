NCE INSTITUTE PATAN WEBSITE PACKAGE

FILES
- index.html: main bilingual futuristic website, course links, online image gallery, admission inquiry, demo student portal, demo certificate verification, demo chatbot and review placeholders.
- courses/*.html: individual course detail pages.
- google-apps-script.gs: optional Google Sheets admission receiver.

ANDROID / GITHUB PAGES
1. Extract this ZIP on your phone.
2. Upload index.html and the courses folder to the repository root (plus any desired supporting files). Keep the folder structure unchanged.
3. WhatsApp is preconfigured to 917778935338 (7778935338). A second contact/WhatsApp number, 9324842567, is also shown in the contact section. Change these in index.html if needed.
4. For Google Sheets: create a Google Sheet, open Extensions > Apps Script, paste google-apps-script.gs, save, Deploy > New deployment > Web app, execute as you, access as Anyone, deploy. Copy the /exec URL into GOOGLE_SHEETS_WEB_APP_URL in index.html. Test with a sample inquiry. Apps Script access settings are your responsibility.
5. Commit/publish via GitHub Pages.

IMPORTANT LIMITATIONS
- Google Sheets is NOT connected until you deploy Apps Script and add the URL. Because the browser uses no-cors, it cannot confirm a successful write; verify by checking the sheet.
- Chatbot is a local keyword-based demo, NOT a real AI model. A real AI assistant requires a server/backend and an AI API key. Never put a private API key in HTML/JavaScript.
- Student login/dashboard is demo-only and stores a demo name/ID in local browser storage. It is NOT secure authentication. Real login requires a backend, database, password handling and access controls.
- Certificate verification only checks a sample ID in browser code. Official verification requires a trusted institute record/database/API.
- Review cards and online gallery images are demo/stock content. Replace with genuine reviews and photos with permission. Do not claim government approval or certificate validity unless verified.
- External gallery images require an internet connection.


NEW IN THIS BUILD
- Dark/Light mode toggle (saved locally in the browser).
- Google Maps embed and open-in-Maps link for the supplied Patan address; verify the pin/address before publishing.
- 3-question sample MCQ test; quiz score is not saved to a server.
- Extra SEO metadata and EducationalOrganization structured data.
- Primary WhatsApp 7778935338; secondary contact 9324842567.

REAL PHOTO GALLERY
The gallery currently uses online stock/reference photos, not verified photographs of NCE Institute. Replace them with photos of your own classroom, computer lab, teachers and students (with permission) before representing them as institute photos.

GOOGLE SHEETS CHECKLIST
1. Create a Google Sheet and open Extensions > Apps Script.
2. Paste google-apps-script.gs, save, then Deploy > New deployment > Web app.
3. Execute as your account; set access appropriately (Anyone makes the endpoint public, so avoid collecting sensitive data). Deploy and copy the /exec URL.
4. In index.html, replace the empty GOOGLE_SHEETS_WEB_APP_URL value with the URL in quotes.
5. Submit a test inquiry and verify a new row in the sheet. The static page cannot reliably confirm success when using no-cors; check the sheet directly.

SECURITY NOTES
- Student portal is a demo, not real authentication. Do not use it to store passwords or confidential student information. Production login requires secure backend/authentication and database rules.
- AI chatbot is keyword-based demo. A real AI chatbot requires a server-side API integration; never expose a private API key in public HTML.
- Certificate checking is demo-only until connected to official records.
- GitHub Pages hosts static files only; Apps Script can serve as a lightweight form endpoint, but a secure student portal requires a proper backend.
