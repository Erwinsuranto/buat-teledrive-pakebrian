
# Prompt: Phase 2.3.4 – Upload Engine (Implement & Commit)
```

Lanjutkan langsung Phase 2.3.4 tanpa meminta konfirmasi.

Gunakan seluruh fondasi Phase 2.3.3.

Target:
Membangun Upload Engine lengkap menggunakan abstraction yang sudah dibuat, tetapi belum terhubung ke Telegram API asli.

Kerjakan:

- Buat Upload Engine.
- Implement Upload Pipeline.
- Implement Upload Job Manager.
- Implement Chunk Upload Interface.
- Implement Progress Tracker.
- Implement Upload Queue.
- Implement Retry Upload.
- Implement Upload Metadata Builder.
- Implement Upload Result DTO.
- Implement Upload Error Mapper.
- Implement Upload Lifecycle.
- Tambahkan Contract Test.
- Audit dependency.
- Rapikan export/index.ts bila perlu.

Jangan:

- Login Telegram.
- Mengirim OTP.
- Menggunakan Bot API.
- Menghubungkan MTProto.
- Upload file sungguhan.
- Mengubah UI.
- Mengubah API.
- Mengubah Repository.

Semua masih berupa engine dan abstraction agar implementasi Telegram asli nanti hanya mengganti adapter.

Update README.md:

- Upload Engine Architecture.
- Upload Pipeline.
- Upload Lifecycle.
- Progress Phase 2.3.4.

Setelah selesai:

- Audit singkat.
- Perbaiki issue kecil bila ada.
- Jalankan typecheck bila memungkinkan.
- Commit langsung.

Output akhir:

- Commit hash.
- Ringkasan implementasi.
- File dibuat.
- File diubah.
- Status kesiapan menuju Phase 2.3.5 (Download Engine).

Jangan berhenti di tengah dan jangan meminta persetujuan. Selesaikan seluruh scope lalu commit.



```

# Prompt: Phase 2.3.3 – Real Telegram Transport Foundation (Implement & Commit)
```


Phase 2.3.3 dimulai.

Lanjutkan langsung tanpa meminta konfirmasi.

Gunakan hasil Phase 2.3.2 sebagai fondasi.

Target:
Mengimplementasikan Real Telegram Transport Foundation sehingga Telegram Client siap dihubungkan ke library Telegram asli tanpa mengubah Service, Repository, UI, maupun API.

Kerjakan:

1. Audit seluruh Telegram Client Foundation.
2. Implement Real Telegram Transport Interface.
3. Hubungkan Transport dengan TelegramAdapter menggunakan Dependency Injection.
4. Buat Session Storage abstraction.
5. Buat Connection Lifecycle.
6. Buat Authentication Lifecycle.
7. Buat Transport State Manager.
8. Buat Connection Pool Manager.
9. Buat Retry Transport Layer.
10. Buat Transport Error Mapper.
11. Buat Transport Event Dispatcher.
12. Buat Upload Transport Interface.
13. Buat Download Transport Interface.
14. Buat Delete Transport Interface.
15. Buat Forward Transport Interface.
16. Buat Metadata Transport Interface.
17. Buat Health Monitoring.
18. Tambahkan Contract Test.
19. Audit dependency dan import.
20. Rapikan export/index.ts bila diperlukan.

Penting:

- Belum login Telegram.
- Belum mengirim OTP.
- Belum menggunakan akun Telegram.
- Belum upload file.
- Belum download file.
- Belum delete file.
- Belum forward message.
- Belum mengubah UI.
- Belum mengubah API.
- Belum mengubah Repository.
- Belum mengubah Business Logic.

Fokus hanya membangun pondasi Real Transport agar implementasi Telegram asli pada phase berikutnya cukup mengganti implementasi adapter tanpa refactor.

Update README.md:

- Real Transport Architecture
- Connection Lifecycle
- Session Lifecycle
- Transport Layer
- Dependency Flow
- Progress Phase 2.3.3

Setelah selesai:

- Jalankan audit singkat.
- Perbaiki issue kecil bila ditemukan.
- Jalankan typecheck bila memungkinkan.
- Commit seluruh perubahan.

Tampilkan:

- Commit hash.
- Ringkasan implementasi.
- File dibuat.
- File diubah.
- Status kesiapan menuju Phase 2.3.4 (Telegram Upload Engine).

Jangan meminta konfirmasi. Selesaikan seluruh scope Phase 2.3.3 kemudian commit langsung.


```
# Prompt: Phase 2.3.2 – Telegram Client Core (Implement & Commit)
```

Phase 2.3.2 dimulai.

Lanjutkan langsung tanpa meminta konfirmasi.

Gunakan hasil Phase 2.3.1 sebagai fondasi.

Target:
Membangun Telegram Client Core yang nantinya menjadi implementasi nyata dari TelegramAdapter.

Kerjakan:

- Audit seluruh Compatibility Layer yang sudah dibuat.
- Implement Telegram Client Interface sebagai implementasi TelegramAdapter.
- Siapkan Session Manager.
- Siapkan Connection Manager.
- Siapkan Authentication Contract.
- Siapkan File Upload Pipeline.
- Siapkan File Download Pipeline.
- Siapkan Delete Pipeline.
- Siapkan Forward Pipeline.
- Siapkan Metadata Reader.
- Siapkan Health Check.
- Siapkan Retry Manager.
- Siapkan Error Handler.
- Siapkan Progress Callback.
- Siapkan Client Factory.
- Tambahkan seluruh DTO yang diperlukan.
- Tambahkan Mapper bila diperlukan.
- Tambahkan Contract Test untuk Telegram Client.

Semua implementasi masih berupa foundation.

Jangan login Telegram.

Jangan menghubungkan MTProto.

Jangan menggunakan Telegram Bot API.

Jangan mengirim file.

Jangan download file.

Jangan mengubah UI.

Jangan mengubah API.

Jangan mengubah Repository.

Jangan mengubah Business Logic.

Pastikan seluruh dependency tetap melalui TelegramAdapter dan Dependency Injection.

Rapikan export/index.ts bila diperlukan.

Update README.md:

- Telegram Client Architecture
- Client Lifecycle
- Upload Pipeline
- Download Pipeline
- Session Management
- Progress Phase 2.3.2

Setelah selesai:

- Audit singkat struktur.
- Perbaiki issue kecil bila ditemukan.
- Jalankan typecheck bila memungkinkan.
- Commit seluruh perubahan.
- Tampilkan:
  - Commit hash
  - Ringkasan implementasi
  - File dibuat
  - File diubah
  - Status kesiapan menuju Phase 2.3.3 (Real Telegram Integration)

Jangan meminta konfirmasi. Selesaikan seluruh scope Phase 2.3.2 kemudian commit langsung.



```
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
