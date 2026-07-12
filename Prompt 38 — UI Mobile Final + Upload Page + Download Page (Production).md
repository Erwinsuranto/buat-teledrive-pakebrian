







# 
```

Jangan berhenti karena dugaan blocker GitHub Actions.

Pastikan dulu penyebabnya dengan memeriksa log workflow.

Jika workflow yang bermasalah:
- perbaiki file .github/workflows jika memang ada kesalahan konfigurasi,
- rerun workflow,
- atau commit kosong untuk memicu ulang CI bila diperlukan.

Jika benar-benar karena quota GitHub Actions atau layanan GitHub sedang bermasalah:
- jangan mengubah kode aplikasi,
- jangan mengulang implementasi,
- jangan membuat audit baru,
- simpan seluruh perubahan di branch PR saat ini,
- laporkan secara singkat bukti bahwa kegagalan terjadi sebelum checkout/test sehingga bukan disebabkan kode.

Jika setelah rerun seluruh CI hijau:
- merge PR ke main,
- lanjutkan penyempurnaan UI yang masih kurang (font mobile, halaman Upload, halaman Download, dan link download).

Jangan mengulang audit repository. Fokus menyelesaikan implementasi.



```
# 
```


Roadmap backend dan audit repository sudah selesai.

JANGAN melakukan audit ulang.
JANGAN membuat laporan production-ready lagi.
JANGAN mengulang pemeriksaan GitHub Actions kecuali saat akan merge.

Fokus hanya mengimplementasikan fitur yang masih belum ada.

Daftar pekerjaan:

1. Kecilkan seluruh font mobile.
2. Perkecil card, padding, margin, bottom action.
3. Selesaikan halaman Upload dengan seluruh fitur upload.
4. Selesaikan halaman Download agar tidak membuka api.telegram.org langsung.
5. Tambahkan halaman Download lengkap (preview, metadata, tombol download, progress, counter).
6. Perbaiki seluruh UI mobile agar mirip Google Drive.
7. Jalankan test.
8. Jika CI hijau langsung merge.
9. Setelah merge langsung lanjut pekerjaan berikutnya sampai seluruh daftar di atas selesai.

Jangan berhenti setelah satu fitur.
Jangan membuat laporan audit lagi.
Laporan cukup sekali setelah seluruh pekerjaan UI selesai.


```
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
