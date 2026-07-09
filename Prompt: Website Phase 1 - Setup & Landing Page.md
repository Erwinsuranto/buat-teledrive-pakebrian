# Prompt website 
```

# Prompt: Website Architecture Preparation

Lanjutkan pengembangan website Telegram Drive.

PENTING:
- Jangan mengubah Bot Telegram.
- Jangan mengubah Upload Handler.
- Jangan mengubah MongoDB.
- Jangan mengubah API.
- Jangan membuat Download Page.
- Jangan membuat Auth/Login.
- Jangan membuat business logic.
- Jangan membuat koneksi database.

Fokus hanya merapikan struktur arsitektur frontend agar siap dihubungkan ke backend nanti.

Lakukan hal berikut:

1. Audit seluruh folder project frontend.

2. Rapikan struktur folder menjadi konsisten.

3. Buat folder yang diperlukan untuk tahap backend berikutnya, misalnya:
- services/
- hooks/
- lib/
- providers/
- types/
- constants/
- utils/

4. Semua folder cukup berisi placeholder bila belum dipakai.

5. Pisahkan reusable components bila masih ada yang tercampur.

6. Pastikan import path tetap rapi.

7. Hapus kode duplikat bila ada.

8. Rapikan penamaan file dan component agar konsisten.

9. Pastikan project tetap build tanpa error.

10. Jangan mengubah tampilan UI yang sudah selesai.

11. Jangan membuat endpoint.

12. Jangan membuat fetch.

13. Jangan membuat API.

14. Jangan membuat database query.

15. Jangan membuat halaman Download.

16. Jangan mengubah Bot Telegram sama sekali.

## Setelah selesai

1. Commit langsung ke GitHub.

2. Update README.md yang sudah ada (WAJIB):
- Jangan membuat README.md baru.
- Jangan menghapus isi README.md lama.
- Jangan membuat file dokumentasi lain.
- Tambahkan Development Log baru di bagian PALING BAWAH README.md.

Format:

### DD MMM YYYY - HH:mm WIB

Perubahan:
- ...

File dibuat:
- ...

File diubah:
- ...

Commit:
- xxxxxxx

3. Laporkan:
- File dibuat
- File diubah
- Hash Commit GitHub
- Pastikan Bot Telegram, Upload Handler, MongoDB, API, Download Page, dan Auth/Login tidak disentuh.



```

```

# Prompt: Website Design System

Lanjutkan pengembangan website Telegram Drive.

PENTING:
- Jangan mengubah Bot Telegram.
- Jangan mengubah Upload Handler.
- Jangan mengubah MongoDB.
- Jangan mengubah API.
- Jangan membuat Download Page.
- Jangan membuat Auth/Login.
- Jangan menghubungkan database.
- Fokus hanya membangun Design System dan reusable UI components.

Gunakan Next.js App Router + Tailwind CSS.

Buat Design System yang akan dipakai seluruh website.

Buat reusable components untuk:

- Button
- Input
- Search Box
- Select
- Badge
- Card
- Modal
- Dialog
- Dropdown Menu
- Tooltip
- Toast
- Tabs
- Pagination
- Breadcrumb
- Empty State
- Loading Skeleton
- Avatar
- Status Badge
- File Icon Component
- File Type Badge
- Theme Container
- Section Header

Semua component dipisahkan ke folder components/ui.

Gunakan style yang konsisten:

- Modern
- Minimalis
- Rounded
- Smooth animation
- Mobile First
- Responsive
- Clean spacing

Semua halaman yang sudah dibuat (Landing Page, Dashboard, Files, Uploads, Users, Settings, Help, About) gunakan component baru ini agar tampilannya konsisten.

Jangan menambahkan backend.

Jangan membuat API.

Jangan membuat database.

Jangan membuat business logic.

Fokus hanya pada UI dan reusable components.

Pastikan project tetap build tanpa error.

## Setelah selesai

1. Commit langsung ke GitHub.

2. Update README.md yang sudah ada (WAJIB):
- Jangan membuat README.md baru.
- Jangan menghapus isi README.md lama.
- Jangan membuat file dokumentasi lain.
- Tambahkan Development Log baru di bagian paling bawah README.md.

Format Development Log:

### DD MMM YYYY - HH:mm WIB

Perubahan:
- ...

File dibuat:
- ...

File diubah:
- ...

Commit:
- xxxxxxx

3. Setelah selesai laporkan:
- File yang dibuat.
- File yang diubah.
- Hash Commit GitHub.
- Pastikan Bot Telegram, Upload Handler, MongoDB, API, Download Page, dan Auth/Login tidak disentuh.



```

```


# Prompt: UI File Manager

Lanjutkan pengembangan website Telegram Drive.

PENTING:
- Jangan mengubah Bot Telegram.
- Jangan mengubah Upload Handler.
- Jangan mengubah MongoDB.
- Jangan mengubah API.
- Jangan membuat Download Page.
- Jangan membuat Auth/Login.
- Jangan menghubungkan database.
- Fokus hanya membuat UI halaman File Manager.

Gunakan Next.js App Router + Tailwind CSS.

Perbaiki halaman /files agar menjadi File Manager modern.

Tambahkan:

- Header halaman
- Search Bar (UI saja)
- Filter Button (UI saja)
- Sort Button (UI saja)
- Toggle Grid/List View
- File Card
- File List View
- Folder Card
- Empty State
- Loading Skeleton
- Pagination Component (dummy)
- Breadcrumb
- Responsive Mobile
- Context Menu UI (Rename, Move, Delete, Share) sebagai placeholder tanpa fungsi
- Floating Upload Button (UI saja)

Setiap File Card tampilkan dummy:

- Thumbnail
- Nama File
- Jenis File
- Ukuran
- Tanggal Upload
- Icon File

Semua data menggunakan dummy data.

Jangan membuat fetch API.

Jangan membuat database query.

Jangan membuat business logic.

Jangan membuat halaman Download.

Gunakan reusable components.

Pastikan halaman dapat dibuka tanpa error.

## Setelah selesai

1. Commit langsung ke GitHub.

2. Update README.md yang sudah ada (WAJIB):
- Jangan membuat README.md baru.
- Jangan menghapus isi README.md lama.
- Jangan membuat file dokumentasi lain.
- Tambahkan Development Log baru di bagian paling bawah README.md.

Format Development Log wajib:

### DD MMM YYYY - HH:mm WIB

Perubahan:
- ...

File dibuat:
- ...

File diubah:
- ...

Commit:
- xxxxxxx

3. Setelah selesai laporkan:
- File yang dibuat.
- File yang diubah.
- Hash Commit GitHub.
- Pastikan Bot Telegram, Upload Handler, MongoDB, API, Download Page, dan Auth/Login tidak disentuh.


```
```

# Prompt: Website Admin Dashboard Layout

Lanjutkan pengembangan website Telegram Drive.

PENTING:
- Jangan mengubah Bot Telegram.
- Jangan mengubah Upload Handler.
- Jangan mengubah MongoDB.
- Jangan mengubah API.
- Jangan membuat Download Page.
- Jangan membuat Auth/Login.
- Jangan menghubungkan database.
- Fokus hanya membuat struktur UI Dashboard Admin.

Gunakan Next.js App Router + Tailwind CSS.

Buat struktur halaman berikut:

- /dashboard
- /files
- /uploads
- /users
- /settings

Semua halaman masih berupa placeholder tetapi menggunakan layout yang sama.

Dashboard harus memiliki:

- Sidebar modern
- Top Navbar
- Breadcrumb
- Responsive Mobile
- Card Component
- Table Component
- Empty State Component
- Loading Skeleton Component
- Modal Component
- Confirm Dialog Component

Semua component dipisahkan ke folder components agar reusable.

Gunakan desain modern, bersih, konsisten dengan identitas Telegram Drive.

Belum boleh ada:
- Fetch API
- Database
- Business Logic
- Download Page
- Auth/Login

Pastikan semua route dapat dibuka tanpa error.

## Setelah selesai

1. Commit langsung ke GitHub.

2. Update README.md yang sudah ada (WAJIB):
- Jangan membuat README.md baru.
- Jangan menghapus isi README.md lama.
- Jangan membuat file dokumentasi lain.
- Tambahkan Development Log baru di bagian PALING BAWAH README.md.

Format Development Log wajib seperti berikut:

## Development Log

### DD MMM YYYY - HH:mm WIB

Contoh:

### 09 Jul 2026 - 22:35 WIB

Perubahan:
- Dashboard UI dibuat.
- Sidebar dibuat.
- Navbar dibuat.
- Breadcrumb dibuat.
- Card Placeholder dibuat.
- Table Placeholder dibuat.
- Loading Skeleton dibuat.
- Empty State dibuat.
- Component dipisahkan agar reusable.

File dibuat:
- ...

File diubah:
- ...

Commit:
- xxxxxxx

3. Setelah selesai laporkan:
- File yang dibuat.
- File yang diubah.
- Hash Commit GitHub.
- Pastikan Bot Telegram, Upload Handler, MongoDB, API, Download Page, dan Auth/Login tidak disentuh.



```

```


Lanjutkan pengembangan website Telegram Drive.

PENTING:
- Jangan mengubah kode Bot Telegram.
- Jangan mengubah Upload Handler.
- Jangan mengubah MongoDB Schema.
- Jangan mengubah API.
- Jangan membuat Download Page.
- Jangan membuat autentikasi/login.
- Fokus hanya pada struktur Dashboard UI.

Buat Dashboard dengan layout modern menggunakan Next.js + Tailwind.

Sidebar:
- Dashboard
- My Files
- Search
- Upload
- Bantuan
- Tentang

Header:
- Logo Telegram Drive
- Judul halaman
- Placeholder User Menu

Halaman Dashboard:
- Welcome Card
- Total Files (placeholder)
- Total Storage (placeholder)
- Recent Files (placeholder)
- Recent Activity (placeholder)

Semua data masih dummy/placeholder.
Jangan ada fetch API.
Jangan ada koneksi database.

Gunakan component terpisah agar mudah dikembangkan nanti.

Setelah selesai:
- Commit langsung ke GitHub.
- Tambahkan Development Log baru di bagian paling bawah README.md.
- Jangan menghapus isi README.md lama.
- Jangan membuat README.md baru.
- Jangan membuat file dokumentasi lain.
- Laporkan file yang dibuat, file yang diubah, dan hash commit.


```
```

Nama Prompt: Website Phase 4 - Dashboard UI

Tambahkan fitur berikut ke project Telegram Drive.

ATURAN WAJIB

1. Fokus hanya mengerjakan fitur yang diminta.
2. Jangan mengubah Bot Telegram.
3. Jangan mengubah sistem Upload Telegram Channel.
4. Jangan mengubah MongoDB.
5. Jangan membuat API.
6. Jangan membuat autentikasi.
7. Jangan membuat Download Page.
8. Jangan membuat fitur tambahan di luar permintaan.
9. Jangan membuat README.md baru.
10. Gunakan hanya SATU README.md yang sudah ada.
11. Jangan menghapus isi README.md yang lama.
12. Setelah fitur selesai, tambahkan ringkasan perubahan di bagian paling bawah README.md pada section "Development Log".
13. Jika "Development Log" belum ada, buat hanya SATU kali.
14. Tambahkan log baru, jangan menghapus log sebelumnya.
15. Jangan membuat docs/, roadmap.md, architecture.md, changelog.md, notes.md, atau file markdown lainnya.
16. Gunakan struktur project yang sudah ada.
17. Jika membuat file baru, buat seminimal mungkin.
18. Pastikan project tetap build tanpa error.
19. Commit langsung ke GitHub.
20. Tampilkan daftar file yang dibuat atau diubah.
21. Jangan menghapus kode yang sudah berjalan.

FITUR YANG HARUS DIBUAT

Buat Dashboard UI Telegram Drive.

Sidebar:
🏠 Dashboard
📁 My Files
📤 Upload
🔍 Search
⚙️ Settings
🚪 Logout

Dashboard berisi:

- 📦 Total Files
- 💾 Total Storage
- 📥 Total Downloads
- 📅 Last Upload

Tambahkan:

- Recent Files (placeholder)
- Recent Activity (placeholder)

Gunakan:

- Telegram Blue Theme
- Clean UI
- Modern
- Responsive
- Mobile First
- Rounded Card
- Soft Shadow
- Smooth Animation

Gunakan data dummy (placeholder).

Jangan mengambil data dari MongoDB.

Jangan membuat backend.

Jangan membuat API.

Jangan membuat Download Page.

Jangan membuat Login System.

Fokus hanya membuat tampilan Dashboard yang nantinya akan dihubungkan ke backend.

README.md

Setelah selesai, tambahkan Development Log seperti contoh berikut tanpa menghapus log lama:

## YYYY-MM-DD
### Website Phase 4 - Dashboard UI

- Dashboard UI dibuat.
- Sidebar dibuat.
- Statistik placeholder ditambahkan.
- Recent Files placeholder ditambahkan.
- Recent Activity placeholder ditambahkan.

Commit langsung ke GitHub setelah selesai.



```

```

Nama Prompt: Website Phase 3 - Website Structure

Tambahkan fitur berikut ke project Telegram Drive.

ATURAN WAJIB

1. Fokus hanya mengerjakan fitur yang diminta.
2. Jangan mengubah Bot Telegram.
3. Jangan mengubah Upload Telegram Channel.
4. Jangan mengubah MongoDB.
5. Jangan membuat API.
6. Jangan membuat database baru.
7. Jangan membuat README.md baru.
8. Gunakan hanya README.md yang sudah ada jika memang perlu.
9. Jangan membuat docs, markdown, roadmap baru.
10. Gunakan struktur project yang sudah ada.
11. Jika membuat file baru, buat seperlunya.
12. Pastikan project tetap build tanpa error.
13. Commit langsung ke GitHub.
14. Tampilkan daftar file yang dibuat atau diubah.
15. Jangan menghapus kode yang sudah berjalan.

FITUR YANG HARUS DIBUAT

Buat struktur halaman website menggunakan App Router Next.js.

Tambahkan halaman berikut:

🏠 Home
📁 My Files
📤 Upload
🔍 Search
ℹ️ About
❓ Help
🔐 Login

Semua halaman cukup berupa placeholder dengan layout yang sama.

Setiap halaman cukup memiliki:

- Judul halaman
- Icon
- Deskripsi singkat
- Tombol kembali ke Home

Gunakan Header dan Footer yang sudah dibuat.

Jangan membuat Dashboard.

Jangan membuat Download Page.

Jangan membuat API.

Jangan menghubungkan MongoDB.

Jangan mengambil data apa pun.

Jangan membuat autentikasi.

Fokus hanya membuat struktur halaman agar routing website sudah lengkap.



```

```

Nama Prompt: Website Phase 2 - Website Layout

Tambahkan fitur berikut ke project Telegram Drive.

ATURAN WAJIB

1. Fokus hanya mengerjakan fitur yang diminta.
2. Jangan mengubah bot Telegram yang sudah berjalan.
3. Jangan mengubah upload Telegram Channel.
4. Jangan mengubah MongoDB schema.
5. Jangan membuat fitur tambahan.
6. Jangan membuat README.md baru.
7. Gunakan hanya README.md yang sudah ada bila memang perlu diperbarui.
8. Jangan membuat docs, roadmap, markdown baru.
9. Gunakan struktur project yang sudah ada.
10. Jika membuat file baru, buat seminimal mungkin.
11. Pastikan project tetap build tanpa error.
12. Commit langsung ke GitHub.
13. Tampilkan daftar file yang dibuat atau diubah.
14. Jangan menghapus kode yang sudah berjalan.

FITUR YANG HARUS DIBUAT

Buat layout website yang akan dipakai seluruh halaman.

Tambahkan:

- Header
- Logo Telegram Drive
- Menu Desktop
- Menu Mobile (hamburger)
- Footer
- Responsive Layout
- Container Layout
- Theme warna Telegram

Menu Header:

🏠 Home
📁 My Files
📤 Upload
ℹ️ Tentang
❓ Bantuan

Footer:

Telegram Drive

Version

Copyright

Responsive untuk HP, Tablet, Desktop.

Jangan membuat Login.

Jangan membuat Dashboard.

Jangan membuat Download Page.

Jangan membuat API.

Jangan menghubungkan MongoDB.

Jangan mengambil data apa pun.

Fokus hanya membuat layout website yang akan dipakai seluruh project.



```
```

Nama Prompt: Website Phase 1 - Setup & Landing Page

Tambahkan fitur berikut ke project Telegram Drive.

ATURAN WAJIB

1. Fokus hanya mengerjakan fitur yang diminta.
2. Jangan mengubah fitur bot Telegram yang sudah berjalan.
3. Jangan mengubah sistem upload Telegram Channel.
4. Jangan mengubah MongoDB schema yang sudah ada.
5. Jangan membuat fitur tambahan di luar permintaan.
6. Jangan membuat README.md baru.
7. Gunakan hanya SATU README.md yang sudah ada apabila memang perlu diperbarui.
8. Jangan membuat docs, roadmap, architecture, markdown baru tanpa diminta.
9. Gunakan struktur project yang sudah ada.
10. Jika perlu membuat file baru, buat seminimal mungkin.
11. Pastikan project tetap bisa build tanpa error.
12. Commit langsung ke GitHub setelah selesai.
13. Tampilkan daftar file yang dibuat atau diubah.
14. Jangan menghapus kode yang sudah berjalan.

FITUR YANG HARUS DIBUAT

Buat pondasi website Telegram Drive menggunakan Next.js yang sudah ada.

Landing Page berisi:

• Logo Telegram Drive
• Nama Telegram Drive
• Deskripsi singkat:
  "Simpan file ke Telegram dengan mudah dan akses kapan saja."

• Tombol:
- Login
- Upload
- Download

Navigation:

- Home
- Tentang
- Bantuan

Footer:

- Telegram Drive
- Copyright
- Version

Gunakan warna:

Primary :
Telegram Blue

Background :
Putih

Card :
Putih

Button :
Telegram Blue

Design:

- Modern
- Minimalis
- Responsive
- Mobile First
- Tidak menggunakan template admin
- Animasi ringan
- Rounded Card
- Shadow lembut

Jangan membuat halaman Dashboard dahulu.

Jangan membuat Login dahulu.

Jangan membuat Download Page dahulu.

Fokus hanya membuat pondasi website dan Landing Page.



```
