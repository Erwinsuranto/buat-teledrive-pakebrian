# Phase 1 — Redesign My Files menjadi Google Drive Mobile Style
```


Title: Phase 1 - Redesign My Files UI (Google Drive Mobile Style)

Project:
Telegram Drive (Next.js + React + TypeScript)

Objective:
Replace the current demo/card-based My Files interface with a modern mobile-first file manager inspired by Google Drive.

IMPORTANT:
This is a redesign only.
Do NOT change backend APIs.
Do NOT change database models.
Do NOT break existing upload, folder or file APIs.

The current backend already works.

Existing APIs:
- GET /api/folders
- POST /api/folders
- Existing file endpoints
- Existing upload endpoints

Use only these APIs.

====================================

UI GOALS

The interface should feel like:

- Google Drive Mobile
- Samsung My Files
- Files by Google

NOT like a dashboard.

====================================

PAGE STRUCTURE

Header

Telegram Drive

Search bar

Floating Action Button

Folders section

Files section

Bottom navigation stays unchanged.

====================================

SEARCH

Place search at the top.

Large rounded search bar.

Search both folders and files.

Real-time filtering.

====================================

FOLDERS

Replace large cards.

Display folders in compact list.

Each row:

📁 Folder Name

2 files • Updated today

⋮

No large preview icons.

No oversized cards.

Clicking a folder opens it.

====================================

FILES

Below folders.

Each file row contains:

Thumbnail (48-64px)

Filename

File size

Upload date

⋮ menu

No giant cards.

Show many files on one screen.

====================================

THUMBNAILS

Images:
Show real thumbnail.

Videos:
Show video thumbnail if available.

PDF:
Show first page preview if available.

Other files:
Use file icon.

Fallback to icon when preview unavailable.

====================================

FLOATING ACTION BUTTON

Single FAB.

When tapped:

Upload File

Upload Photo

Create Folder

====================================

BREADCRUMB

When inside folder:

Home > Folder Name

Allow returning to previous folder.

====================================

EMPTY STATES

Folders:

"No folders yet"

Files:

"No files yet"

Provide Upload button.

====================================

MOBILE DESIGN

Optimize for phones.

No horizontal scrolling.

Comfortable spacing.

Large tap targets.

====================================

ACCESSIBILITY

Keyboard accessible.

ARIA labels.

Focus states.

====================================

KEEP EXISTING

Do NOT change:

Authentication

Database

API routes

Upload logic

Folder logic

File logic

====================================

REMOVE

Remove oversized cards.

Remove demo placeholders.

Remove folder preview icons.

Remove unnecessary white space.

Remove dashboard appearance.

====================================

OUTPUT

Deliver a production-ready responsive UI.

Keep current backend integration.

Run:

npm run build

Fix every TypeScript error.

Fix every lint issue.

Commit changes.

Push to GitHub.

Create Pull Request.

Wait for review before continuing to Phase 2.


```
