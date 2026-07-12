


# 
```
# Telegram Drive - Phase 5.1 (Production Implementation)

Gunakan branch terbaru dari main.

WAJIB mengikuti workflow berikut:

- Selalu mulai dari latest main.
- Satu phase = satu branch.
- Satu branch = satu Pull Request.
- Satu Pull Request = satu merge.
- Jangan pernah force push ke main.
- Jangan menggunakan mock.
- Jangan menghapus fitur production yang sudah ada.
- Jangan membuat placeholder.
- Jangan membuat TODO tanpa implementasi.
- Gunakan production code.

Sebelum mengubah kode:

1. Pull latest main.
2. Jalankan lint.
3. Jalankan typecheck.
4. Jalankan build.
5. Jalankan seluruh regression test.
6. Pastikan baseline hijau.

==================================================================

PHASE 5.1

Implementasikan seluruh fitur berikut dalam SATU PHASE.

## Favorites

- Star / Unstar file
- Star / Unstar folder
- Favorites page
- Favorites sorting
- Favorites persistence
- Favorites API
- Favorites database

==================================================================

## Recent

- Recent files
- Recent folders
- Last opened
- Last viewed
- Last downloaded
- Recent API
- Recent database

==================================================================

## Folder Download ZIP

- Download folder sebagai ZIP
- Progress indicator
- Cancel download
- Preserve folder structure
- Streaming ZIP
- Large folder support
- Production ready

==================================================================

## File Detail Panel

Klik file akan menampilkan panel detail:

- Preview
- File Name
- Size
- Type
- MIME
- Owner
- Upload Date
- Modified Date
- Folder Path
- Telegram Message ID
- Telegram Channel
- File Hash
- Download Count

Desktop menggunakan side panel.

Mobile menggunakan bottom sheet.

==================================================================

## Breadcrumb Navigation

Contoh:

My Files
>
Movies
>
2026
>
Marvel

Breadcrumb dapat ditekan.

==================================================================

## File Information

Tambahkan metadata:

- Type
- Extension
- Size
- Created
- Modified
- Owner
- Path

==================================================================

QUALITY

Tidak boleh merusak fitur berikut:

✓ Upload
✓ Folder
✓ Rename
✓ Delete
✓ Move
✓ Copy
✓ Search
✓ Grid View
✓ List View
✓ Preview
✓ Download
✓ Copy Link
✓ Multi Select
✓ Bulk Actions
✓ Sort
✓ Filter
✓ Responsive UI

==================================================================

TESTING

Sebelum commit:

- lint
- typecheck
- build
- API integration
- Folder integration
- Playwright Chromium
- Playwright Firefox
- Playwright WebKit

Jika ada kegagalan:

- baca log GitHub Actions
- identifikasi root cause
- perbaiki production code
- jalankan ulang seluruh CI

Ulangi sampai seluruh GitHub Actions hijau.

==================================================================

Setelah selesai:

1. Push ke branch baru.
2. Buat Pull Request.
3. Tunggu seluruh GitHub Actions selesai.
4. Jangan merge jika masih ada satu saja check merah.
5. Perbaiki sampai seluruh CI hijau.
6. Jalankan regression test penuh.
7. Merge ke main jika semua hijau.
8. Hapus branch setelah merge.

==================================================================

Setelah merge selesai:

- Audit seluruh aplikasi.
- Pastikan tidak ada regression.
- Update README.md dan CHANGELOG.md dengan fitur Phase 5.1.
- Tulis ringkasan perubahan.
- Berikan daftar file yang diubah.
- Berikan daftar API yang ditambah atau diubah.
- Berikan daftar database/model yang berubah.
- Berikan hasil lint, build, typecheck, Playwright, GitHub Actions.
- Jangan lanjut ke Phase 5.2 sampai seluruh hasil Phase 5.1 sudah production-ready dan tervalidasi.




```
# 
```

Always start from the latest main branch.

One phase = one branch.
One branch = one Pull Request.
One Pull Request = one merge.

Do not continue to the next phase until:
- lint passes
- typecheck passes
- build passes
- API integration passes
- Playwright (Chromium, Firefox, WebKit) passes
- GitHub Actions are all green

Every new feature must preserve existing production functionality and include regression testing before merge.



```

# memperbaiki CI sampai hijau.
```


Do not start Phase 5.1.

Investigate every failed GitHub Action in PR #31.

Open each failed workflow log and identify the exact root cause.

Fix only the production code required to make all checks pass.

Do not remove any Phase 5.0 functionality.

After each fix:
- run lint
- typecheck
- build
- Playwright
- API integration
- push to the same PR

Repeat until every GitHub Action is green.

Only then merge PR #31.


```
# Prompt 1
```

Before starting Phase 5.1, perform a full regression audit.

Verify that all existing production features still work:

- Upload
- Folder creation
- Folder navigation
- Search
- List View
- Grid View
- File Preview
- Download
- Copy Link
- Rename
- Move
- Delete
- Mobile UI
- Desktop UI
- Responsive layout
- Telegram API integration

If any regression is found, fix it before merging.

Only when all CI is green and regression audit passes, merge PR #31 into main.

After merge, create a new branch for Phase 5.1.

Never stack multiple features in one PR.
One phase = one branch = one PR = one merge.



```

# Prompt 
```



Update roadmap.

Jangan mulai dari Trash.

Prioritaskan fitur yang paling meningkatkan pengalaman pengguna (UX) sebelum fitur keamanan.

Urutan implementasi:

Phase 5.0
- Multi Select
- Bulk Actions (Delete, Move, Copy, Download)
- Sort (Name, Date, Size, Type)
- Filter (Image, Video, Audio, Document, Archive)

Phase 5.1
- Favorites
- Recent
- Folder Download as ZIP
- Detail Panel
- Breadcrumb Navigation
- File Details

Phase 5.2
- Trash (Soft Delete)
- Restore
- Empty Trash
- Retention Policy

Setelah roadmap diperbarui, buat branch baru dari main dan implementasikan Phase 5.0 secara lengkap menggunakan production code.

Jangan menggunakan mock.
Jangan menghapus fitur yang sudah ada.
Semua perubahan harus lulus lint, typecheck, build, Playwright, dan GitHub Actions.
Buat PR ke main, merge jika seluruh CI hijau, lalu lanjut ke fitur berikutnya.

```
# Prompt 
```

Sekarang buat roadmap implementasi berdasarkan hasil audit.

Jangan langsung mengubah kode.

Kelompokkan semua fitur yang belum ada menjadi:

Phase 5
Phase 5.1
Phase 5.2
Phase 6
Phase 7
Phase Enterprise

Urutkan dari yang paling penting untuk production.

Pastikan roadmap membuat Telegram Drive mendekati Google Drive dan MEGA.

Tambahkan juga fitur UX yang masih kurang seperti:
- Multi Select
- Bulk Actions
- Sort & Filter
- Folder ZIP Download
- Recent
- Favorites
- Tags
- Detail Panel
- Breadcrumb Navigation
- File Details
- Drag & Drop Desktop
- Shared With Me
- Team Drive

Setelah roadmap selesai, pilih SATU fitur paling prioritas dan jelaskan alasannya. Jangan mengubah kode dulu.



```
# 
```

Audit seluruh project Telegram Drive dari origin/main.

Jangan langsung membuat branch.

Buat laporan lengkap mengenai SEMUA fitur yang masih belum ada dibandingkan Google Drive, Telegram Drive, dan MEGA.

Kelompokkan menjadi:

Phase 5
Phase 6
Phase 7

Untuk setiap fitur jelaskan:
- Sudah ada atau belum
- Tingkat prioritas
- Dampak ke user
- Estimasi kompleksitas
- Apakah membutuhkan perubahan backend atau hanya frontend

Urutkan berdasarkan prioritas production.

Jangan mengubah kode apa pun.

Setelah audit selesai, baru rekomendasikan satu fitur terbaik untuk dikerjakan berikutnya.



```
# 
```


Saya melanjutkan project Telegram Drive.

Current status:
- Backend production selesai.
- Upload, download, preview, folder, search, copy link sudah production.
- PR #29 sudah merged ke main.
- Semua lint, typecheck, build, Playwright, Chromium, Firefox, WebKit sudah PASS.

Mulai sekarang jangan mengulang fitur yang sudah selesai.

Fokus hanya pada fitur berikutnya yang belum ada.
Selalu gunakan production code.
Jangan membuat mock.
Jangan menghapus fitur yang sudah bekerja.
Selalu buat branch baru dan Pull Request baru.


```


# Prompt 29 – Final Production List View (MEGA Style)
```

Create a NEW branch from origin/main named feature/my-files-ui-final.

IMPORTANT:
- PR #28 has already been merged and closed.
- Do NOT modify or reopen PR #28.
- Continue from the current origin/main.
- Create a NEW PR when finished.
- Do NOT create mock UI.
- Implement only production-ready code.

Project:
This is a Telegram Drive web application inspired by Telegram + Google Drive + MEGA.
The backend, upload system, folders, search, file management, and previous production fixes are already completed and merged.
Do NOT rewrite working features.
Preserve all existing APIs and business logic.

Your task is ONLY to finish the remaining My Files production UI and UX.

Requirements:

1. Redesign My Files to look modern like MEGA / Google Drive while keeping our own identity.
2. Keep both Grid View and List View.
3. Add smooth switch animation between Grid and List.
4. List View should resemble MEGA:
   - thumbnail/icon
   - filename
   - file size
   - modified date
   - optional owner
   - context menu (three dots)
   - copy link button
5. Grid View:
   - responsive cards
   - consistent spacing
   - large preview
   - selection state
6. Folder cards:
   - cleaner layout
   - folder count
   - modified date
   - responsive
7. Improve breadcrumbs.
8. Improve search bar.
9. Sticky header on mobile.
10. Better spacing for Safe Area (Android & iPhone).
11. Better FAB placement.
12. Better empty states.
13. Better loading skeletons.
14. Better hover/focus/pressed states.
15. Better dark/light compatibility.
16. Mobile-first responsive design.
17. Tablet responsive.
18. Desktop responsive.

Maintain existing features:

- Upload Queue
- Folder creation
- Folder navigation
- File preview
- File download
- Copy Link
- Context Menu
- Search
- Breadcrumbs
- Upload progress
- Existing APIs
- Existing authentication
- Existing routing

Do NOT remove or break:
- Working backend
- MongoDB logic
- Upload logic
- Download logic
- Folder APIs
- Existing tests

Fix remaining UI inconsistencies without changing business logic.

Before committing:
- npm install
- npm run lint
- npm run typecheck
- npm run build
- Run Playwright tests
- Fix every failing test
- Verify Chromium, Firefox and WebKit

Only commit if:
- Build passes
- Typecheck passes
- Lint passes
- Browser tests pass
- Mobile layout verified
- No runtime errors

Finally:
- Commit changes.
- Push the new branch.
- Open a NEW Pull Request.
- Include screenshots of Desktop, Tablet and Mobile.
- Include a summary of every UI improvement.
- Do NOT stop until every requirement above has been completed and verified.



```
# Prompt 29 – Final Production List View (MEGA Style)
```


Continue working on the existing PR #28.

Do NOT create a new PR.

Implement the REAL production code only.

Goal:
Complete the My Files List View so it feels like a professional cloud drive similar to MEGA and Google Drive.

Requirements

1. Production List View

Redesign every row.

Each row must contain:

• Proper file/folder icon
• File/folder name
• Metadata under the name
    - size
    - modified date
    - optional type
• Copy Link button
• Three-dot context menu

The layout must be compact and clean.

Do not waste vertical space.

Support long filenames with ellipsis.

Responsive on:

- Mobile
- Tablet
- Desktop

------------------------------------------------

2. File Icons

Automatically display icons by file type.

Folder
Image
Video
Audio
PDF
ZIP
RAR
APK
DOCX
XLSX
PPTX
TXT
Unknown

Do not display the same icon for every file.

------------------------------------------------

3. Thumbnail Rules

List View

Image
→ small thumbnail

Video
→ thumbnail with play indicator

Other files
→ icon only

Folder
→ folder icon

No broken thumbnails.

------------------------------------------------

4. Copy Link

Copy icon must

• copy immediately

• show success toast

• work on desktop and mobile

------------------------------------------------

5. Context Menu

Three-dot menu must include

Preview

Download

Copy Link

Rename

Move

Delete

Properties

Desktop:
right click also opens this menu.

------------------------------------------------

6. Folder Rows

Folder row shows

Folder icon

Folder name

Number of files

Last modified

Three-dot menu

------------------------------------------------

7. Visual Polish

Rounded cards

Proper spacing

Better typography

Hover state (desktop)

Pressed state (mobile)

Smooth transitions

Skeleton loading

Empty state

Loading state

------------------------------------------------

8. Responsive

Desktop

Tablet

Mobile

No overlapping elements.

No clipped text.

------------------------------------------------

9. Accessibility

Keyboard navigation

Focus state

ARIA labels

Screen reader friendly

------------------------------------------------

10. Validation

Test manually on

Chrome

Firefox

Android Chrome

Desktop

Mobile

------------------------------------------------

Requirements

Do not create mock UI.

Implement production components.

Keep existing backend.

Do not break search.

Do not break uploads.

Do not break folder navigation.

Do not break copy link.

Do not break current API.

Run:

npm run lint

npm run typecheck

npm run build

Run manual QA.

Commit.

Push to the SAME PR #28.

Wait until every GitHub Action is green.

Merge only after every check passes.

Output only a PASS/FAIL checklist after manual verification.


```

# 
```

Root cause found from GitHub Actions.

The browser-runtime job is failing because the production app crashes while trying to connect to MongoDB.

Error:

MongooseServerSelectionError
connect ECONNREFUSED 127.0.0.1:27017

Fix the real production code and GitHub Actions.

Requirements:

- Find every place where MongoDB is initialized.
- Do not hardcode mongodb://127.0.0.1:27017.
- Use process.env.MONGODB_URI.
- If browser-runtime does not require MongoDB, prevent the connection during startup.
- If browser-runtime requires MongoDB, configure a MongoDB service in GitHub Actions.
- Keep using PR #28.
- Do not create another PR.
- Commit, push, rerun Actions, and merge only after all checks are green.



```
# Prompt untuk Codex
```



Continue working on the existing repository.

DO NOT create a new branch.
DO NOT create a new Pull Request.
Continue working on the current production branch/PR only.

Current production blockers:

1. Fix runtime error:
   crypto.randomUUID is not a function
   Folder creation must work on all supported browsers by using a compatible UUID implementation or a safe fallback.

2. Verify Create Folder actually creates a real folder through the existing backend API.
   No mock implementation.

3. Fix all overlay and z-index problems.
   Drawer, dialog, preview, context menu and bottom sheet must never overlap incorrectly.

4. Implement production My Files UI.

- List View (default)
  - Similar to Windows Explorer / MEGA.
  - Small file icon.
  - Filename.
  - File size.
  - Modified date.
  - Copy Link button.
  - Three-dot menu.
  - Single click opens preview.

- Grid View
  - Thumbnail cards.
  - Images show thumbnails.
  - Videos show preview.
  - Documents show proper icons.

5. Desktop:
   Right-click opens context menu.

6. Mobile:
   Long press opens bottom action sheet.

7. Verify:
   - Folder creation
   - Open preview
   - Copy Link
   - Download
   - Rename
   - Delete
   - Move
   - Search
   - Grid/List switch

8. Run build.
9. Run browser verification.
10. Commit only after manual verification.
11. Merge only after every GitHub check is green.

Output:
- Root cause
- Files changed
- Manual verification results
- PASS/FAIL for every feature

```

# prompt
```


STOP.

Do not claim the feature is complete.

I have manually tested the production build.

The implementation still contains production bugs.

Fix these before merging PR #28.

HIGH PRIORITY

1. Folder creation is broken.

Current error:

crypto.randomUUID is not a function

Do not use crypto.randomUUID directly.

Implement a cross-browser ID generator.

Use:

globalThis.crypto?.randomUUID?.()

If unavailable, use a UUID library or a deterministic fallback.

Folder creation must work on:

- Android Chrome
- Chromium
- Desktop Chrome
- Firefox

2. Drawer/Menu overlaps page content.

Fix layout stacking.

Correct all z-index values.

Drawer must never overlap page incorrectly.

3. Header spacing is broken.

Safe area and top spacing must be correct.

4. Floating Action Button overlaps file cards.

Reposition FAB.

5. Grid layout is still inconsistent.

6. Search/header/breadcrumb spacing must match Google Drive.

7. Run manual browser verification after every fix.

Do not mark COMPLETE until I can:

- create folders
- switch list/grid
- preview files
- copy links
- open context menu
- use upload queue

without any runtime errors.

Continue using PR #28.
Do not create another PR.
Merge only after all GitHub checks pass and these bugs are fixed.


```
# 
```

Do not wait indefinitely.

Check the current status of the remaining Chromium verification.

If it has failed:
- investigate the failure,
- fix it on the same PR (#28),
- push the fix,
- rerun the failed check.

If it is still running:
- report the current progress,
- wait until it finishes.

As soon as all GitHub checks are green:
1. Merge PR #28 into main.
2. Verify origin/main contains the merge commit.
3. Confirm the merge SHA.
4. Tell me to run:
   git pull
   npm run build
   npm start (or restart the process)

Do not create a new PR.
Continue using PR #28 until it is merged successfully.



```

# 
```
Wait until ALL GitHub checks are green.

Do not create another PR.

When Chromium verification finishes:

1. Merge PR #28 into main.
2. Verify merge succeeded.
3. Confirm the commit SHA now exists on origin/main.
4. Do not stop after merge.
5. Perform a final visual QA against the specification.
6. Report every implemented feature and every remaining issue.
7. Only say COMPLETE when the production-ready implementation matches the specification.

If any GitHub check fails, fix it on the same PR instead of creating a new one.




```
# Langkah berikutnya
```


STOP.

Do not investigate deployment or runtime anymore.

The production server is already running the latest commit.

The missing features are NOT a deployment problem.
They are missing implementation.

Continue working from the current codebase.

Implement all remaining My Files features until they exist in production.

Required:

1. Two view modes
   - List View (default, similar to MEGA mobile)
   - Grid View (thumbnail cards)

2. View switch button beside Search.

3. List View
   - file icon only
   - filename
   - size
   - modified date
   - copy-link icon
   - three-dot menu on right

4. Grid View
   - real image thumbnails
   - video thumbnails
   - file type icons

5. Single click/tap:
   Open preview.

6. Desktop:
   Right click opens context menu.

7. Mobile:
   Long press opens context menu.

8. Context menu:
   Open
   Download
   Copy Link
   Rename
   Move
   Delete
   Favorite
   Details

9. Folder creation must work.

10. Upload queue must work.

11. Search.

12. Breadcrumb navigation.

13. No overlapping UI.

14. Responsive desktop/tablet/mobile.

Do not create mock UI.

Implement the real production code.

Commit only after manual verification.

Push to the same PR until every feature is finished.


```
# mengubah UX My Files menjadi setara aplikasi cloud storage modern
```

# Phase 5 – Professional File Explorer UX (Google Drive + Windows Explorer + MEGA)

Lakukan redesign total pada halaman My Files agar terasa seperti aplikasi cloud storage profesional.

Jangan hanya memperbaiki komponen lama.

Buat pengalaman pengguna baru yang menggabungkan kelebihan Google Drive, Windows File Explorer, dan MEGA.

## Target

Ini adalah File Explorer utama untuk Telegram Drive.

Prioritaskan UX, kemudahan penggunaan, performa, dan konsistensi.

Backend, MongoDB, Telegram Bot, API, database schema, upload pipeline, dan autentikasi TIDAK BOLEH diubah.

Semua perubahan hanya pada frontend.

---

# 1. Dua Mode Tampilan

Tambahkan tombol View Switch di kanan atas.

Mode:

• List View (Default)
• Grid View

Pilihan user harus diingat (localStorage).

---

# 2. List View

Default menggunakan List View.

Jangan memakai card besar.

Gunakan layout seperti MEGA atau Windows Explorer.

Setiap file tampil sebagai satu baris.

Kolom:

Icon
Nama
Ukuran
Folder
Tanggal Upload
Favorite (jika ada)
Share Status (jika ada)

Contoh:

🖼 IMG-20260710.jpg
36 KB • Foto • Today

📄 Invoice.pdf
2.3 MB • Yesterday

🎬 Movie.mp4
1.8 GB • Today

Tidak menggunakan thumbnail besar.

Gunakan icon berdasarkan tipe file.

---

# 3. Grid View

Grid View digunakan untuk melihat thumbnail.

Gunakan layout seperti Google Drive.

Thumbnail besar.

Nama file.

Ukuran.

Tanggal.

Hover effect.

Lazy loading.

Responsive.

---

# 4. Preview

Klik kiri (desktop)

atau

Tap (mobile)

langsung membuka preview.

Bukan membuka menu.

Preview wajib mendukung:

Image

Video

Audio

PDF

Text

Office document (placeholder bila viewer belum tersedia)

Preview fullscreen.

Zoom.

Swipe.

Keyboard navigation.

Download.

Close.

---

# 5. Context Menu

Desktop:

Klik kanan.

Mobile:

Long Press.

Hapus seluruh tombol tiga titik pada setiap file.

Context Menu harus berisi:

Open

Open in New Tab

Copy Link

Download

Rename

Move

Copy

Favorite

Details

Delete

Gunakan menu modern seperti Google Drive.

---

# 6. Details Panel

Saat memilih Details,

munculkan panel seperti Windows Explorer.

Data:

Nama

Ukuran

Tipe File

Folder

Owner

Upload Date

Modified Date

Telegram File ID

Hash (jika ada)

Download Link

Copy Link

Thumbnail

Semua informasi tersusun rapi.

---

# 7. Folder

Folder tampil berbeda dari file.

Klik folder:

langsung masuk folder.

Breadcrumb otomatis berubah.

Back bekerja.

Tidak reload halaman.

---

# 8. Thumbnail

Thumbnail hanya muncul pada Grid View.

List View hanya memakai icon.

Image.

Video.

PDF cover.

Fallback icon.

Lazy load.

---

# 9. Search

Search realtime.

Folder dan file ikut difilter.

Highlight keyword.

---

# 10. Responsive

Desktop.

Tablet.

Mobile.

Semua menu tidak boleh saling bertabrakan.

Tidak boleh overflow.

Tidak boleh terpotong.

---

# 11. Accessibility

Keyboard navigation.

Focus state.

ARIA.

Screen reader.

---

# 12. Animasi

Gunakan animasi halus.

Open preview.

Context menu.

Hover.

Selection.

Tidak berlebihan.

---

# 13. Performa

Virtual scrolling bila file banyak.

Lazy rendering.

Image lazy loading.

Optimasi re-render.

---

# 14. QA

Sebelum push:

npm run lint

npm run typecheck

npm run build

Jalankan website.

Uji manual seluruh fitur.

Pastikan:

PASS Folder

PASS Preview

PASS Grid View

PASS List View

PASS Context Menu

PASS Copy Link

PASS Download

PASS Rename

PASS Move

PASS Delete

PASS Favorite

PASS Details Panel

PASS Search

PASS Responsive

PASS Mobile

PASS Desktop

PASS Thumbnail

PASS Accessibility

PASS Performance

Jika ada bug,

perbaiki terlebih dahulu.

Jangan push sebelum seluruh fitur benar-benar bekerja.

Buat Pull Request.

Merge hanya setelah semua GitHub checks hijau.

Jangan berhenti di tengah proses.

Teruskan sampai implementasi selesai tanpa meminta konfirmasi selama hanya mengubah frontend My Files.



```
# Prompt
```

Do not merge PR #28 yet.

One required check is still failing:

My Files runtime verification / browser-runtime

Find the root cause and fix it.

Requirements:

- Do not bypass, disable, or ignore the failing test.
- Fix the real runtime problem.
- Run the browser runtime verification until it passes.
- Ensure all GitHub checks are green.
- Verify manually in Chromium after the fix.

Re-test all My Files features:

✓ Open folder
✓ Open file
✓ Preview image
✓ Preview video
✓ Preview PDF
✓ Preview audio
✓ Preview text
✓ Copy Link
✓ Download
✓ Rename
✓ Move
✓ Delete
✓ Favorite
✓ Create Folder
✓ Search
✓ Thumbnail
✓ Mobile
✓ Desktop

Do not create another PR.

Continue working on PR #28 until every check passes.

Merge only after all GitHub checks are green.



```
# Prompt
```


Production Audit & Fix - My Files

PR #26 sudah merged tetapi implementasi di production tidak sesuai.

Lakukan audit penuh pada seluruh fitur My Files.

Jangan menganggap pekerjaan selesai hanya karena build, lint, typecheck, atau CI hijau.

Verifikasi dengan menjalankan aplikasi dan memastikan semua fitur benar-benar bekerja.

Temukan dan perbaiki seluruh masalah berikut.

1.
Klik folder harus benar-benar membuka folder.

2.
Klik file harus membuka preview.

3.
Preview harus bekerja untuk:
- Image
- Video
- PDF
- Audio
- Text

4.
Copy Link harus bekerja.

5.
Download harus bekerja.

6.
Rename harus bekerja.

7.
Move harus bekerja.

8.
Delete harus bekerja.

9.
Favorite harus bekerja.

10.
Create Folder harus bekerja.

Bug saat ini:

crypto.randomUUID is not a function

Jangan gunakan crypto.randomUUID apabila environment tidak mendukung.

Gunakan solusi yang kompatibel dengan browser lama maupun Node:

- crypto.randomUUID bila tersedia
- fallback ke nanoid atau uuid
- atau fallback internal yang aman

Folder wajib dapat dibuat tanpa error.

11.

Pastikan thumbnail muncul.

12.

Pastikan tidak ada overlay, drawer, modal, atau menu yang saling bertabrakan.

13.

Pastikan seluruh perubahan benar-benar terlihat di production.

Jika ada cache Next.js, build cache, service worker, hydration, stale deployment, atau routing yang menyebabkan perubahan tidak muncul, perbaiki juga.

Jangan berhenti sampai perubahan benar-benar muncul saat website dijalankan.

Sebelum membuat PR lakukan:

npm run lint

npm run typecheck

npm run build

jalankan website

uji seluruh fitur secara manual

baru push

buat PR

merge jika seluruh checks hijau.

Output akhir wajib berisi checklist PASS/FAIL untuk setiap fitur yang telah diuji secara langsung, bukan hanya berdasarkan pembacaan kode.


```
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
