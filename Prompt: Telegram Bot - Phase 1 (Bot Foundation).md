# buat-teledrive-pakebrian

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
