# buat-teledrive-pakebrian


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
