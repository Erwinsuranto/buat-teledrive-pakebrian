# Prompt: Phase 2.3.1 – Compatibility Layer & Telegram Service Foundation



```
Phase 2.3.1 dimulai.

Sebelum menghubungkan Telegram API asli, bangun fondasi Telegram Service menggunakan Compatibility Layer agar transisi dari arsitektur lama ke arsitektur baru berjalan aman.

Tujuan:
Mempersiapkan seluruh struktur Telegram Service sehingga implementasi Telegram Client nantinya hanya tinggal menghubungkan adapter tanpa mengubah Service, Repository, atau UI.

Kerjakan:

1. Audit kembali seluruh hasil Phase 2.1 sampai Phase 2.2.8.
2. Pastikan seluruh Repository baru menjadi satu-satunya jalur akses data.
3. Buat Compatibility Contract untuk Telegram Service.
4. Buat Telegram Adapter Interface.
5. Buat Telegram Service Interface.
6. Buat placeholder implementation yang masih menggunakan mock/fake adapter.
7. Hubungkan Composition Root dengan adapter baru.
8. Pastikan dependency hanya mengarah ke Interface, bukan implementation.
9. Pastikan tidak ada import langsung MongoDB atau Mongoose dari Telegram Service.
10. Siapkan struktur agar nantinya mudah mengganti Mock Adapter menjadi Telegram Client asli.

Yang harus disiapkan:

- TelegramService Interface
- TelegramAdapter Interface
- TelegramSession Contract
- Upload Contract
- Download Contract
- Delete Contract
- Forward Contract
- File Metadata Contract
- Message Mapping Contract
- Error Contract
- Retry Contract
- Health Check Contract

Tambahkan folder bila diperlukan, misalnya:

backend/
 └── src/
      ├── telegram/
      │     ├── contracts/
      │     ├── adapters/
      │     ├── services/
      │     ├── mapper/
      │     ├── dto/
      │     ├── errors/
      │     └── index.ts

Gunakan Dependency Injection yang sudah dibuat pada Phase 2.2.

Jangan:

- Menghubungkan Telegram API.
- Menggunakan MTProto.
- Menggunakan Bot API.
- Membuat upload file sungguhan.
- Membuat download sungguhan.
- Mengubah UI.
- Mengubah API.
- Mengubah Business Logic.
- Menghapus compatibility layer lama.

Update README.md dengan:

- Telegram Service Architecture
- Compatibility Layer
- Adapter Pattern
- Dependency Flow
- Progress Phase 2.3.1

Di akhir pekerjaan berikan laporan:

1. Ringkasan implementasi.
2. File yang dibuat.
3. File yang diubah.
4. Diagram dependency singkat.
5. Penjelasan bagaimana Compatibility Layer bekerja.
6. Penjelasan bagaimana Telegram Client asli nanti akan dipasang.
7. Audit singkat apakah struktur sudah siap untuk Phase 2.3.2 (Telegram Client Implementation).

Jangan melakukan implementasi Telegram API pada phase ini. Fokus hanya pada fondasi dan arsitektur agar Phase 2.3.2 dapat langsung mengimplementasikan Telegram Client tanpa refactor besar.




```
