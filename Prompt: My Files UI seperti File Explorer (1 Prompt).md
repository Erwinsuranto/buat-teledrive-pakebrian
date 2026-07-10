# Prompt: My Files UI Premium (Compact File Explorer)
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
