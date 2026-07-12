







# 
```

Mulai sekarang jangan memberikan update setiap progress kecil.

Jangan melapor ketika:
- CI masih berjalan.
- Masih 8/10, 9/10 check.
- Masih menunggu Playwright.
- Masih memperbaiki error kecil.
- Masih push commit.

Kerjakan semuanya sendiri sampai selesai.

Jika CI gagal:
- baca log,
- perbaiki,
- commit,
- push,
- jalankan ulang,
- ulangi terus tanpa bertanya.

Jangan kirim status sementara.

Hanya berhenti dan memberikan laporan jika salah satu kondisi berikut terjadi:

1. Seluruh GitHub Actions hijau.
2. PR berhasil di-merge ke main.
3. Production regression selesai.
4. Audit production selesai.
5. Phase berikutnya sudah dibuat.
6. Ada blocker teknis yang benar-benar tidak bisa diperbaiki beserta log lengkap.

Jika seluruh Phase selesai, LANGSUNG lanjut ke phase berikutnya menggunakan workflow yang sama tanpa meminta izin lagi.

Di akhir setiap phase cukup kirim SATU laporan lengkap berisi:
- nomor Phase
- PR
- commit merge
- file yang berubah
- endpoint API baru
- perubahan database
- hasil GitHub Actions
- hasil regression
- status production
- phase berikutnya yang dimulai

Jangan mengirim update lain di tengah proses.
Fokus menyelesaikan roadmap secepat mungkin dengan tetap menjaga production tetap hijau.



```
# Prompt berikutnya
```

PROJECT: Telegram Drive

Lanjutkan Phase 6 sampai benar-benar selesai.

Jangan berhenti setelah memberi status.

WORKFLOW WAJIB

1. Pantau seluruh GitHub Actions pada PR Phase 6.
2. Jangan merge sebelum SEMUA check selesai.
3. Jika ada SATU check gagal:
   - buka log GitHub Actions
   - identifikasi root cause
   - perbaiki production code
   - commit
   - push
   - jalankan ulang CI
   - ulangi sampai seluruh check hijau
4. Jangan gunakan mock.
5. Jangan menghapus fitur lama.
6. Semua regression harus tetap hijau.
7. Semua API lama harus tetap kompatibel.

Jika seluruh GitHub Actions hijau:

- Merge PR ke main.
- Pull latest main.
- Jalankan full production regression.
- Audit production.
- Pastikan tidak ada regression.

Update:
- README.md
- CHANGELOG.md

Buat laporan lengkap:
- file yang berubah
- endpoint API baru
- perubahan database
- hasil seluruh GitHub Actions
- hasil regression
- commit merge
- status production

Jika seluruh audit production berhasil tanpa regression:

LANGSUNG mulai Phase 7 menggunakan latest main dengan workflow yang sama.

Setelah Phase 7 selesai dan merged:
langsung lanjut Enterprise menggunakan workflow yang sama.

Setiap phase harus:
- production-ready
- regression-tested
- seluruh GitHub Actions hijau
- merge ke main
- audit production
- baru lanjut phase berikutnya.

Jangan berhenti sampai seluruh roadmap selesai atau ada blocker teknis yang benar-benar tidak dapat diselesaikan beserta bukti log dan penjelasannya.



```
# Phase 6.
```


PROJECT: Telegram Drive

Mulai Phase 6 (Sharing & Collaboration).

WAJIB mengikuti workflow ini untuk Phase 6, Phase 7, dan seluruh Enterprise.

GENERAL RULES

- Production code only.
- Jangan menggunakan mock.
- Jangan menghapus fitur yang sudah ada.
- Jangan mengubah API lama kecuali benar-benar diperlukan dan tetap backward compatible.
- Semua fitur lama harus tetap berjalan.
- Semua perubahan harus regression-tested.
- README.md dan CHANGELOG.md harus diperbarui setiap phase.
- Setiap phase dimulai dari latest main.
- Setiap phase menggunakan branch baru.
- Merge hanya jika seluruh GitHub Actions hijau.

========================================
PHASE 6 — Sharing & Collaboration
========================================

Implement production-ready:

1. Sharing ke user tertentu (ACL)
   - Owner
   - Editor
   - Viewer
   - Commenter

2. Shared with me

3. Shared folders

4. Permission management UI

5. Link sharing
   - public
   - private
   - password
   - expiration
   - revoke

6. Comments

7. Mentions

8. Notifications

9. Activity feed

10. Tags

11. Labels

12. Folder color

13. Description

14. Better collaboration UX

15. Regression tests lengkap.

========================================

Setelah implementasi:

- lint
- typecheck
- build
- API Integration
- Folder Integration
- Chromium
- Firefox
- WebKit

Jika SATU saja gagal:

- buka log GitHub Actions
- cari root cause
- perbaiki production code
- commit
- push
- jalankan ulang CI
- ulangi sampai seluruh check hijau

Jika semua hijau:

- merge ke main
- pull latest main
- audit production
- regression penuh
- update README
- update CHANGELOG

========================================
AUTOMATIC CONTINUATION
========================================

Setelah Phase 6 selesai:

langsung mulai Phase 7 dengan workflow yang sama.

Setelah Phase 7 selesai:

langsung mulai Enterprise dengan workflow yang sama.

========================================
STOP CONDITION
========================================

Jangan berhenti di tengah pekerjaan.

Hanya berhenti apabila:

1. seluruh roadmap Telegram Drive telah selesai; ATAU

2. ada blocker teknis yang benar-benar tidak dapat diselesaikan, dan sertakan:
   - log GitHub Actions,
   - root cause,
   - file yang terdampak,
   - solusi yang sudah dicoba,
   - alasan teknis mengapa tidak dapat dilanjutkan.

Di akhir setiap phase berikan laporan lengkap:
- daftar file yang berubah,
- endpoint API baru,
- perubahan database,
- hasil seluruh GitHub Actions,
- hasil regression test,
- commit merge,
- status production.


```
