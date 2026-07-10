

# Prompt: Fix All TypeScript Errors Until GitHub Actions Pass
```
You are working directly on this repository using GitHub MCP.

Goal:
Fix ALL TypeScript errors until GitHub Actions "Release Candidate Verification" passes successfully.

DO NOT stop after fixing only one file.
DO NOT create temporary workarounds.
DO NOT use "any", "@ts-ignore", "skipLibCheck", "eslint-disable", or disable strict mode.
Keep the architecture intact.

The current failing workflow is Typecheck.

Known failing files include:

- app/files/[id]/page.tsx
- backend/src/persistence/mappers/index.ts
- services/file.service.ts
- services/download.service.ts
- services/folder.service.ts
- services/upload.service.ts
- services/user.service.ts
- components/file/file-card.tsx
- components/file/list-view.tsx
- components/upload/upload-experience.tsx
- types/file.ts

Known errors include:

1. TS2305
Missing exported member.
Verify imports and exports.
Do not rename APIs unless necessary.

2. TS2339
Properties like "_id" and "__v" do not exist.
Update mapper types to match the current Mongo document types instead of forcing casts.

3. TS2322
ServiceResult generic types no longer match returned values.
Update ServiceResult interfaces and service return types consistently.

4. TS2604 / TS2786
React component type errors involving Icon components.
Update imports and JSX typing so components use valid React component types.

5. TS7053
Invalid object indexing.
Use proper keyof types instead of unsafe indexing.

Requirements:

- Read every affected file using GitHub MCP.
- Trace the real source of each error.
- Fix root causes instead of patching symptoms.
- Update related interfaces and types where necessary.
- Keep API compatibility.
- Do not remove functionality.

After finishing:

1. Run typecheck.
2. Fix every remaining error.
3. Run lint.
4. Fix every lint issue.
5. Run build.
6. If any new TypeScript errors appear, continue fixing automatically.
7. Repeat until all gates pass.

Only when ALL of the following succeed:

- Typecheck
- Lint
- Build

then:

- Commit changes with a descriptive message.
- Push to the current branch.
- Wait for GitHub Actions.
- If GitHub Actions still fails, read the new errors, continue fixing automatically, commit again, and repeat until GitHub Actions is completely green.

Do NOT stop after the first commit.

Final output should contain only:

- Root causes fixed
- Files modified
- Final commit hash
- GitHub Actions status
- Remaining issues (if any)




```


# 
```


Lanjutkan tanpa meminta konfirmasi.

Jangan upgrade dependency apa pun kecuali benar-benar menjadi penyebab workflow gagal.

Repository GitHub tetap menjadi source of truth.

Tugas:

1. Periksa seluruh GitHub Actions yang gagal.
2. Identifikasi penyebab sebenarnya.
3. Jika penyebab bukan dependency, jangan melakukan upgrade package.
4. Perbaiki hanya akar masalah hingga seluruh workflow hijau.
5. Jalankan ulang:
   - typecheck
   - lint
   - build
   - unit tests
   - contract tests
   - integration tests
   - seluruh GitHub Actions
6. Jika semua workflow berhasil:
   - tandai README sebagai VERIFIED
   - tambahkan bagian:
     ## Release Candidate Verified
     - CI: PASS
     - Build: PASS
     - Tests: PASS
     - Workflow: PASS
     - Verified Date
     - Commit Hash
   - buat branch `phase-4.2-stable-release`
   - commit perubahan.

Output akhir cukup:
- Penyebab workflow gagal
- Cara perbaikan
- Commit hash
- README diperbarui
- Branch phase-4.2-stable-release dibuat
- Status READY FOR STABLE RELEASE


```


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

