# शिवराज मामा योजना मॉनिटरिंग डैशबोर्ड

Hindi-language front-end dashboard prototype for scheme monitoring for Vidisha and Sehore.

## What's included
- 12 color-coded scheme cards and progress meters
- Add/edit/delete tasks with owner/assignee, due date, status, percentage progress and notes
- Search and filter schemes/tasks
- KPI counters and charts for status/progress
- CSV import/export (Excel can open CSV files)
- PowerPoint report generation for all schemes or selected schemes
- Local-browser file attachments for small PDFs, images, CSVs, spreadsheets and documents
- Profile-photo upload preview
- User/team list UI with role labels and activate/deactivate controls
- Browser localStorage persistence; tasks start empty

## Preview locally
Open `index.html` in a modern browser with internet access for Chart.js and PptxGenJS CDN libraries.

## Important: prototype vs production
This is **not a production-ready multi-user application**. Data is stored in the current browser's localStorage, so it is not shared with colleagues and may be lost if browser data is cleared. Small attachments are limited to about 1.2 MB each. The user/role screen is a local management mockup and **does not provide authentication or enforce security**. Do not enter confidential or sensitive information.

Real sign-in for `consultant.shivrajoffice@gmail.com`, password reset, server-enforced Owner/Admin/Monitoring Officer/Team Member permissions, shared persistent database, audit logs, secure cloud file storage and backups require a backend (e.g. Supabase/Firebase) and a configured project. Never hard-code passwords or service-role keys in this repository.

## Free static hosting via GitHub Pages
A GitHub Actions deployment workflow is included at `.github/workflows/deploy-pages.yml`. A repository administrator must enable Pages once:
1. Open Settings → Pages.
2. Under Build and deployment, select **GitHub Actions** as the source.
3. Open the Actions tab and rerun the latest **Deploy dashboard to GitHub Pages** workflow.

The connected GitHub integration does not have permission to enable Pages automatically, so deployment will not complete until the repository owner makes that setting change. GitHub Pages hosts only the static front-end; it does not add the backend features listed above.
