
# Prompt lanjutan
```


Production UX Fix - Google Drive Interaction

Jangan ubah backend, database, authentication, Telegram Bot, upload pipeline, atau API.

Fokus hanya pada My Files UI/UX.

Perbaiki seluruh interaction agar mengikuti pola Google Drive modern.

1. Klik kiri pada file wajib langsung membuka Preview.

2. Desktop:
- Right click membuka Context Menu.
- Tidak menggunakan tombol tiga titik lagi.

3. Mobile:
- Tap membuka Preview.
- Long press membuka Bottom Sheet.

4. Context Menu / Bottom Sheet wajib berisi:

Open
Copy Link
Download
Rename
Move
Favorite
Delete
Details

5. Implementasikan Copy Link menggunakan share/download URL yang sudah tersedia.

6. Perbaiki seluruh z-index sehingga Drawer, Context Menu, Modal, Bottom Sheet, Search Overlay, dan Header tidak saling bertabrakan.

7. Perbaiki thumbnail:
- image thumbnail
- video thumbnail
- pdf preview
- fallback icon bila preview gagal

8. Semua Preview harus fullscreen dengan tombol Close dan Download.

9. Hilangkan seluruh interaction yang membingungkan.

10. Setelah selesai:
- build
- lint
- typecheck
- test
- push
- buat PR
- merge bila seluruh checks hijau.

Jangan berhenti sebelum seluruh interaction My Files benar-benar terasa seperti Google Drive modern.


```
# Telegram Drive - My Files QA & Production Fix (Post PR #24)

# 
```
Telegram Drive - My Files QA & Production Fix (Post PR #24)


Context

PR #24 sudah merged.
Phase 2–5 sudah selesai.
Semua GitHub checks hijau.

Sekarang fokus HANYA pada penyempurnaan My Files.

Jangan mengubah backend API, database schema, authentication, Telegram Bot, upload pipeline, atau endpoint yang sudah berjalan.

Semua perbaikan harus berada di frontend dan integrasi frontend dengan API yang sudah ada.

==================================================

TARGET

My Files harus terasa seperti Google Drive modern.

Bukan sekadar mirip tampilannya, tetapi juga pengalaman pengguna.

Semua fitur harus benar-benar dapat digunakan.

==================================================

PERBAIKI SELURUH BUG

Open file

Download file

Thumbnail image

Thumbnail video

Thumbnail PDF

Responsive mobile

Responsive tablet

Responsive desktop

Bottom Sheet mobile

Overflow menu

Long filename

Lazy loading

Infinite scrolling

Loading state

Error state

Empty state

Refresh state

Folder navigation

Breadcrumb

Selection state

==================================================

FILE CARD

Hilangkan model card lama.

Gunakan layout modern seperti Google Drive.

Card harus sederhana.

Thumbnail besar.

Nama file.

Ukuran file.

Tanggal upload.

Tidak ada icon atau elemen yang membingungkan.

==================================================

MENU AKSI

Jangan gunakan dropdown kecil.

Pada mobile gunakan Bottom Sheet.

Pada desktop gunakan Context Menu.

Semua tombol wajib berfungsi.

Open

Preview

Download

Rename

Move

Delete

Details

Share

==================================================

THUMBNAIL

Image

Tampilkan thumbnail asli.

Video

Gunakan thumbnail video.

PDF

Gunakan preview halaman pertama.

File lain

Gunakan icon sesuai tipe file.

==================================================

OPEN

Open harus benar-benar membuka file.

Image

Preview viewer.

Video

Video player.

PDF

PDF viewer.

Audio

Audio player.

Text

Viewer.

==================================================

DOWNLOAD

Download harus benar-benar mengunduh file.

Tidak boleh placeholder.

==================================================

PREVIEW

Gunakan modal fullscreen.

Support pinch zoom image.

Support keyboard desktop.

Support swipe mobile.

Support ESC.

Support next previous.

==================================================

FOLDER

Folder dapat ditekan.

Masuk folder.

Kembali folder.

Breadcrumb berjalan.

Jumlah file benar.

==================================================

SEARCH

Realtime.

Cepat.

Tanpa refresh.

==================================================

PERFORMANCE

Optimalkan render.

Kurangi re-render.

Gunakan lazy loading.

Gunakan memo bila diperlukan.

==================================================

ACCESSIBILITY

Keyboard navigation.

ARIA.

Focus state.

==================================================

CODE QUALITY

Refactor bila diperlukan.

Hapus placeholder.

Hapus dead code.

Hapus duplicate component.

Jangan membuat technical debt.

==================================================

TESTING

Setelah coding selesai WAJIB:

- Build
- Type check
- Lint
- Jalankan semua test
- Perbaiki semua error
- Pastikan GitHub Checks hijau

==================================================

OUTPUT

Jangan berhenti di tengah.

Kerjakan semua bug di atas dalam satu Pull Request.

Commit bila diperlukan.

Push ke branch.

Buat Pull Request.

Merge jika seluruh checks hijau.

==================================================

IMPORTANT

Jangan berhenti meminta konfirmasi.

Jangan bertanya "lanjut?"

Jangan membuat roadmap baru.

Jangan membuat placeholder baru.

Jangan memberi contoh implementasi.

Langsung implementasikan sampai selesai.

Hanya berhenti jika backend API, database schema, atau authentication memang harus diubah. Selain itu lanjutkan otomatis sampai seluruh My Files benar-benar production-ready.



```
# 
```


Do not start the Authentication phase yet.

Authentication will be implemented later.

Continue with all remaining frontend and user experience phases that do not require changing:

- Authentication
- Database schema
- Backend APIs

Continue improving Telegram Drive until the My Files experience is production-ready.

Complete in order:

Phase 2
- File and folder interactions
- Bottom sheet actions
- Mobile usability
- Touch interactions

Phase 3
- Real thumbnails
- Preview viewer
- Image viewer
- PDF viewer
- Video player

Phase 4
- Performance
- Lazy loading
- Infinite scrolling
- Responsive improvements

Phase 5
- Polish
- Animations
- Accessibility
- UX refinements

Automatically continue between phases without asking for confirmation.

Only stop if backend APIs, database schema, or authentication must change.


```

# 
```
Do not start the Authentication phase yet.

Authentication will be implemented later.

Continue with all remaining frontend and user experience phases that do not require changing:

- Authentication
- Database schema
- Backend APIs

Continue improving Telegram Drive until the My Files experience is production-ready.

Complete in order:

Phase 2
- File and folder interactions
- Bottom sheet actions
- Mobile usability
- Touch interactions

Phase 3
- Real thumbnails
- Preview viewer
- Image viewer
- PDF viewer
- Video player

Phase 4
- Performance
- Lazy loading
- Infinite scrolling
- Responsive improvements

Phase 5
- Polish
- Animations
- Accessibility
- UX refinements

Automatically continue between phases without asking for confirmation.

Only stop if backend APIs, database schema, or authentication must change.




```
# Phase 2
```

Workflow Instructions

Complete each phase in order.

After finishing a phase:

1. Run a full build.
2. Fix every TypeScript error.
3. Fix every lint issue.
4. Verify existing functionality still works.
5. Commit changes.

If there are no blocking issues:

Automatically continue to the next phase.

Do NOT stop after every phase asking for confirmation.

Only stop and request confirmation if:

- A backend API must change.
- A database schema must change.
- Authentication must change.
- Existing functionality would become incompatible.
- A design decision cannot be made automatically.
- A production risk requires user approval.

Otherwise, continue implementing the roadmap until all phases are completed.

At the end, create a single Pull Request containing all completed phases and provide:
- Summary of completed work
- Screenshots
- Remaining improvements (if any)



```
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
