# शिवराज मामा योजना मॉनिटरिंग डैशबोर्ड

A colorful Hindi front-end prototype for monitoring scheme-related tasks for Vidisha and Sehore.

## Run locally
Open `index.html` in a modern browser. The page uses no build step. CSV import/export and task editing are available in the prototype.

## Features in this prototype
- Color-coded scheme cards and progress meters
- Add/edit/delete tasks, assign a responsible person, due date, status, progress and notes
- Search and filter schemes/tasks
- CSV import, CSV export and copy task list
- KPI counters for total schemes, total tasks, in-progress and completed tasks
- Task data starts empty

## Important limitations
This is a **front-end prototype**, not a production-ready multi-user system. Task data exists only in browser memory and resets on refresh. There is no real authentication, password management, database persistence, secure role-based access, shared team workspace, or actual file/PDF/photo storage. The portrait area is a placeholder; add an approved image asset before publishing.

The requested owner email is displayed for planning purposes only; this page does not authenticate or grant ownership to that email address.

## Production next steps
1. Add a backend database (for example, Supabase or Firebase) and persist schemes/tasks.
2. Implement secure sign-in and invite users, with server-enforced Owner/Admin/Monitoring Officer/Team Member permissions.
3. Add private storage for PDFs, spreadsheets, images and other attachments.
4. Add audit logs, backups, validation, access rules and deployment configuration.
5. Configure the requested owner account through the chosen authentication provider—never hard-code passwords in source code.

## Deployment
This static prototype can be previewed with GitHub Pages after enabling Pages in repository settings. GitHub Pages alone will **not** add authentication, shared database storage, or secure permissions.
