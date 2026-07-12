# Prompt 38 — UI Mobile Final + Upload Page + Download Page (Production)
```


Lanjutkan dari main terbaru.

Jangan membuat roadmap baru.
Jangan membuat branch tambahan selain satu branch kerja.
Jangan berhenti setelah satu fitur jika masih ada pekerjaan pada prompt ini.

Target:
Menyelesaikan seluruh kekurangan UI mobile dan halaman Upload/Download agar pengalaman pengguna setara Google Drive.

WAJIB:
- Jangan menghapus fitur yang sudah ada.
- Jangan mengubah API yang sudah production jika tidak diperlukan.
- Tidak menggunakan mock.
- Semua perubahan harus lulus lint, typecheck, build, Playwright, dan GitHub Actions.
- Merge hanya jika seluruh CI hijau.

====================================================
1. MOBILE UI FINAL
====================================================

Perbaiki seluruh tampilan mobile.

Target:

- font lebih kecil
- card lebih pendek
- padding diperkecil
- margin diperkecil
- list lebih rapat
- bottom action tidak terlalu tinggi
- header lebih ringkas
- search bar lebih kecil
- chip lebih kecil
- icon proporsional
- responsive dari 320px sampai desktop

Halaman:

- Home
- My Files
- Folder
- Favorites
- Recent
- Shared
- Upload
- Download
- Detail File
- Search

====================================================
2. HALAMAN UPLOAD
====================================================

Buat halaman Upload yang benar-benar lengkap.

Fitur:

✔ pilih file

✔ pilih banyak file

✔ drag and drop desktop

✔ upload progress

✔ upload queue

✔ cancel upload

✔ retry upload

✔ pause/resume jika memungkinkan

✔ pilih folder tujuan

✔ rename sebelum upload

✔ metadata

✔ ukuran file

✔ tipe file

✔ thumbnail

✔ upload ke Telegram

✔ sukses

✔ gagal

✔ toast notification

====================================================
3. HALAMAN DOWNLOAD
====================================================

Jangan lagi membuka URL Telegram API langsung.

Saat membuka link download harus muncul halaman Download terlebih dahulu.

Halaman berisi:

Preview file

Nama file

Ukuran

Tanggal upload

Folder

Owner

Download counter

Virus status

Metadata

Share button

Copy Link

Open in Telegram

Download button besar

Progress download

Error handling

Expired handling

404 handling

====================================================
4. FILE DETAIL
====================================================

Lengkapi halaman detail.

Tambah:

Preview

Metadata

History

Owner

Folder

Favorite

Share

Copy Link

Download

Open Telegram

Move

Rename

Delete

====================================================
5. LINK DOWNLOAD
====================================================

Perbaiki seluruh link download.

Jangan membuka:

https://api.telegram.org/file/...

Secara langsung.

Harus melewati endpoint aplikasi sehingga:

permission

counter

logging

security

audit

tetap berjalan.

====================================================
6. UI POLISH
====================================================

Audit seluruh UI.

Perbaiki:

spacing

alignment

responsive

overflow

dark mode jika ada

loading skeleton

empty state

error state

toast

animation ringan

====================================================
7. TEST
====================================================

Tambahkan regression test untuk:

Upload

Download

Rename

Delete

Move

Copy

Bulk Action

Mobile

Responsive

====================================================
8. CI
====================================================

Setelah selesai:

lint

typecheck

build

API

Playwright

GitHub Actions

Semua harus hijau.

====================================================
9. GITHUB
====================================================

Buat SATU Pull Request.

Jika seluruh CI hijau:

merge ke main.

Hapus branch feature jika memungkinkan.

====================================================
10. LAPORAN
====================================================

Setelah selesai cukup laporkan:

- file yang berubah
- endpoint baru
- halaman baru
- hasil GitHub Actions
- commit merge
- status production

Jangan berhenti di tengah pekerjaan.

Jika menemukan error:
langsung perbaiki sendiri sampai CI hijau.

Baru setelah seluruh prompt ini selesai, berhenti dan menunggu instruksi berikutnya.


```
