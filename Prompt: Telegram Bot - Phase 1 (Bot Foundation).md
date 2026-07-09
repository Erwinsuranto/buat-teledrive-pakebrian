# buat-teledrive-pakebrian

```

Audit startup bot.

Masalah:
Setelah menjalankan `npm run bot`, yang muncul hanya:

[INFO] Metadata database connected.

Padahal saya ingin startup banner muncul SETELAH semua koneksi berhasil.

Urutannya harus:

🚀 Telegram Drive Bot Running
🤖 Bot : @BOT_USERNAME
📦 MongoDB : Connected ✅
📢 Channel : Connected ✅
🌐 Mode : Development
🕒 Started : waktu server

✅ Bot siap menerima upload file.

Banner hanya muncul sekali saat startup.

Jangan ubah fitur upload.
Jangan ubah database.
Jangan ubah handler.

Jika ada logger lama yang membuat banner tidak muncul, perbaiki.

Commit langsung ke GitHub.



```
```


Jangan menambah fitur baru.

Rapikan log saat bot berhasil dijalankan.

Ganti log startup menjadi lebih informatif menggunakan emoji.

Contoh:

🚀 Telegram Drive Bot Running...
🤖 Bot : @BOT_USERNAME
📦 Database : Connected ✅
📡 Telegram Channel : Ready ✅
🌐 Mode : Development
⏰ Started : Tampilkan waktu server

✅ Bot siap menerima upload file.

Jangan mengubah fitur upload, MongoDB, atau Telegram Channel.

Commit langsung ke GitHub.


```

```

# Prompt: Telegram Bot - Rapikan Pesan Upload

Jangan menambahkan fitur baru.

Rapikan UX setelah upload.

Target:

- Hapus pesan "Sedang memproses file kamu...".
- Gunakan Telegram Chat Action (typing/upload_document/upload_photo) sebagai indikator proses, bukan mengirim pesan.
- Hapus Link Download dari balasan bot.
- downloadToken tetap dibuat dan tetap disimpan di MongoDB, tetapi jangan ditampilkan ke user.
- Rapikan pesan sukses menjadi:

✅ Upload Berhasil!

🖼️ Jenis File
👤 Pengguna
📦 Ukuran
🆔 ID Singkat
🕒 Waktu Upload

✨ File berhasil disimpan di Telegram Drive.

- Jangan mengubah alur upload.
- Jangan mengubah MongoDB.
- Jangan mengubah Telegram Channel Database.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.

Commit langsung ke GitHub dan tampilkan file yang diubah.



```

```


# Prompt: Audit Core Upload Flow

Jangan menambahkan fitur baru.

Fokus hanya mengaudit alur utama Telegram Drive.

Pastikan:

- Bot menerima upload file.
- File berhasil dikirim ke Telegram Channel Database.
- Metadata berhasil disimpan ke MongoDB.
- Jika salah satu langkah gagal, tampilkan error yang jelas.
- Pastikan tidak ada bug pada alur upload.
- Rapikan kode jika diperlukan tanpa mengubah fitur.
- Build project harus berhasil tanpa error.

Jangan membuat website.
Jangan membuat dokumentasi baru.
Jangan membuat fitur tambahan.

Commit hasil audit ke GitHub dan tampilkan file yang diubah.


```
```

# Prompt: Telegram Bot - Phase 11 (Share Download Link)

Lanjutkan pengembangan Telegram Bot.

Fokus hanya pada pembuatan link download.

Target:

- Setelah upload berhasil, bot mengirim pesan:
  ✅ File berhasil disimpan.

  🔗 Link Download:
  https://t.me/<BOT_USERNAME>?start=<downloadToken>

- BOT_USERNAME diambil otomatis dari konfigurasi bot.
- Pastikan link menggunakan downloadToken yang sudah ada, jangan membuat token baru.
- Saat link dibuka, bot langsung memproses token yang sudah dibuat sebelumnya.
- Jangan mengubah sistem upload.
- Jangan mengubah MongoDB.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.
- Commit langsung ke GitHub dan tampilkan file yang diubah.



```
```

# Prompt: Telegram Bot - Phase 10 (Download Link)

Lanjutkan pengembangan Telegram Bot.

Fokus hanya pada fitur Download Link.

Target:

- Setelah upload berhasil, buat downloadToken unik untuk setiap file.
- Simpan downloadToken bersama metadata di MongoDB.
- Tambahkan command /start <downloadToken>.
- Jika token valid, bot mengambil metadata dari MongoDB lalu mengirim kembali file dari Telegram Channel Database ke user.
- Jika token tidak valid, tampilkan pesan:
❌ Link tidak valid atau sudah tidak tersedia.
- Gunakan satu downloadToken yang nantinya juga akan dipakai oleh website, jangan membuat sistem token terpisah.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.
- Jangan mengubah fitur upload, My Files, atau Search yang sudah berjalan.
- Commit langsung ke GitHub dan tampilkan file yang diubah.



```
```

# Prompt: Telegram Bot - Phase 9 (Search Files)

Lanjutkan pengembangan Telegram Bot.

Fokus hanya pada fitur Search.

Target:

- Saat pengguna menekan 🔍 Search, bot meminta kata kunci.
- Cari file milik user sendiri di MongoDB berdasarkan nama file.
- Pencarian tidak membedakan huruf besar/kecil.
- Tampilkan maksimal 10 hasil.
- Jika tidak ada hasil tampilkan:
  ❌ File tidak ditemukan.
- Jika ada hasil tampilkan:
  📄 Nama File
  📦 Ukuran
  📅 Tanggal Upload
- Setelah hasil ditampilkan, tampilkan kembali menu utama.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.
- Jangan membuat link download dulu.
- Commit langsung ke GitHub dan tampilkan file yang diubah.



```

```

# Prompt: Telegram Bot - Phase 8 (My Files)

Lanjutkan pengembangan Telegram Bot.

Fokus hanya membuat fitur My Files.

Target:

- Saat pengguna menekan tombol 📁 My Files, tampilkan daftar file milik user dari MongoDB.
- Hanya tampilkan file milik user tersebut.
- Urutkan dari upload terbaru.
- Maksimal tampilkan 10 file per halaman.
- Jika file belum ada, tampilkan:
  📂 Kamu belum memiliki file.
  Silakan upload file terlebih dahulu.
- Tampilkan nama file, ukuran, dan tanggal upload.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.
- Jangan membuat link download dulu.
- Commit langsung ke GitHub dan tampilkan file yang diubah.



```

```
# Prompt: Telegram Bot - Phase 7 (Metadata Database)

Lanjutkan pengembangan Telegram Bot.

Fokus hanya pada metadata database.

Target:
- Setelah file berhasil dikirim ke Telegram Channel Database, simpan metadata ke database.
- Simpan minimal:
  - user_id
  - message_id
  - file_id
  - file_unique_id
  - file_name
  - file_size
  - file_type
  - upload_date
- Gunakan struktur yang mudah dikembangkan.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.
- Jangan membuat fitur Search atau My Files dulu.
- Commit langsung ke GitHub dan tampilkan file yang diubah.




```
```

# Prompt: Telegram Bot - Phase 6 (Fallback & Conversation Flow)

Lanjutkan pengembangan Telegram Bot.

Jangan membuat website.

Jangan membuat README, docs, roadmap, atau file markdown baru.

Jangan mengubah fitur upload yang sudah berjalan.

Fokus pada alur percakapan bot.

Target Phase 6:

- Tambahkan handler untuk semua pesan yang tidak dikenali.
- Jika pengguna mengirim teks yang bukan command atau menu, balas dengan pesan yang ramah.

Contoh:

🤔 Maaf, saya tidak mengerti perintah tersebut.

Silakan gunakan menu di bawah atau ketik /start untuk kembali ke menu utama.

- Jika pengguna menekan tombol keyboard, arahkan ke handler yang sesuai.
- Setelah setiap aksi selesai, tampilkan kembali menu utama agar pengguna tidak bingung.
- Tambahkan command /cancel untuk membatalkan proses yang sedang berjalan.
- Jika pengguna mengirim file saat bot tidak sedang menunggu upload, berikan petunjuk yang jelas.
- Rapikan seluruh pesan agar konsisten menggunakan emoji.
- Simpan seluruh teks pada file konfigurasi messages.ts yang sudah ada, jangan membuat file konfigurasi baru.
- Jangan membuat database.
- Jangan membuat website.
- Jangan membuat link download.
- Jangan membuat dokumentasi baru.
- Usahakan perubahan file seminimal mungkin.

Pastikan project build tanpa error.

Commit langsung ke repository GitHub dan tampilkan daftar file yang dibuat atau diubah.



```

```
# Prompt: Telegram Bot - Phase 5 (Upload Validation & User Experience)

Lanjutkan pengembangan Telegram Bot.

Jangan membuat website.

Jangan membuat README, docs, roadmap, atau file markdown baru.

Fokus hanya pada validasi upload dan pengalaman pengguna.

Target Phase 5:

- Tambahkan batas maksimal ukuran file melalui konfigurasi .env.
- Validasi tipe file yang didukung.
- Jika file terlalu besar, tampilkan pesan yang ramah beserta emoji.
- Saat proses upload tampilkan status seperti:
  ⏳ Sedang memproses...
- Setelah berhasil:
  ✅ File berhasil disimpan.
- Jika gagal:
  ❌ Upload gagal.
  Sertakan alasan yang mudah dipahami.
- Tambahkan logging yang lebih jelas.
- Jangan mengubah fitur upload yang sudah berjalan.
- Jangan membuat database.
- Jangan membuat website.
- Jangan membuat link download.
- Jangan membuat dokumentasi baru.

Usahakan perubahan file seminimal mungkin.

Pastikan project build tanpa error.

Commit langsung ke repository GitHub dan tampilkan daftar file yang dibuat atau diubah.




```
```

# Prompt: Telegram Bot - Phase 4 (Start Menu & User Experience)

Lanjutkan pengembangan Telegram Bot.

Jangan membuat website.

Jangan membuat README, docs, roadmap, atau file markdown baru.

Jangan mengubah fitur upload yang sudah selesai.

Fokus pada pengalaman pengguna (UX) bot.

Target Phase 4:

- Perbarui command /start menjadi lebih menarik menggunakan emoji.
- Tambahkan ucapan selamat datang yang rapi.
- Gunakan HTML parse mode agar teks lebih menarik.
- Tambahkan Reply Keyboard (bukan Inline Keyboard).

Menu yang ditampilkan:

📤 Upload File
📁 My Files
🔍 Search
❓ Bantuan
⚙️ Tentang Bot

Jika pengguna menekan salah satu menu, bot harus memberikan respon yang sesuai (sementara boleh berupa placeholder kecuali Upload File).

Contoh pesan /start:

👋 Halo, <nama pengguna>!

Selamat datang di <b>Telegram Drive</b>.

☁️ Simpan file dengan mudah.
⚡ Upload cepat.
🔗 Link download akan dibuat otomatis.
📂 Semua file tersimpan dengan aman di Telegram.

Silakan pilih menu di bawah.

Tambahkan emoji pada semua pesan agar terlihat modern tetapi tidak berlebihan.

Gunakan satu file khusus untuk konfigurasi semua teks agar nanti mudah diterjemahkan atau diubah.

Jangan membuat database.
Jangan membuat website.
Jangan membuat link download.
Jangan membuat dokumentasi baru.

Pastikan build berhasil tanpa error.

Commit langsung ke repository GitHub dan tampilkan daftar file yang dibuat atau diubah.



```


```


# Prompt: Telegram Bot - Phase 3 (Save Uploaded Files to Telegram Channel)

Lanjutkan pengembangan Telegram Bot.

Jangan membuat website.

Jangan membuat README, docs, roadmap, atau file markdown baru.

Jangan menambahkan fitur yang tidak diminta.

Fokus hanya pada fitur berikut.

Target Phase 3:

- Setelah pengguna mengirim file (document, photo, video, audio, voice), bot harus langsung meneruskan atau mengirim file tersebut ke Telegram Channel Database yang ID-nya diambil dari file .env.
- Simpan informasi penting dari hasil upload seperti:
  - message_id
  - file_id
  - file_unique_id
  - jenis file
  - nama file (jika ada)
  - ukuran file
- Belum menggunakan database permanen. Cukup siapkan struktur agar nanti mudah dihubungkan ke database.
- Tambahkan validasi jika CHANNEL_ID atau BOT_TOKEN belum diatur.
- Tambahkan logging yang jelas jika upload berhasil atau gagal.
- Jangan membuat link download dulu.
- Jangan membuat fitur pencarian.
- Jangan membuat My Files.
- Jangan membuat website.
- Jangan membuat dokumentasi baru.

Usahakan perubahan file seminimal mungkin dan gunakan struktur project yang sudah ada.

Sebelum commit, pastikan project build tanpa error.

Commit langsung ke repository GitHub dan tampilkan daftar file yang dibuat atau diubah.


```
```

# Prompt: Telegram Bot - Phase 2 (Upload File Foundation)

Lanjutkan pengembangan Telegram Bot.

Jangan membuat website.

Jangan membuat README atau file dokumentasi baru.

Jangan membuat docs baru.

Fokus hanya pada implementasi bot.

Target Phase 2:

- Tambahkan handler upload file.
- Bot harus dapat menerima:
  - Document
  - Photo
  - Video
  - Audio
  - Voice
- Pisahkan handler sesuai struktur project.
- Buat konfigurasi yang mudah dikembangkan.
- Jangan implementasi database dulu.
- Jangan implementasi website.
- Jangan implementasi download link dulu.
- Jangan mengubah struktur project yang sudah ada jika tidak diperlukan.
- Jangan membuat file yang tidak diperlukan.

Jika ada file yang perlu ditambah, buat seminimal mungkin.

Setelah selesai:

- Pastikan project berhasil build tanpa error.
- Commit langsung ke repository GitHub.
- Tampilkan daftar file yang dibuat atau diubah.



```
```
Buat pondasi Telegram Bot langsung di repository GitHub yang sudah terhubung.

Jangan membuat website dulu.

Fokus hanya pada Telegram Bot.

Target Phase 1:

- Pastikan project dapat dijalankan tanpa error.
- Konfigurasi Telegram Bot menggunakan Telegraf.
- Buat struktur folder bot yang rapi.
- Tambahkan konfigurasi .env.example.
- Tambahkan command:
/start
/help
/ping

Command /ping harus membalas "Bot Online ✅".

Pisahkan kode menjadi beberapa file agar mudah dikembangkan.

Jangan membuat fitur upload, database, atau download terlebih dahulu.

Semua file dibuat langsung di repository GitHub, bukan hanya ditampilkan di chat.

Setelah selesai, commit seluruh perubahan dan tampilkan daftar file yang dibuat atau diubah.




```
