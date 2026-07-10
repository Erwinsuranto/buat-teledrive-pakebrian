

# Prompt: Repository Context Loading (GPT-5.6)
```

You are taking over an existing software project from another AI.

Your first task is to completely understand this repository before making any code changes.

Read the entire repository carefully.

Analyze and understand:

- Overall project purpose
- Folder structure
- Frontend architecture
- Backend architecture
- API routes
- Database architecture
- Telegram Bot integration
- Authentication flow
- Upload workflow
- Download workflow
- Search workflow
- My Files workflow
- Admin Panel
- Dashboard
- Services
- Repositories
- Models
- Schemas
- Utilities
- Middleware
- Environment variables
- Build process
- Deployment configuration
- README and documentation
- Package configuration
- GitHub workflows

Identify:

- Completed features
- Features still under development
- Existing TODO/FIXME
- Existing mock data
- Existing technical debt
- Existing bugs (if any)

Rules:

- Do NOT modify any code.
- Do NOT refactor.
- Do NOT optimize.
- Do NOT create commits.
- Do NOT delete files.
- Do NOT install unnecessary dependencies.
- Do NOT ask for confirmation.
- Only understand the repository and build a complete mental model of the project.

After finishing, generate a detailed report including:

1. Project overview
2. Architecture summary
3. Folder structure summary
4. Current application flow
5. Completed features
6. Features still under development
7. Build status
8. Production readiness
9. Recommended next development priority

Wait for my next instruction before making any code changes.



```
# Prompt: Ubah Seluruh Website ke Bahasa Indonesia
```


Convert the entire website UI to Bahasa Indonesia.

Requirements:

- Replace every visible English text with natural Indonesian.
- Do not mix English and Indonesian.
- Use consistent terminology across the entire application.

Translate all:

- Navigation
- Buttons
- Labels
- Placeholders
- Headings
- Menus
- Dialogs
- Alerts
- Toast notifications
- Forms
- Empty states
- Validation messages
- Error messages
- Success messages
- Loading messages
- Pagination
- Tooltips
- Modals
- Search page
- Upload page
- Download page
- My Files
- Admin Panel
- Login
- Register
- Dashboard
- Settings
- Profile
- File Preview
- File Details

Use professional and user-friendly Indonesian.

Avoid machine-translated wording.

Keep all existing functionality.

Do not change backend logic.

If possible, centralize all UI text into one translation system (i18n/localization) so future language changes are easy.

Ensure no visible English text remains anywhere in the application except technical names, file extensions, API names, or developer-only logs.


```

# Judul: Redesign Search Page to Production UI
```


Completely redesign the Search page.

This page currently looks like a design demo.

Transform it into a real production Telegram Drive interface.

Requirements:

- Remove the large hero section.
- Remove "Find anything fast".
- Remove the long description.
- Remove fake Recent suggestions.
- Remove fake Suggestions.
- Remove all placeholder chips.

The page should immediately display:

- compact search bar
- storage summary
- folders
- files
- quick filters
- sorting
- pagination/load more if needed

Optimize for mobile first.

Reduce vertical spacing.

Show as many files as possible on one screen.

Use a modern Telegram Drive / Google Drive style.

Keep all existing functionality.

Only redesign the UI.

Do not modify backend logic.


```

# Prompt: Fix Build Until Success
```


You are continuing work on an existing Next.js + TypeScript repository.

The repository has already undergone a major architecture refactor.

Do NOT perform another architecture review.

Do NOT redesign the project.

Do NOT migrate anything.

Your only objective is to restore a successful production build.

Rules:

- Never ask for confirmation.
- Never stop after fixing one error.
- Automatically continue until npm run build succeeds.
- After fixing one build error, immediately run npm run build again.
- If another error appears, fix it automatically.
- Repeat until there are no TypeScript errors.
- Preserve all existing features.
- Do not remove functionality.
- Do not modify unrelated files.

Current status:
- Previous build errors (missing exports and renamed types) have already been fixed.
- The repository is now failing only because of remaining TypeScript compatibility issues introduced during refactoring.

Continue fixing:
- generic type mismatches
- ServiceResult<T> incompatibilities
- interface mismatches
- renamed types
- broken imports
- repository return types
- service return types

Do not stop until:

- npm run build exits successfully.
- No TypeScript errors remain.
- Next.js production build completes successfully.

At the end:

1. List every modified file.
2. Explain every fix.
3. Confirm that npm run build passes successfully.
4. Report any warnings that remain (warnings are acceptable if they do not fail the build).


```



# Prompt: Fix All Remaining TypeScript Build Errors
```
The previous build error has been fixed.

Now continue fixing ALL remaining TypeScript build errors automatically.

Current error:

components/file/list-view.tsx

imports

DriveFile

from

@/types/file

but that type is no longer exported.

Tasks:

1. Find where DriveFile was moved, renamed or replaced.

2. Restore compatibility.

3. Update every broken import across the repository.

4. Search the entire repository for all references to DriveFile.

5. Fix every broken type import.

6. Run npm run build again.

7. If another TypeScript error appears, immediately fix it and continue automatically.

8. Repeat until npm run build finishes successfully with exit code 0.

9. Do not stop after fixing one error.

10. Do not modify unrelated features.

11. At the end provide:
- modified files
- deleted files
- build result
- confirmation that npm run build completed successfully.
```
```
The project is failing because of a real TypeScript build error.

Do NOT perform any architecture refactoring.

Do NOT migrate anything.

Do NOT optimize unrelated files.

Your only task is to restore a successful build.

Current error:

app/files/[id]/page.tsx

imports

getFoundationFileById

from

@/services/file.service

but that function is no longer exported.

Tasks:

1. Find where getFoundationFileById was moved, renamed or removed.

2. Restore compatibility.

3. Either:
   - export the correct function again, OR
   - update every import to the new API.

4. Search the entire repository for every reference to getFoundationFileById.

5. Fix every broken import automatically.

6. Run npm run build repeatedly until it succeeds.

7. Do not stop after fixing only one error.

8. Continue fixing every build error until the build finishes successfully.

9. Do not modify unrelated functionality.

10. At the end report every modified file.




```


# Prompt: Continue Until Repository Is Fully Optimized
```

Continue from the latest commit.

Do not stop.

Do not ask for confirmation.

Assume production migration approval has already been granted.

If something cannot be verified because external production resources are unavailable (MongoDB deployment, Telegram credentials, backups, runtime environment, deployment topology), do NOT stop.

Instead:

- Complete every improvement that can be safely implemented inside the repository.
- Refactor every remaining architectural issue.
- Remove all obsolete code.
- Remove all duplicated code.
- Remove every unused file.
- Improve dependency injection.
- Improve repository structure.
- Improve runtime architecture.
- Improve API consistency.
- Improve documentation.
- Improve tests.
- Improve health checks.
- Improve deployment scripts.
- Improve startup validation.
- Improve rollback support.
- Improve migration tooling.

When an external resource is required, automatically create the necessary adapters, interfaces, validation code, migration scripts, and documentation so the repository is fully prepared.

Never stop because external infrastructure is unavailable.

Only exclude the final execution against production resources.

Everything else must be completed automatically.

At the end:

- run all tests
- run typecheck
- run build
- run lint
- fix every failure
- generate a complete report
- list every remaining issue that requires real production access

Everything that can be solved inside the repository must already be solved before stopping.



```



```
IMPORTANT EXECUTION RULES

Do NOT ask for confirmation.

Do NOT pause for approval.

Do NOT ask whether to continue.

Do NOT stop after analysis.

Automatically continue through every implementation phase until the repository reaches the best possible production-ready state.

If a migration is required, create any necessary compatibility layer automatically and continue the migration without waiting for permission.

If a destructive change could break existing functionality, first implement a safe migration strategy, backups, rollback support, and compatibility adapters, then continue automatically.

Preserve every existing feature.

Never leave the repository in a partially migrated state.

Complete every phase in one continuous workflow.

Only stop when:
- every possible architectural improvement has been completed,
- all tests pass,
- the project builds successfully,
- existing features still work,
- and a final production readiness report has been generated.

Do not ask me any questions unless you encounter an unrecoverable technical blocker that cannot be resolved from the repository itself.
```
# Prompt: Production Readiness 100% Audit & Architecture Refactor
```


You are the lead software architect for this repository.

Your task is NOT to rewrite the project.

Your task is to transform the current release candidate into a production-ready repository while preserving every existing feature and behavior.

Current audit summary:

- Repository Health Score: 68/100
- Code Quality: PASS
- Performance: PASS
- CI/CD: PASS
- Typecheck: PASS
- ESLint: PASS
- Build: PASS
- Tests: PASS

Remaining issues are architectural.

==================================================
ABSOLUTE RULES
==================================================

DO NOT remove any existing feature.

DO NOT break:

- Telegram upload
- Telegram download
- My Files
- Search
- Download tokens
- Authentication
- Sessions
- Admin panel
- Website
- APIs
- Dashboard
- Metadata
- Verification
- File sharing
- Existing database

Everything must continue working exactly as before.

Never reduce functionality.

Never replace working code only because you prefer another style.

Only improve architecture.

==================================================
OBJECTIVES
==================================================

Reach production-ready architecture.

Fix every issue reported by the audit.

Keep backwards compatibility.

Repository must remain fully functional after every commit.

==================================================
REQUIRED TASKS
==================================================

1. Remove duplicated legacy architecture.

There are duplicated:

- models
- repositories
- schemas
- services

Consolidate everything into ONE canonical backend architecture.

No duplicated business logic.

No duplicated persistence.

No duplicated models.

--------------------------------------------------

2. Remove legacy scaffolding.

Delete obsolete folders that are no longer used.

Delete compatibility code only if it is truly unused.

Remove obsolete ESLint configuration.

Remove dead code.

Remove abandoned files.

--------------------------------------------------

3. Production persistence.

Replace all runtime in-memory state with durable persistence.

Nothing important may disappear after server restart.

All runtime state must survive restart.

--------------------------------------------------

4. Runtime integration.

Connect every module to the canonical backend.

Authentication

Sessions

Verification

Dashboard

Metadata

Password reset

Admin

must all use the same architecture.

--------------------------------------------------

5. Telegram integration.

Telegram Bot must use the same repository architecture.

Do not allow separate database paths.

No duplicate service layer.

One persistence system only.

--------------------------------------------------

6. API consistency.

Version every endpoint consistently.

Avoid mixed API styles.

Use one routing strategy.

--------------------------------------------------

7. Monitoring.

Improve health checks.

Improve logging.

Improve telemetry abstraction.

Prepare production monitoring.

--------------------------------------------------

8. Multi-instance readiness.

Repository must support running multiple instances safely.

Avoid inconsistent runtime state.

Avoid singleton memory dependencies.

--------------------------------------------------

9. Release readiness.

Improve deployment workflow.

Improve migration workflow.

Improve rollback safety.

Improve startup validation.

--------------------------------------------------

10. Documentation.

Update README.

Update architecture documentation.

Explain every important structural change.

==================================================
VALIDATION
==================================================

After every major refactor automatically execute:

- npm install if needed
- typecheck
- eslint
- build
- unit tests
- integration tests

Fix every failure before continuing.

==================================================
SAFETY
==================================================

Never leave repository in broken state.

Commit only working code.

Preserve Git history.

Do not remove configuration required by deployment.

==================================================
FINAL GOAL
==================================================

The repository should achieve:

✔ Production-ready architecture

✔ No duplicate persistence

✔ No duplicate service layer

✔ Durable storage

✔ Unified backend

✔ Unified Telegram integration

✔ Clean folder structure

✔ Stable startup

✔ Stable deployment

✔ Stable runtime

✔ Backward compatibility

✔ Zero feature regression

At the end:

1. Produce a detailed report of every change.
2. Explain why each change was necessary.
3. List every modified file.
4. List every removed file.
5. Confirm that all existing features still work.
6. Run a final full validation.
7. If any requirement cannot be completed, explain exactly why and what is blocking it.
8. Do not stop until every possible architectural issue has been resolved without breaking functionality.


```


# Prompt: Final Production Audit & Stable Release Verification
```
You are working directly on this repository using GitHub MCP.

Current status:

- GitHub Actions are GREEN.
- Typecheck: PASS
- ESLint: PASS
- Build: PASS
- Tests: PASS
- Dependency Audit: PASS
- Release Candidate: PASS

Your task is NOT to rewrite the project.

Instead, perform a complete production-grade audit of the entire repository.

Audit every important area including:

1. Project architecture
2. Folder structure
3. Backend architecture
4. Frontend architecture
5. API routes
6. Database models
7. Services
8. Repository layer
9. Dependency Injection
10. TypeScript types
11. React components
12. Next.js App Router
13. Authentication
14. Authorization
15. File upload/download system
16. Telegram integration
17. Storage abstraction
18. Error handling
19. Logging
20. Environment configuration
21. Security
22. Performance
23. Scalability
24. Maintainability
25. Dead code
26. Duplicate code
27. Unused files
28. Unused dependencies
29. Circular dependencies
30. Broken imports
31. Workflow configuration
32. CI/CD
33. Release configuration
34. Documentation
35. Production readiness

Rules:

- Read the repository using GitHub MCP.
- Verify actual code instead of making assumptions.
- Do NOT modify working code without a real reason.
- Do NOT introduce new features.
- Do NOT refactor code that already passes unless there is a measurable benefit.
- Do NOT change architecture unless a real issue exists.

If you find problems:

- Explain the root cause.
- Estimate the impact.
- Fix only real issues.
- Commit only if code actually changes.
- Push the fixes.
- Wait for GitHub Actions.
- Ensure all workflows remain GREEN.

If no problems are found:

Do NOT create unnecessary commits.

Instead generate a production verification report containing:

# Repository Health Score (0–100)

## Architecture
PASS / FAIL

## Code Quality
PASS / FAIL

## Type Safety
PASS / FAIL

## Security
PASS / FAIL

## Performance
PASS / FAIL

## Maintainability
PASS / FAIL

## CI/CD
PASS / FAIL

## Documentation
PASS / FAIL

## Technical Debt

List every remaining issue ranked by:

Critical
High
Medium
Low

If there are none, explicitly write "None".

Finally answer with:

- Overall Production Readiness Score
- Remaining Risks
- Recommended Next Phase
- Whether the repository is suitable as the foundation for long-term development
- Whether you recommend creating the Stable Release branch now

Only claim "Production Ready" if the repository truly meets production-quality standards after verification.



```



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

