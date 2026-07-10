# Phase 2 dimulai 

# Phase 2.2.7 – Backend Validation & Migration
```


Phase 2.2.7 dimulai.

Selesaikan seluruh High Priority blocker sebelum memulai Telegram Service.

Target:
Project harus benar-benar siap secara teknis untuk memasuki Phase 2.3.

Kerjakan:

- Pastikan seluruh typecheck lulus tanpa error.
- Buat dan jalankan integration test untuk Repository MongoDB.
- Verifikasi CRUD utama:
  - User
  - Folder
  - File
  - Activity
  - ShareLink
  - UploadJob
  - DownloadHistory
- Audit seluruh repository legacy di root.
- Migrasikan persistence lama ke Repository Layer baru bila aman.
- Pastikan tidak ada dependency lama yang masih dipakai.
- Pastikan seluruh wiring menggunakan Composition Root.
- Jangan mengubah UI.
- Jangan membuat Telegram Service.
- Jangan membuat API endpoint.

Update README.md dengan bagian:

- Backend Validation
- MongoDB Integration Test
- Legacy Migration
- Readiness Report

Di akhir:

1. Hasil typecheck.
2. Hasil integration test.
3. File yang diubah.
4. Legacy yang berhasil dimigrasikan.
5. Konfirmasi apakah seluruh High Priority blocker telah selesai.
6. Jika semua lulus, nyatakan project siap memasuki Phase 2.3 Telegram Service.


```
# Prompt: Phase 2.2.6 – Verification & Integration Readiness
```


Phase 2.2.6 dimulai.

Sebelum memulai Telegram Service, lakukan tahap verifikasi akhir terhadap Repository Layer dan MongoDB Foundation.

Target:
Memastikan fondasi backend benar-benar siap untuk integrasi Telegram tanpa menghasilkan technical debt.

Kerjakan:

- Jalankan typecheck seluruh project.
- Jalankan integration test Repository dan MongoDB jika sudah tersedia.
- Periksa seluruh dependency injection dan composition root.
- Verifikasi seluruh Repository Contract telah digunakan dengan benar.
- Pastikan tidak ada import langsung Mongoose Model dari Service Layer.
- Pastikan seluruh mapper berjalan sesuai Domain Entity.
- Audit kembali relasi antar repository.
- Periksa tidak ada dependency cycle.
- Periksa tidak ada duplicate repository.
- Jangan mengubah UI.
- Jangan membuat Telegram Service.
- Jangan membuat API endpoint.

Jika menemukan masalah:
- Perbaiki hanya jika aman dan tidak mengubah arsitektur.
- Jika perubahan besar diperlukan, hentikan dan jelaskan alasannya.

Update README.md dengan bagian "Phase 2.2 Verification".

Di akhir:

1. Ringkasan hasil verifikasi.
2. File yang diubah (jika ada).
3. Hasil typecheck dan integration test.
4. Konfirmasi apakah project 100% siap memasuki Phase 2.3 Telegram Service.


```
# Prompt: Phase 2.2.5 – Domain & Repository Implementation
```

Phase 2.2.5 dimulai.

Gunakan hasil audit Repository Layer sebagai acuan implementasi.

Tujuan:
Menyelesaikan seluruh temuan High Priority pada Domain Layer dan Repository Layer sebelum memulai Telegram Service.

Kerjakan:

- Lengkapi Repository khusus:
  - FileRepository
  - FolderRepository
  - UploadJobRepository
  - ShareLinkRepository
  - ActivityRepository
  - FavoriteRepository
  - TrashRepository
  - UserRepository

- Jadikan Domain Entity sebagai sumber kebenaran, bukan Mongoose Model.

- Pisahkan Domain Entity, Database Model, Repository, dan Service agar tidak saling bergantung langsung.

- Tambahkan mapper Domain ↔ Database bila diperlukan.

- Pastikan Repository tidak pernah mengembalikan Mongoose Document ke Service Layer.

- Rapikan dependency direction sesuai hasil audit.

- Hilangkan duplikasi struktur antara root dan backend jika memungkinkan tanpa merusak project.

- Tambahkan validasi, index, dan repository contract yang diperlukan.

- Jangan mengubah UI.

- Jangan membuat API.

- Jangan menghubungkan Telegram.

- Jangan menghapus mock data frontend.

Update README.md mengenai perubahan Repository Layer.

Di akhir pekerjaan:

1. Sebutkan seluruh masalah audit yang berhasil diperbaiki.
2. Sebutkan file yang dibuat dan diubah.
3. Lakukan audit ulang singkat.
4. Berikan penilaian apakah project sudah siap masuk ke Phase 2.3 Telegram Service.

Jika masih ada blocker High Priority, hentikan implementasi dan jelaskan apa yang masih harus diselesaikan terlebih dahulu.



```
# Prompt: Phase 2.2.5 – Domain & Repository Implementation
```

Phase 2.2.5 dimulai.

Lanjutkan pembangunan backend Telegram Drive dengan menyempurnakan Domain Layer dan Repository Layer berdasarkan arsitektur serta MongoDB Foundation yang telah dibuat.

Target:
Membuat fondasi data yang benar-benar siap digunakan oleh Telegram Service, API, dan UI tanpa mengubah tampilan aplikasi.

Kerjakan:

- Lengkapi seluruh Repository Interface.
- Lengkapi implementasi Repository.
- Audit seluruh Model dan Schema.
- Pastikan relasi User, Folder, File, Share Link, Activity, Favorite, Trash, Upload Job, dan Download History sudah konsisten.
- Tambahkan validation pada model.
- Tambahkan mapper antara Database Model dan Domain Model bila diperlukan.
- Pastikan seluruh business logic tetap berada di Service Layer, bukan Repository.
- Siapkan Transaction Pattern bila nanti dibutuhkan.
- Tambahkan unit test dasar untuk repository (jika project sudah mendukung testing).

Jangan membuat API endpoint.

Jangan menghubungkan Telegram.

Jangan mengubah UI.

Jangan menghapus mock data yang masih dipakai frontend.

Update README.md:

- Domain Layer
- Repository Layer
- Collection Relationship
- Data Flow
- Progress Phase 2

Setelah selesai:

- Jelaskan struktur Repository.
- Sebutkan file yang dibuat dan diubah.
- Jelaskan relasi antar model.
- Jelaskan kesiapan untuk Phase 2.3 Telegram Service.
- Lakukan audit agar Repository siap digunakan seluruh project.



```
# Prompt: Phase 2.2 – MongoDB Foundation
```

Phase 2.2 dimulai.

Lanjutkan pengembangan backend Telegram Drive dengan membangun fondasi MongoDB berdasarkan arsitektur yang sudah diaudit.

Target:
Membangun layer database yang bersih, modular, scalable, dan siap digunakan oleh seluruh fitur Telegram Drive.

Kerjakan:

- Buat koneksi MongoDB yang reusable.
- Buat database configuration.
- Buat model/schema utama:
  - User
  - Folder
  - File
  - Share Link
  - Activity
  - Favorite
  - Trash
  - Upload Job
  - Download History
- Buat repository interface dan implementasinya.
- Pisahkan model, repository, dan database layer dengan jelas.
- Gunakan dependency injection bila struktur project mendukung.
- Pastikan seluruh repository belum mengubah UI maupun business logic.
- Belum perlu menghubungkan Telegram Bot.
- Belum perlu membuat API endpoint.
- Jangan menghapus mock data, cukup siapkan agar nanti mudah diganti.

Update README.md:

- MongoDB Architecture
- Collection Structure
- Repository Layer
- Database Flow
- Progress Phase 2

Setelah selesai:

- Jelaskan schema yang dibuat.
- Sebutkan file yang dibuat dan diubah.
- Jelaskan hubungan antar collection.
- Lakukan audit agar struktur database mudah dikembangkan untuk Telegram Drive.



```
```

Phase 2 dimulai.

Lakukan audit menyeluruh terhadap project Telegram Drive dan siapkan fondasi backend untuk pengembangan selanjutnya.

Tujuan:
Membangun arsitektur backend yang bersih, modular, scalable, dan mudah dipelihara tanpa mengubah UI yang telah selesai.

Tugas:

- Audit seluruh struktur project.
- Identifikasi seluruh mock data, dummy service, dan placeholder.
- Pisahkan dengan jelas Presentation Layer, Business Logic, dan Data Layer.
- Audit struktur folder, dependency, dan reusable components.
- Identifikasi technical debt, duplicate code, dan potensi bug.
- Pastikan struktur siap untuk MongoDB, Telegram Bot, Telegram Channel, Authentication, Upload, Download, Share Link, dan Admin Panel.
- Jangan mengubah tampilan UI, UX, routing, maupun komponen frontend yang sudah selesai.

Buat dokumentasi arsitektur yang menjelaskan:

- Project Structure
- Folder Responsibility
- Data Flow
- Service Layer
- Repository Layer
- API Layer
- Database Layer
- Telegram Integration Layer

Update README.md dengan:

- Phase 2 Roadmap
- Architecture Overview
- Current Project Status
- Backend Development Plan
- Daftar Mock Data yang akan diganti pada tahap berikutnya

Di akhir pekerjaan berikan laporan berisi:

1. Ringkasan audit.
2. Struktur project setelah audit.
3. File yang dibuat atau diubah.
4. Masalah yang ditemukan.
5. Rekomendasi implementasi Phase 2.2.

Jangan mulai menghubungkan MongoDB atau Telegram pada tahap ini. Fokus hanya pada audit dan persiapan arsitektur backend.



```
