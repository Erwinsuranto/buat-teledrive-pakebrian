


# Phase 4.2 Stable Release belum boleh dimulai, karena AI menyatakan status CI/Workflow hijau belum dapat diverifikasi dari aksesnya.
```

Lanjutkan tanpa meminta konfirmasi.

Jangan audit ulang repository.
Jangan membuat fitur baru.
Jangan mengubah arsitektur.

Repository GitHub tetap menjadi source of truth.

Fokus hanya pada verifikasi Release Candidate.

1. Periksa seluruh GitHub Actions / CI Workflow.
2. Pastikan:
   - typecheck sukses
   - lint sukses
   - build sukses
   - unit tests sukses
   - contract tests sukses
   - integration tests sukses
   - workflow utama hijau
3. Jika ada workflow gagal:
   - identifikasi penyebab
   - perbaiki source code atau workflow
   - commit perbaikan
   - jalankan ulang hingga seluruh workflow hijau.
4. Jika seluruh workflow sudah hijau:
   - tandai Release Candidate sebagai VERIFIED.
   - buat branch Phase 4.2 Stable Release.
   - update README.md dengan section:

## Phase 4.2 Ready

Berisi:
- Status CI
- Status Tests
- Status Build
- Status Workflow
- Commit Hash terakhir
- Tanggal verifikasi
- Project Ready for Stable Release

Output akhir cukup:

- Status seluruh workflow
- Workflow yang diperbaiki (jika ada)
- Commit hash
- README diperbarui
- Apakah project sudah benar-benar siap memasuki Phase 4.2 Stable Release.



```


# Phase 4.1 Final QA & Release Candidate.
```


Lanjutkan langsung Phase 4.1 Final QA & Release Candidate.

Jangan meminta konfirmasi.
Jangan audit ulang seluruh repository.
Jangan berhenti di tengah.
Repository GitHub tetap menjadi source of truth.

Buat branch baru.

Target Phase 4.1:

- Jalankan audit akhir seluruh backend.
- Perbaiki seluruh warning.
- Perbaiki seluruh error.
- Hapus dead code.
- Hapus unused imports.
- Hapus duplicate implementation.
- Rapikan folder bila diperlukan tanpa breaking change.
- Verifikasi seluruh API contract.
- Verifikasi seluruh Repository contract.
- Verifikasi seluruh Service contract.
- Verifikasi Authentication.
- Verifikasi Upload Engine.
- Verifikasi Download Engine.
- Verifikasi Transfer Engine.
- Verifikasi Metadata Engine.
- Verifikasi File Manager.
- Verifikasi Dashboard.
- Verifikasi Admin.
- Verifikasi Monitoring.
- Verifikasi Telegram Integration.
- Verifikasi Database.
- Verifikasi Production Config.
- Verifikasi Security Middleware.
- Verifikasi Health Endpoint.
- Verifikasi Logging.
- Verifikasi Environment.
- Verifikasi Export.

Jalankan:

- typecheck
- lint
- build
- unit tests
- contract tests
- integration tests
- workflow

Perbaiki otomatis sampai seluruh workflow hijau.

Setelah selesai:

- Commit.
- Update README.md.

Tambahkan section baru:

## Phase 4.1 - Final QA & Release Candidate

Isi:

- Ringkasan QA
- Bug yang diperbaiki
- Warning yang dihilangkan
- File baru
- File diubah
- Hasil seluruh test
- Build status
- Workflow status
- Commit hash
- Status roadmap
- Next Phase: 4.2 Stable Release

README.md harus tetap menjadi changelog lengkap seluruh project dari Phase 2 sampai Phase 4.1 tanpa menghapus riwayat sebelumnya.

Output akhir cukup:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- README diperbarui
- Semua test hijau
- Build sukses
- Status siap menuju Phase 4.2 Stable Release


```


# Phase 4.0 Production Hardening & Final Integration.
```
Lanjutkan langsung Phase 4.0 Production Hardening & Final Integration.

Jangan meminta konfirmasi.
Jangan audit ulang seluruh repository.
Jangan berhenti di tengah.
Repository GitHub tetap menjadi source of truth.

Buat branch baru.

Target Phase 4.0:

- Hardening seluruh backend.
- Audit dependency yang dipakai saja.
- Rapikan import/export.
- Hilangkan duplicate code.
- Optimasi DI Container.
- Optimasi Repository Layer.
- Optimasi Service Layer.
- Optimasi API Layer.
- Optimasi Database Layer.
- Optimasi Telegram Layer.
- Optimasi Authentication.
- Tambahkan centralized configuration validation.
- Tambahkan production error handler.
- Tambahkan structured logging.
- Tambahkan request tracing.
- Tambahkan graceful shutdown.
- Tambahkan health check final.
- Tambahkan readiness & liveness endpoint.
- Tambahkan production environment validation.
- Tambahkan security headers.
- Tambahkan rate limiter global.
- Tambahkan API versioning bila belum ada.
- Rapikan folder structure bila diperlukan tanpa breaking change.
- Pastikan seluruh contract tetap kompatibel.
- Pastikan fail-closed tetap aktif.

Jalankan:

- typecheck
- lint
- unit tests
- contract tests
- integration tests
- workflow

Perbaiki otomatis jika ada kegagalan hingga seluruh workflow hijau.

Setelah selesai:

- Commit.
- Update README.md.

Tambahkan section baru:

## Phase 4.0 - Production Hardening & Final Integration

Berisi:

- Tujuan
- Ringkasan implementasi
- File baru
- File diubah
- Optimasi yang dilakukan
- Security improvements
- Performance improvements
- Breaking changes (jika ada)
- Commit hash
- Status roadmap
- Next Phase: 4.1 Final QA & Release Candidate

README harus menjadi changelog lengkap seluruh project dan mempertahankan riwayat phase sebelumnya.

Output akhir cukup:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- README diperbarui
- Status siap menuju Phase 4.1 Final QA & Release Candidate




```

