





# 
```

Enterprise adalah phase terakhir.

Jangan berhenti lagi sampai seluruh roadmap benar-benar selesai 100%.

Jangan memberikan update sementara.

Jangan melapor ketika:
- commit selesai,
- push selesai,
- PR dibuat,
- CI masih berjalan,
- Playwright masih berjalan,
- regression masih berjalan,
- audit masih berjalan.

Kerjakan semuanya sendiri.

Workflow wajib:

- mulai dari latest main
- buat branch Enterprise
- implementasikan seluruh sisa roadmap Enterprise
- jangan menggunakan mock
- jangan menghapus fitur yang sudah ada
- pertahankan backward compatibility
- update README, CHANGELOG dan dokumentasi bila diperlukan
- commit
- push
- buat Pull Request
- perbaiki seluruh CI sampai semuanya hijau
- merge ke main
- audit production
- regression test penuh
- bersihkan branch yang sudah selesai jika memungkinkan
- pastikan repository berada pada kondisi production-ready

Jika menemukan error:
- baca log
- perbaiki
- commit
- push
- jalankan ulang CI
- ulangi sampai hijau

Jangan meminta persetujuan.
Jangan berhenti karena error kecil.
Jangan membuat phase baru jika roadmap sudah selesai.

BARU kirim SATU laporan terakhir ketika seluruh roadmap benar-benar selesai 100%.

Laporan akhir harus berisi:

- Persentase roadmap (harus 100%)
- Daftar seluruh phase yang selesai
- Semua PR
- Semua merge commit
- Semua endpoint API baru
- Semua perubahan database
- Semua file yang berubah
- Semua GitHub Actions hijau
- Semua regression test lulus
- Status production
- Daftar branch yang masih ada
- Daftar branch yang berhasil dibersihkan
- Audit akhir repository
- Daftar fitur yang belum ada (jika masih ada)
- Kesimpulan apakah repository sudah production-ready

Target akhirnya adalah repository selesai 100%, production-ready, seluruh roadmap selesai, seluruh GitHub Actions hijau, seluruh regression test lulus, tanpa regression, dan tidak ada pekerjaan roadmap yang tersisa.



```
# 
```

Lanjutkan pekerjaan.

Phase 6 sudah selesai, merged ke main, seluruh GitHub Actions hijau, regression lulus, production bersih.

Sekarang lanjutkan mulai Phase 7 sampai seluruh roadmap selesai.

Aturan tetap sama:

- Jangan menggunakan mock.
- Jangan menghapus fitur yang sudah ada.
- Selalu mulai dari latest main.
- Buat satu branch untuk satu phase.
- Commit kecil jika diperlukan.
- Push ke GitHub.
- Buat Pull Request.
- Perbaiki seluruh CI sampai hijau.
- Merge ke main hanya setelah seluruh GitHub Actions hijau.
- Audit production.
- Baru lanjut ke phase berikutnya.

Jika CI gagal:
- baca log,
- perbaiki,
- commit,
- push,
- jalankan ulang,
- ulangi sampai hijau.

Jangan berhenti karena error kecil.

Jangan meminta persetujuan di tengah jalan.

Jangan memberikan update setiap commit, push, atau CI.

Hanya kirim laporan ketika SATU phase selesai sepenuhnya.

Setelah satu phase selesai, langsung lanjut phase berikutnya tanpa menunggu instruksi baru.

Di akhir setiap phase kirim laporan lengkap:

- Nomor phase
- PR
- Merge commit
- Daftar file berubah
- Endpoint API baru
- Perubahan database
- GitHub Actions
- Regression test
- Production audit
- Branch yang dibuat
- Branch yang di-merge
- Branch yang masih perlu dibersihkan
- Status roadmap (%)
- Phase berikutnya yang langsung dimulai

Target akhir adalah seluruh roadmap Phase 7 dan Enterprise selesai, seluruh PR sudah merge ke main, seluruh GitHub Actions hijau, production stabil, tanpa regression, dan tanpa menghentikan pekerjaan di tengah jalan kecuali ada blocker teknis yang benar-benar tidak dapat diperbaiki beserta log lengkap.



```
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
