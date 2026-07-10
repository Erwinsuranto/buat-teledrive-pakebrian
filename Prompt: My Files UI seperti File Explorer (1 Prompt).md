# Prompt: My Files UI Premium (Compact File Explorer)


# Prompt: File Management Experience
```

Lanjutkan pengembangan UI Telegram Drive dengan menyempurnakan pengalaman File Management agar terasa seperti aplikasi cloud storage modern.

Target:
Membuat pengelolaan file cepat, mudah, dan konsisten di seluruh aplikasi.

Tambahkan:

- Multi Select (checkbox pada file/folder).
- Select All.
- Bulk Actions:
  - Download
  - Move
  - Copy
  - Delete
  - Favorite
  - Share
- Drag & Drop untuk memindahkan file (UI saja).
- Rename dengan inline editing.
- Move dan Copy menggunakan dialog pemilihan folder.
- Favorite dengan ikon bintang.
- Trash (Recycle Bin) sebagai placeholder.
- Restore File (placeholder).
- Delete Permanently (placeholder).
- Progress dialog untuk operasi file (mock).
- Toast notification untuk setiap aksi.
- Shortcut keyboard (Ctrl+A, Delete, F2, Ctrl+C, Ctrl+V sebagai placeholder UI).

Pastikan semua fitur menggunakan komponen reusable yang sudah dibuat dan tampil konsisten dengan My Files, Search, Upload, Preview, dan Dashboard.

Jangan mengubah backend, API, database, authentication, Telegram Bot, upload/download logic, maupun service.

Update README.md dengan bagian "File Management".

Setelah selesai:
- Ringkas perubahan.
- Sebutkan file yang dibuat dan diubah.
- Jelaskan komponen reusable yang digunakan.
- Lakukan visual audit agar seluruh fitur File Management memiliki kualitas setara aplikasi cloud storage modern.



```
# Prompt: Settings & Preferences
```

Lanjutkan pengembangan UI Telegram Drive dengan membuat halaman Settings yang modern, bersih, dan konsisten dengan seluruh aplikasi.

Target:
Menyediakan pusat pengaturan pengguna yang siap dihubungkan ke backend pada tahap berikutnya.

Tambahkan menu:

- Profile
- Appearance (Light, Dark, System)
- Language
- Notifications
- Download Preferences
- Upload Preferences
- Privacy
- Security
- Connected Telegram Account
- Connected Google Drive (placeholder)
- Storage Information
- Keyboard Shortcuts
- About Application

Tambahkan fitur UI:

- Toggle Switch
- Dropdown
- Input Field
- Save Button
- Reset to Default
- Confirmation Dialog
- Success & Error Toast (mock)

Gunakan komponen reusable yang sudah dibuat.

Pastikan:
- Responsive.
- Desain konsisten dengan halaman lain.
- Menggunakan spacing, typography, dan ikon yang sama.

Jangan mengubah backend, API, database, authentication, Telegram Bot, upload logic, download logic, maupun service.

Update README.md dengan bagian "Settings & Preferences".

Setelah selesai:
- Jelaskan perubahan.
- Sebutkan file yang dibuat dan diubah.
- Sebutkan komponen reusable yang digunakan.
- Lakukan visual audit agar halaman Settings memiliki kualitas yang sama dengan halaman lainnya.



```

# Prompt: Dashboard & Home Experience
```


Lanjutkan pengembangan UI Telegram Drive dengan menyempurnakan halaman Home/Dashboard.

Target:
Membuat Dashboard terasa seperti halaman utama aplikasi cloud storage modern, bukan landing page biasa.

Tambahkan:

- Welcome Header yang dinamis.
- Quick Statistics:
  - Total Files
  - Total Folders
  - Storage Used
  - Recent Uploads
- Quick Actions:
  - Upload File
  - Upload Folder
  - New Folder
  - Search
- Recent Files.
- Recent Folders.
- Favorites.
- Recent Activity Timeline.
- Storage Usage Card dengan progress bar.
- Recent Downloads.
- Empty State jika belum ada data.
- Skeleton Loading.
- Responsive untuk desktop, tablet, dan mobile.
- Gunakan animasi ringan dan konsisten dengan halaman lainnya.

Gunakan kembali komponen reusable yang sudah dibuat.

Jangan mengubah backend, API, database, authentication, upload, download, Telegram Bot, routing, maupun service.

Update README.md dengan bagian "Dashboard Experience".

Setelah selesai:
- Jelaskan perubahan.
- Sebutkan file yang dibuat dan diubah.
- Sebutkan komponen reusable yang digunakan.
- Lakukan visual audit agar Dashboard memiliki kualitas yang sama dengan My Files, Search, Upload, dan Preview.


```
# Prompt: File Preview & Details
```
Lanjutkan pengembangan UI Telegram Drive dengan menyempurnakan fitur File Preview dan File Details.

Target:
Membuat pengalaman membuka file terasa seperti Google Drive atau OneDrive.

Tambahkan:

- Preview gambar langsung.
- Preview video dengan player.
- Preview audio dengan player.
- Preview PDF.
- Preview dokumen (placeholder).
- Preview arsip (ZIP/RAR) berupa informasi isi file.
- Fullscreen Preview.
- Zoom In / Zoom Out untuk gambar dan PDF.
- Navigasi Previous / Next file.
- Download Button.
- Share Button (placeholder).
- Copy Link (placeholder).
- Favorite.
- Rename.
- Move.
- Delete.
- Metadata lengkap:
  - Nama
  - Ukuran
  - Tipe File
  - Created
  - Updated
  - Telegram File ID
  - Channel
  - Tags
  - Status

Gunakan Side Details Panel yang modern.

Pastikan Preview dan Details tetap konsisten dengan My Files, Search, dan Upload.

Gunakan kembali komponen reusable yang sudah dibuat.

Jangan mengubah backend, API, database, Telegram Bot, authentication, upload logic, download logic, maupun service.

Update README.md dengan bagian "File Preview & Details".

Setelah selesai:
- Jelaskan perubahan.
- Sebutkan file yang dibuat dan diubah.
- Jelaskan komponen reusable yang digunakan.
- Lakukan visual audit agar pengalaman Preview setara aplikasi cloud storage modern.




```
# Prompt: Upload Experience
```

Lanjutkan pengembangan UI Telegram Drive dengan menyempurnakan halaman Upload agar terlihat seperti aplikasi cloud storage modern.

Target:
- Pengalaman upload sederhana, cepat, dan profesional.
- Konsisten dengan My Files dan Search.
- Gunakan kembali komponen reusable yang sudah ada.

Tambahkan:

- Drag & Drop upload area.
- Tombol "Choose Files" dan "Choose Folder".
- Multiple file upload (mock).
- Upload queue.
- Progress bar untuk setiap file.
- Pause, Resume, Cancel (placeholder).
- Status Uploading, Completed, Failed, Waiting.
- Informasi nama file, ukuran, dan estimasi waktu.
- Empty state sebelum ada file.
- Skeleton loading.
- Notifikasi upload berhasil atau gagal (mock).
- Responsive untuk desktop, tablet, dan mobile.
- Gunakan animasi ringan.

Jangan mengubah backend, API, database, Telegram Bot, autentikasi, upload logic, download logic, maupun service.

Update README.md dengan bagian "Upload Experience".

Setelah selesai:
- Jelaskan perubahan.
- Sebutkan file yang dibuat dan diubah.
- Sebutkan komponen reusable yang digunakan.
- Lakukan visual audit agar tampilan Upload memiliki kualitas yang sama dengan My Files dan Search.



```
# Prompt: Search Experience
```

Lanjutkan pengembangan UI Telegram Drive dengan menyempurnakan halaman Search agar memiliki pengalaman pencarian seperti aplikasi cloud storage modern.

Target:
- Search terasa cepat, bersih, dan profesional.
- Konsisten dengan komponen Explorer yang sudah dibuat.
- Gunakan kembali komponen reusable yang sudah ada, jangan membuat duplikasi.

Tambahkan:

- Search bar yang lebih besar dan menjadi fokus halaman.
- Live search (mock data).
- Recent searches.
- Search suggestions.
- Filter berdasarkan jenis file (Image, Video, Document, Archive, Audio, Folder).
- Sort (Name, Date, Size, Type).
- View mode mengikuti My Files (List, Grid, Large Grid).
- Highlight kata yang dicari.
- Empty state jika hasil tidak ditemukan.
- Skeleton loading saat pencarian.
- Details panel dan context menu tetap dapat digunakan pada hasil pencarian.
- Breadcrumb dan toolbar tetap konsisten.

Jangan mengubah backend, API, database, authentication, upload, download, bot, maupun service.

Update README.md dengan bagian "Search Experience".

Setelah selesai:
- Jelaskan perubahan.
- Sebutkan file yang dibuat dan diubah.
- Jelaskan komponen reusable yang digunakan kembali.
- Lakukan visual audit agar tampilan Search memiliki kualitas yang sama dengan My Files.



```
# Prompt: Telegram Drive — Phase 1 UI Explorer Foundation
```
Lakukan pengembangan dan penyempurnaan UI Telegram Drive untuk menyelesaikan Phase 1: UI Explorer Foundation.

## Tujuan

Bangun fondasi UI yang modern, profesional, reusable, dan siap dihubungkan ke backend Telegram di tahap berikutnya.

Target kualitas setara aplikasi cloud storage modern seperti:

- Google Drive
- Dropbox
- OneDrive
- Windows Explorer
- VS Code Explorer

Jangan menyalin desain mereka secara langsung, tetapi gunakan prinsip UX yang serupa.

----------------------------------------------------------------

RULES

Jangan mengubah:

- Backend
- API
- Database
- MongoDB
- Telegram Bot
- Authentication
- Upload Logic
- Download Logic
- Services
- Business Logic
- Routing yang sudah stabil

Fokus hanya pada:

Frontend
UI
UX
Component Structure
Documentation

----------------------------------------------------------------

DESIGN PRINCIPLES

UI harus:

- Clean
- Modern
- Minimal
- Premium
- Professional
- Productivity First

Hindari:

- Tampilan seperti template demo.
- Area kosong yang tidak memiliki fungsi.
- Komponen dengan gaya berbeda-beda.
- Warna berlebihan.
- Padding tidak konsisten.

Pastikan seluruh halaman terasa sebagai satu aplikasi.

----------------------------------------------------------------

1. NAVBAR

Redesign Navbar.

Harus memiliki:

Logo Telegram Drive

Nama aplikasi

Search Bar

Menu:

Home

My Files

Upload

Search

About

Help

User Avatar

Dropdown User

Sticky Navbar

Backdrop Blur ringan

Shadow tipis

Responsive

Desktop

Tablet

Mobile

Active Menu

Hover Effect

Keyboard Navigation

Accessibility

----------------------------------------------------------------

2. PAGE HEADER

Tambahkan Header modern.

Isi:

Judul Halaman

Deskripsi singkat

Statistics Cards:

Folders

Files

Storage

Favorites

Gunakan layout yang ringkas.

----------------------------------------------------------------

3. TOOLBAR

Tambahkan Toolbar Explorer.

Isi:

New Folder

Upload

Refresh

Search

Filter

Sort

View Switcher

List

Grid

Large Grid

Toolbar tetap berada di bawah Header.

----------------------------------------------------------------

4. EXPLORER WORKSPACE

Perbaiki area utama.

Support:

List View

Grid View

Large Grid View

Hover

Selected

Keyboard Focus

Responsive

----------------------------------------------------------------

5. BREADCRUMB

Contoh:

Home

>

My Files

>

Folder

>

Sub Folder

Breadcrumb selalu terlihat.

----------------------------------------------------------------

6. CONTEXT MENU

Desktop:

Klik kanan.

Mobile:

Long Press.

Menu:

Open

Open in New Tab

Preview

Rename

Favorite

Share

Copy Link

Move

Copy

Download

Delete

Properties

Backend belum perlu dibuat.

Gunakan placeholder action.

----------------------------------------------------------------

7. DETAILS PANEL

Gunakan Side Panel.

Bukan modal.

Isi:

Preview

Nama

Jenis

Ukuran

Created

Updated

Folder ID

Telegram Channel

Visibility

Tags

Download Link

----------------------------------------------------------------

8. EMPTY STATE

Buat Empty State untuk:

Folder kosong

Search kosong

Belum ada upload

Error

Gunakan ilustrasi sederhana.

----------------------------------------------------------------

9. LOADING

Gunakan Skeleton Loading.

Bukan spinner biasa.

----------------------------------------------------------------

10. RESPONSIVE

Desktop

Tablet

Mobile

Tidak ada elemen yang rusak.

----------------------------------------------------------------

11. ANIMATION

Hover

Open Folder

Context Menu

Dropdown

Details Panel

Semua animasi ringan.

----------------------------------------------------------------

12. COMPONENT STRUCTURE

Pisahkan komponen.

Reusable.

Mudah dikembangkan.

Jangan membuat satu file yang sangat panjang.

Gunakan struktur folder yang rapi.

----------------------------------------------------------------

13. CODE QUALITY

Gunakan:

Clean Code

TypeScript yang baik

Naming konsisten

Komentar seperlunya

Tidak ada duplikasi komponen.

----------------------------------------------------------------

14. README.md

Update README.md.

Tambahkan:

# Phase 1 UI Explorer Foundation

Jelaskan:

- Navbar
- Header
- Toolbar
- Explorer Workspace
- View Mode
- Breadcrumb
- Context Menu
- Details Panel
- Empty State
- Loading State
- Responsive Design
- Reusable Components

Tambahkan juga roadmap bahwa seluruh UI sudah siap dihubungkan ke backend Telegram pada tahap berikutnya.

----------------------------------------------------------------

15. VISUAL AUDIT

Sebelum menganggap pekerjaan selesai:

Audit seluruh tampilan.

Pastikan:

- Tidak ada area kosong yang tidak memiliki tujuan.
- Tidak ada komponen yang terlihat sementara.
- Alignment konsisten.
- Spacing konsisten.
- Typography konsisten.
- Warna konsisten.
- Shadow konsisten.
- Border Radius konsisten.
- Responsive berjalan baik.

Jika menemukan bagian yang terasa kurang profesional, perbaiki sebelum selesai.

----------------------------------------------------------------

16. FINAL REPORT

Setelah selesai:

Berikan laporan:

1. Ringkasan perubahan.

2. Alasan UX dan desain yang dipilih.

3. Daftar file yang dibuat.

4. Daftar file yang diubah.

5. Komponen reusable yang dibuat.

6. Bagian yang masih menggunakan placeholder.

7. Bagian yang siap dihubungkan ke backend.

8. Kendala yang ditemukan.

9. Rekomendasi untuk Phase 2.

Jangan berhenti di tengah pekerjaan. Selesaikan seluruh Phase 1 hingga konsisten dan siap menjadi fondasi untuk pengembangan berikutnya.




```
# Prompt: Modern Application Navbar Redesign
```
Lakukan redesign total pada Navbar Telegram Drive agar terlihat seperti aplikasi cloud storage modern, bukan website biasa.

## Tujuan

Navbar harus memberikan kesan:

- Professional
- Clean
- Modern
- Premium
- Productivity First

Gunakan inspirasi UX dari:

- Google Drive
- Dropbox
- OneDrive
- GitHub
- VS Code

Jangan menyalin desain mereka secara langsung, tetapi gunakan prinsip UX yang sama.

---

## Layout

Gunakan layout seperti ini.

---------------------------------------------------------
Telegram Drive

[ Search ............................................. ]

Home
My Files
Upload
Search
About
Help

(Login/Profile)
---------------------------------------------------------

Bukan menu yang memenuhi seluruh lebar layar.

Gunakan container dengan max-width agar lebih rapi.

---

## Brand

Logo Telegram Drive berada di kiri.

Tampilkan:

Logo

Telegram Drive

dengan typography modern.

Jika layar kecil cukup tampilkan logo + nama.

---

## Navigation

Menu:

🏠 Home

📁 My Files

☁ Upload

🔍 Search

ℹ About

❓ Help

Jangan menggunakan icon yang terlalu besar.

Gunakan icon outline yang konsisten.

---

## Active State

Halaman aktif harus jelas.

Misalnya:

Background biru muda

Text biru

Border Radius

Indicator kecil di bawah atau kiri.

---

## Hover

Hover harus halus.

Gunakan:

Transition

Background berubah sedikit

Icon ikut berubah

Cursor pointer

Tidak boleh terlalu mencolok.

---

## Search

Navbar memiliki Search Bar modern.

Placeholder:

Search files, folders, links...

Search harus menjadi elemen utama navbar.

Desktop:

Search berada di tengah.

Mobile:

Search menjadi icon yang membuka search.

---

## Right Section

Jika belum login:

🔐 Login

Jika sudah login:

Avatar

Nama User

Dropdown:

Profile

Settings

Logout

Gunakan dropdown modern.

---

## Sticky Navbar

Navbar tetap berada di atas saat halaman di-scroll.

Tambahkan sedikit blur (backdrop blur).

Background semi transparan.

Shadow tipis.

---

## Responsive

Desktop:

Logo

Search

Menu

User

Tablet:

Menu lebih ringkas.

Mobile:

Hamburger Menu.

Search menjadi icon.

Semua tetap nyaman digunakan.

---

## Visual

Gunakan:

Padding yang proporsional

Spacing konsisten

Border Radius modern

Shadow tipis

Glass effect ringan (jangan berlebihan)

Tidak menggunakan warna yang terlalu ramai.

---

## UX

Navbar harus terasa seperti aplikasi desktop modern.

Fokus pada:

Cepat

Ringan

Rapi

Profesional

Mudah digunakan.

---

## Accessibility

Pastikan:

Keyboard Navigation

ARIA Label

Focus State

Kontras warna baik.

---

## Performance

Navbar tidak boleh membuat halaman berat.

Gunakan animasi ringan.

Komponen reusable.

---

## README.md

Update README.md.

Tambahkan bagian:

Modern Navbar

Jelaskan:

Layout baru

Responsive

Sticky Navbar

Search

Active State

Dropdown User

Accessibility

---

## Penjelasan

Setelah selesai:

1. Jelaskan perubahan desain.

2. Jelaskan alasan UX yang dipilih.

3. Sebutkan file yang diubah.

4. Jelaskan bagaimana navbar ini siap untuk pengembangan fitur berikutnya.

Jangan mengubah backend, API, database, autentikasi, upload, download, service, maupun bot.

Fokus hanya pada redesign Navbar dan dokumentasi README.md.

Sebelum selesai, lakukan visual audit untuk memastikan Navbar memiliki kualitas setara aplikasi cloud storage modern dan tidak terlihat seperti template website biasa.




```

# Prompt: My Files Explorer Enhancement
```


Tingkatkan halaman My Files agar terasa seperti file explorer modern (Google Drive / Windows Explorer), tanpa mengubah backend, API, database, autentikasi, upload, download, maupun struktur routing.

Perbaiki hanya frontend.

Tambahkan:

1. View Switcher
- List View
- Grid View
- Large Grid View
- Simpan pilihan di localStorage.

2. Context Menu
Setiap folder dan file memiliki menu:
- Open
- Open in New Tab
- Details
- Rename
- Favorite
- Share
- Copy Link
- Move
- Copy
- Download
- Delete

Desktop menggunakan klik kanan.
Mobile menggunakan long press.

3. Details Panel
Gunakan side panel kanan (bukan modal) berisi:
- Nama
- Jumlah file
- Ukuran
- Created
- Updated
- Folder ID
- Telegram Channel
- Visibility
- Tags

4. Folder Navigation
Saat masuk folder:
- Breadcrumb tetap tampil.
- View Switcher tetap tersedia.
- Search tetap tersedia.
- Sort dan Filter tersedia.

5. File Explorer Feel
Gunakan spacing, hover, selected state, icon, dan animasi ringan agar terasa seperti file explorer modern.

Jangan mengubah backend, MongoDB, API, auth, upload, download, service, maupun bot.


```
```

Tugas: Perubahan terakhir menyebabkan aplikasi Next.js gagal berjalan.

Gejala:
- Browser menampilkan "missing required error components, refreshing..."
- Sebelumnya juga muncul "Cannot find module './682.js'".
- Semua route (Home, Login, My Files) ikut gagal.

Lakukan audit dan perbaikan.

Periksa:
- app/layout.tsx
- app/error.tsx
- app/global-error.tsx
- app/not-found.tsx
- template.tsx
- globals.css
- import CSS
- semua perubahan terakhir pada My Files.

Pastikan:
1. Struktur App Router Next.js valid.
2. Semua required error components tersedia.
3. Tidak ada import yang rusak.
4. Home, Login, My Files kembali normal.
5. Jangan mengubah backend, Bot Telegram, MongoDB, Repository, Service, API, Download, maupun Auth.

Setelah selesai:
- Jalankan build audit.
- Commit ke GitHub.
- Laporkan penyebab error, file yang diperbaiki, dan hash commit.



```

# Tugas: Setelah perubahan UI My Files, seluruh website menjadi rusak.
```


Tugas: Setelah perubahan UI My Files, seluruh website menjadi rusak.

Gejala:
- CSS hilang.
- Navbar berubah menjadi link HTML.
- Layout berantakan.
- Muncul lingkaran hitam besar.
- Setelah membuka My Files lalu kembali Home, Home ikut rusak.

Cari penyebabnya dan perbaiki.

Periksa:
- layout.tsx
- template.tsx
- page.tsx
- globals.css
- import CSS
- Tailwind
- React hydration
- tag HTML yang tidak tertutup
- komponen My Files yang mungkin merusak layout global
- portal/dialog yang tidak ditutup
- overflow/body style yang tertinggal
- z-index
- position fixed
- React Fragment

Pastikan:
- Home kembali normal.
- My Files tetap normal.
- Tidak ada CSS global yang berubah.
- Tidak ada perubahan backend.
- Tidak mengubah Bot Telegram.
- Tidak mengubah MongoDB.
- Tidak mengubah Upload Handler.
- Tidak mengubah Repository.
- Tidak mengubah Service.
- Tidak mengubah API.
- Tidak mengubah Download.
- Tidak mengubah Auth.

Commit ke GitHub.

Laporkan:
- Penyebab bug.
- File yang diperbaiki.
- Hash commit GitHub.


```



```


Tugas: Rapikan tampilan halaman My Files agar benar-benar terasa seperti File Explorer modern (Windows Explorer, Google Drive, OneDrive), bukan hanya daftar folder besar.

JANGAN mengubah:
- Bot Telegram
- Upload Handler
- MongoDB Connection
- Repository Layer
- Service Layer
- API Layer
- Landing Page
- Download Page
- Auth/Login
- Backend
- Routing

Fokus HANYA pada UI My Files.

Target perubahan:

1. Kecilkan tinggi setiap Folder Card sekitar 40–50%.
   - Dalam satu layar HP minimal terlihat 5–7 folder.
   - Jangan ada card yang terlalu tinggi.

2. Rapikan isi card:
   Baris 1:
   📁 Nama Folder
   Baris 2:
   Jumlah File • Total Size
   Baris 3:
   Last Updated

Contoh:

📁 Photos
48 Files • 12.3 GB
Updated 09 Jul 2026

3. Perkecil icon folder agar proporsional.

4. Perkecil tombol menu (⋮) dan letakkan sejajar dengan nama folder.

5. Tambahkan preview isi folder.
   Untuk folder Photos tampilkan 3 thumbnail kecil.
   Untuk folder Documents tampilkan icon PDF/DOC.
   Untuk Videos tampilkan preview video.
   Semua menggunakan mock data.

6. Tambahkan badge kecil apabila diperlukan:
- Shared
- Private
- Favorite
- Empty

Badge harus kecil dan elegan.

7. Tambahkan Floating Action Button (+) di kanan bawah.
Saat ditekan tampilkan Bottom Sheet:
- Upload File
- New Folder
- Import Link

Belum perlu fungsi backend.

8. Saat folder ditekan jangan pindah ke halaman kosong.
Masuk ke halaman Folder Explorer mock yang menampilkan:
- Breadcrumb
Home > Photos
- Daftar file
- Mock data
- Layout seperti File Explorer.

9. Gunakan spacing yang lebih rapat.
Target UI modern, minimalis, premium.

10. Jangan menggunakan card besar yang memakan layar.

11. Gunakan mock data saja.
Backend sama sekali tidak boleh disentuh.

12. Commit ke GitHub.

Laporan:
- File dibuat
- File diubah
- Hash Commit GitHub


```

```
Tugas: Redesign halaman My Files agar tampil seperti File Explorer modern (Windows Explorer / Google Drive), tanpa mengubah backend, API, database, Bot Telegram, Upload Handler, MongoDB, Repository Layer, Service Layer, API Layer, Landing Page, Download Page, maupun Auth/Login.

Target:

1. Hapus tampilan penuh tombol biru (Grid, List, Sort, Filter, Type, dll) dari bagian utama.

2. Bagian atas hanya berisi:
   - Search bar.
   - Tombol Upload.
   - Tombol New Folder.
   - Tombol Refresh.
   - Tombol Filter kecil (icon).
   - Tombol View (Grid/List) kecil (icon).

3. Di bawah toolbar tampilkan daftar Folder sebagai card:
   📁 Documents
   📁 Photos
   📁 Videos
   📁 Archives
   📁 Lainnya

4. Setelah folder tampilkan daftar file seperti File Explorer:
   - Icon file sesuai tipe.
   - Nama file.
   - Ukuran.
   - Upload date.
   - Folder.
   - Tombol menu (⋮).

5. Checkbox hanya muncul saat user masuk mode Select.

6. Sort, Filter, File Type dipindahkan ke popup atau drawer, jangan memenuhi halaman.

7. Layout mobile harus rapi, ringan, dan nyaman digunakan.

8. Gunakan mock data dahulu. Jangan mengambil data backend.

9. Jangan mengubah struktur routing.

10. Commit ke GitHub.

Laporkan:
- File dibuat.
- File diubah.
- Hash commit GitHub.




```
