





# 
```

Lanjutkan.

Jangan kirim wrapper page.

Kirim file implementasi sebenarnya:

components/final-ui/upload-studio.tsx

atau file yang berisi UploadStudio.

Saya ingin seluruh isi source code lengkap, bukan page wrapper.



```
# 
```
STOP.

Jangan membuat audit, ringkasan, atau laporan.

Saya ingin memverifikasi implementasi yang Anda klaim sudah selesai.

Kirim SELURUH source code yang Anda buat untuk fitur Upload dan Download.

Sertakan:

1. Semua file halaman Upload.
2. Semua file halaman Download.
3. Semua komponen React yang digunakan.
4. Semua API route yang dibuat atau diubah.
5. Semua helper/service untuk upload ke Telegram.
6. Semua perubahan routing.
7. Sebutkan path lengkap setiap file.

Contoh:

app/upload/page.tsx
app/download/[id]/page.tsx
components/upload/UploadForm.tsx
components/download/DownloadPreview.tsx
lib/telegram.ts
app/api/upload/route.ts
app/api/download/[id]/route.ts

Jika file terlalu panjang, kirim satu file penuh per balasan sampai seluruh implementasi selesai.

Jangan ringkas.
Jangan hanya menyebut nama file.
Jangan mengatakan "sudah ada di repository".
Saya ingin melihat isi source code lengkap untuk setiap file yang Anda ubah.




```
# Prompt 39 – Complete Mobile Upload & Download UI (No Audit Until Finished)
```



Lanjutkan pekerjaan dari PR #38.

JANGAN membuat audit repository lagi.
JANGAN membuat laporan progress lagi.
JANGAN membuat laporan production-ready lagi.
JANGAN membuat PR baru setiap fitur kecil.
JANGAN berhenti setelah satu fitur selesai.

Fokus hanya menyelesaikan implementasi UI dan functionality sampai benar-benar selesai.

Target:

========================
1. Upload Page
========================

Buat halaman Upload lengkap.

Harus memiliki:

- Choose File
- Upload Button
- Drag & Drop
- Mobile File Picker
- Multiple Upload
- Folder Upload jika browser mendukung
- Progress Bar
- Upload Speed
- Remaining Time
- Cancel Upload
- Retry Upload
- Pause Resume
- Success Notification
- Error Notification
- Preview Image
- Preview Video
- Preview PDF
- File Information
- Upload Queue
- Recent Uploads

Upload harus langsung menggunakan API Telegram Drive yang sudah ada.

========================
2. Download Page
========================

Buat halaman Download lengkap.

Harus memiliki:

- File Preview
- Thumbnail
- File Metadata
- Download Button
- Download Progress
- Remaining Time
- Retry
- Resume
- Copy Link
- Share
- QR Code
- Related Files
- Recent Downloads

========================
3. Mobile UI
========================

Perbaiki seluruh UI mobile.

Font terlalu besar.

Gunakan ukuran yang nyaman seperti Google Drive.

Kurangi whitespace.

Perkecil:

- Header
- Card
- Button
- Menu
- List
- Dialog
- Search
- Metadata

Semua harus nyaman digunakan pada layar HP.

========================
4. Navigation
========================

Pastikan menu:

Home
My Files
Upload
Download
Favorites
Recent
Trash
Settings

berfungsi.

========================
5. Responsive
========================

Pastikan tampil baik pada:

Android
iPhone
Tablet
Desktop

========================
6. API
========================

Gunakan API yang sudah ada.

Jangan membuat API baru jika endpoint lama masih bisa dipakai.

========================
7. Git
========================

Kerjakan seluruh implementasi dalam branch PR #38.

Jangan membuat PR baru.

Merge hanya jika:

- seluruh UI Upload selesai
- seluruh UI Download selesai
- responsive selesai
- tidak ada placeholder
- tidak ada halaman kosong

========================
8. Output
========================

Jangan membuat laporan panjang.

Jangan audit lagi.

Jangan menjelaskan setiap perubahan.

Kerjakan terus sampai seluruh fitur Upload dan Download selesai.

Jika ada GitHub Actions gagal karena billing atau runner GitHub, hentikan hanya proses CI.

Tetap lanjutkan implementasi source code.

Yang penting seluruh kode selesai terlebih dahulu.

Laporan cukup satu kali setelah semua fitur selesai.

```
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
