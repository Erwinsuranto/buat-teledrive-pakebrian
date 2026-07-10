

# Phase 3.3.
```


Lanjutkan langsung Phase 3.3 Email Verification tanpa meminta konfirmasi apa pun.

Repository GitHub adalah source of truth. Jangan audit ulang repository. Jangan membaca ulang seluruh project. Langsung lanjut dari branch Phase 3.2.

Scope Phase 3.3:

Implementasikan fondasi lengkap Email Verification.

Kerjakan dalam satu branch dan commit akhir.

Implementasikan:

- Email Verification Service
- Verification Token Entity
- Repository
- Service
- Controller
- HTTP Routes
- Send Verification Email
- Verify Email Endpoint
- Resend Verification Endpoint
- Token Expiration
- One-time Token
- Secure Random Token Generator
- Rate Limit
- Email Template Abstraction
- Mail Provider Interface
- Mock Mail Provider
- Event Hook
- DTO
- Validator
- Mapper
- Error Mapper
- Contract Test
- Integration Test bila memungkinkan
- Export
- README

Jangan mengubah:

- UI
- Telegram
- Upload Engine
- Download Engine
- File Manager
- Metadata Engine

Gunakan dependency injection yang sudah ada.

Jika menemukan bug kecil di Authentication, perbaiki langsung tanpa bertanya.

Jalankan typecheck dan seluruh test.

Jika lolos, langsung commit.

Output akhir cukup:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- Status siap menuju Phase 3.4 Password Reset


```

# Prompt: Phase 3.2 – Login & Register API
```

Lanjutkan langsung Phase 3.2 tanpa meminta konfirmasi apa pun.

Repository GitHub adalah source of truth. Jangan audit ulang seluruh repository kecuali yang berkaitan dengan Authentication.

Target Phase 3.2:

Implementasikan Login & Register API yang benar-benar siap dipakai website nantinya.

Kerjakan seluruh implementasi berikut dalam satu commit:

- Register endpoint
- Login endpoint
- Logout endpoint
- Refresh Token endpoint
- Get Current User endpoint
- Update Profile endpoint
- Change Password endpoint
- Session revoke endpoint
- Remember Me support
- Multi-device session
- Cookie/JWT compatibility
- CSRF preparation
- Rate limiter hook
- Account lock policy hook
- Email verification hook (placeholder)
- Password reset hook (placeholder)

Lengkapi:

- DTO
- Validator
- Mapper
- Error handling
- Controller
- Service
- Repository integration
- Contract test
- Integration test bila memungkinkan
- Export/index
- README.md

Jangan mengubah:

- UI
- Telegram
- Upload Engine
- Download Engine
- Transfer Engine
- Metadata Engine
- File Manager

Semua endpoint harus fail-closed dan memakai dependency injection yang sudah ada.

Apabila menemukan bug kecil pada Authentication Foundation, perbaiki langsung tanpa meminta persetujuan.

Jalankan typecheck dan seluruh contract test bila tersedia.

Jika ada warning kecil yang aman diperbaiki, perbaiki langsung.

Setelah selesai langsung commit ke branch Phase 3.2.

Output akhir cukup berisi:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- Status kesiapan menuju Phase 3.3 Email Verification



```

# Prompt: Phase 3.1 – User & Authentication Foundation
```

Lanjutkan langsung Phase 3.1 tanpa meminta konfirmasi apa pun.

Anggap repository GitHub saat ini sebagai source of truth. Audit singkat otomatis sebelum mulai tanpa meminta izin.

Target:

Membangun fondasi User Management dan Authentication yang akan dipakai seluruh website.

Kerjakan:

- User Entity.
- User Repository.
- User Service.
- User Profile.
- Email Authentication.
- Password Hashing.
- Session Management.
- JWT Authentication.
- Refresh Token.
- Role System.
- Permission System.
- Account Status.
- Login Audit.
- Security Middleware.
- Authentication DTO.
- Authentication Validator.
- Authentication Error Mapper.
- Contract Test.
- Rapikan export/index.ts bila diperlukan.

Jangan:

- Mengubah UI.
- Menghubungkan Telegram.
- Mengubah Upload Engine.
- Mengubah Download Engine.
- Mengimplementasikan OTP.
- Mengimplementasikan Login Page.

Tahap ini hanya membangun backend dan fondasi authentication.

Update README.md:

- Authentication Architecture.
- User Architecture.
- Security Flow.
- Progress Phase 3.1.

Setelah selesai:

- Audit singkat.
- Perbaiki issue kecil bila ada.
- Jalankan typecheck bila memungkinkan.
- Commit langsung tanpa meminta persetujuan.

Output akhir:

- Commit hash.
- Ringkasan implementasi.
- File dibuat.
- File diubah.
- Status kesiapan menuju Phase 3.2 (Login & Register API).



```
