

# Phase 3.5 – User Dashboard & Profile.
```
Lanjutkan langsung Phase 3.5 User Dashboard & Profile.

Jangan meminta konfirmasi.
Jangan audit ulang repository.
Repository GitHub tetap menjadi source of truth.
Langsung buat branch baru dan commit setelah selesai.

Target Phase 3.5:

Implementasikan fondasi Dashboard User dan Profile yang siap dihubungkan dengan UI.

Scope implementasi:

- Current User Service
- Dashboard Service
- User Profile Service
- Profile Controller
- Dashboard Controller
- Dashboard API
- Profile API
- Avatar abstraction
- User statistics service
- Storage usage service
- Recent activity service
- Favorite summary service
- Shared files summary
- Upload summary
- Download summary
- Account status
- Session list API
- Logout all sessions
- Profile update
- Change email preparation
- Change password integration
- DTO
- Validator
- Mapper
- Error mapper
- Dependency Injection
- Repository integration
- Contract tests
- Integration tests bila memungkinkan
- Export/index
- README

Jangan mengubah:

- UI
- Telegram
- Upload Engine
- Download Engine
- Metadata Engine
- File Manager

Jika menemukan bug kecil pada Authentication, perbaiki langsung.

Jalankan workflow, typecheck, contract test, dan integration test.

Jika seluruh test hijau, langsung commit.

Output akhir cukup:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- Status siap menuju Phase 3.6 Admin Foundation




```

# Siap menuju Phase 3.4 Password Reset
```
Lanjutkan langsung Phase 3.4 Password Reset.

Jangan meminta konfirmasi.
Jangan audit ulang repository.
Jangan membaca ulang project.
Repository GitHub tetap menjadi source of truth.
Langsung buat branch baru dan commit setelah selesai.

Target Phase 3.4:

Implementasikan sistem Password Reset production-ready.

Scope:

- Password Reset Token Entity
- Repository
- Service
- Controller
- Forgot Password endpoint
- Reset Password endpoint
- Token generator
- Token hash
- Token expiry
- Single-use token
- Revoke token setelah digunakan
- Rate limiter
- Email provider abstraction
- Mock mail provider
- Email template abstraction
- Security validation
- Audit log hook
- DTO
- Validator
- Mapper
- Error mapper
- Dependency Injection
- Contract tests
- Integration tests bila memungkinkan
- Export/index
- README

Jangan mengubah:

- UI
- Telegram
- Upload Engine
- Download Engine
- File Manager
- Metadata Engine
- Authentication yang sudah selesai selain bug kecil

Jika menemukan bug kecil, perbaiki langsung.

Jalankan workflow, typecheck, dan seluruh test.

Jika semuanya hijau, langsung commit.

Output akhir cukup berisi:

- Commit hash
- Ringkasan implementasi
- File dibuat
- File diubah
- Status siap menuju Phase 3.5 User Dashboard & Profile




```

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
