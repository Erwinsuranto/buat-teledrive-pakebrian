


#
#Prompt: Fix MongoDB connection for Next.js API

```


Audit the entire repository and fix the root cause of the MongoDB timeout affecting the Next.js API.

Current findings:

- backend/src/database/mongodb.connection.ts exports connectMongoDB().
- repositories/file.repository.ts calls FileModel.find() directly.
- app/api/files/route.ts calls fileService.getAllFiles().
- No file inside app/, services/, or lib/ calls connectMongoDB().
- GET /api/files returns:
  Operation `files.find()` buffering timed out after 10000ms.
- GET /api/folders works correctly.
- npm run build passes successfully.

Requirements:

1. Find the correct place where connectMongoDB() should be initialized for the Next.js application.
2. Ensure every API route using MongoDB establishes a connection before any repository query.
3. Do NOT duplicate connection logic.
4. Reuse the existing backend/src/database/mongodb.connection.ts implementation if possible.
5. Keep connection singleton-safe.
6. Update imports if necessary.
7. Run npm run build.
8. Test:
   curl http://localhost:3000/api/files
   curl http://localhost:3000/api/folders
9. Continue fixing until /api/files returns JSON data instead of a timeout.
10. Commit only the required changes.
```

# 
```


The latest GitHub Actions build for PR #15 still fails.

Do not stop at the first error.

Audit the entire repository for missing module imports.

For every "Module not found: Can't resolve ..." error:
- determine whether the component was renamed, moved, or deleted,
- update imports or recreate the missing component if appropriate,
- remove stale imports only if they are no longer needed,
- run the build again,
- repeat until there are zero "Module not found" errors and all required GitHub Actions checks pass.

Do not finish until every required workflow is green.


```

# Prompt: Fix FolderCard After MockFolder Refactor
```


The production build fails because components/file/folder-card.tsx still uses an old MockFolder API.

Current MockFolder is:

type MockFolder = {
  id: string;
  name: string;
  kind: 'folder' | 'shared' | 'empty';
  fileCount: number;
  totalSize: string;
  created: string;
  updated: string;
  badge?: 'Shared' | 'Private' | 'Favorite' | 'Empty';
};

The component still references removed fields and legacy kinds:

- folder.previews
- folder.kind === 'photos'
- folder.kind === 'videos'
- folder.kind === 'archive'

Those no longer exist.

Update FolderCard to match the new MockFolder model.

Requirements:
- Remove every reference to previews.
- Remove every comparison with photos/videos/archive.
- Keep the visual layout as close as possible.
- Render a simple icon according to:
  - folder
  - shared
  - empty
- Preserve FolderBadge.
- Make the file compile with strict TypeScript.
- Do not use any `any` casts.
- Run npm run build and ensure there are zero TypeScript errors.
- Commit only the necessary changes.


```

# Prompt: Complete Build & Workflow Repair
```
Do not only inspect logs or perform an audit.

From now on, directly repair this repository.

Primary goal:

- Every GitHub Actions workflow must finish with SUCCESS.
- npm run build must pass.
- npm run typecheck must pass.
- npm run lint must pass.

Rules:

1. Do not stop after finding the first error.
2. Fix every file responsible for build failures.
3. For every "Module not found" error, determine the real cause:
   - moved file
   - deleted file
   - renamed file
   - incorrect import path
   Do not create placeholder or dummy components if the real file already exists.
4. Fix all TypeScript errors using the correct types.
5. Fix all React and Next.js implementation errors.
6. Run the build again after each repair.
7. Continue fixing every new error that appears.
8. Repeat until every workflow passes.
9. Do not stop to ask for approval after each fix.
10. Modify the repository directly.

After everything is fixed:

- Run npm run build
- Run npm run lint
- Run npm run typecheck
- Verify all GitHub Actions are SUCCESS.
- Commit all changes.
- Push to the current branch.

Do not stop until the entire workflow is green.




```

# Prompt: Fix Canonical Repository (Missing Modules)
```


Jangan membuat komponen, file, atau placeholder baru kecuali benar-benar tidak ada.

Lakukan audit terhadap seluruh repository dan perbaiki semua error "Module not found" dengan menggunakan struktur repository yang sudah ada.

Tugas:

1. Cari seluruh file yang dipindahkan, dihapus, atau diubah namanya.
2. Perbaiki semua import path yang salah.
3. Pulihkan struktur canonical repository.
4. Pastikan semua halaman Explorer, Upload, Activity, Favorites, Trash, Folder, dan My Files kembali menggunakan komponen yang benar.
5. Jangan menghapus fitur apa pun.
6. Jangan mengubah UI atau desain.
7. Jangan membuat mock component atau dummy component.
8. Jalankan npm run build setiap selesai memperbaiki satu kelompok error.
9. Ulangi sampai npm run build berhasil tanpa error.
10. Commit seluruh perubahan ke branch yang sedang digunakan.

Di akhir tampilkan:
- Ringkasan perbaikan
- Daftar file yang diubah
- Hasil build terakhir
- Error yang tersisa (jika masih ada)


```

# 
```

Prompt: Full Repository Repair, Audit & Workflow Verification

Your task is to fully stabilize this repository.

Do NOT stop after fixing the first error.

Continue fixing every compilation, runtime, TypeScript, React, Next.js and architecture issue until the repository reaches a successful production build.

Rules:

- Do NOT ask for confirmation.
- Do NOT create a new branch.
- Do NOT create a Pull Request.
- Work directly on the current branch.
- Preserve all existing functionality.
- Never bypass errors using any, ts-ignore, disabled type checking or fake implementations.

Perform a complete repository audit.

Audit:

- TypeScript
- Next.js
- React
- Server Actions
- API Routes
- MongoDB integration
- Telegram integration
- Upload workflow
- Folder workflow
- Search
- Preview
- Download
- Authentication
- GitHub Actions
- Build workflow
- ESLint
- Dead code
- Legacy mock data
- Broken imports
- Runtime errors
- File Explorer architecture

Whenever an error is found:

1. Fix it.
2. Run npm run build.
3. If another error appears, continue automatically.
4. Repeat until npm run build exits successfully.

After the build succeeds:

- Audit the repository again.
- Verify Upload.
- Verify Folder creation.
- Verify Folder selection.
- Verify MongoDB synchronization.
- Verify Search.
- Verify Preview.
- Verify Download.
- Verify File Explorer.

Ensure MongoDB is the canonical data source and the website correctly displays the stored folders and files.

Final report must include:

- Every modified file
- Why it was changed
- Build result
- Remaining warnings
- Audit summary
- Workflow verification summary
- Latest commit hash



```

# Prompt: Fix Folder Type Migration Build Error
```


Prompt: Fix Folder Type Migration

The build is failing because folder-card.tsx still depends on the legacy MockFolder model while the repository is being migrated to the real MongoDB folder model.

Current error:

components/file/folder-card.tsx

Type error:
This comparison appears to be unintentional because the types

"folder" | "shared" | "empty"

and

"photos"

have no overlap.

Requirements:

1. Do NOT silence TypeScript.

2. Do NOT use "as any".

3. Do NOT disable type checking.

4. Do NOT reintroduce old MockFolder types just to make the build pass.

5. Replace every remaining MockFolder dependency with the canonical MongoDB folder model.

6. Remove obsolete folder.kind comparisons such as:

folder.kind === "photos"

if those values no longer exist.

7. Search the entire repository for:

- MockFolder
- kind === "photos"
- kind === "videos"
- kind === "documents"
- any remaining mock folder implementation

Replace them with the current folder architecture.

Run:

npm run build

The build must complete successfully.

Report every modified file and explain why it was changed.


```


# Prompt: Replace Mock Data With Real MongoDB Data
```



The upload workflow is now working correctly.

Files are successfully uploaded to Telegram.

Metadata is successfully stored in MongoDB.

However, the website is still displaying mock/demo data.

Current problems:

- My Files still displays demo folders.
- Newly created folders do not appear.
- Newly uploaded files do not appear.
- Folder selector and file listing are not using the same database source.

Tasks:

1. Remove every remaining mock folder implementation.

2. Remove every remaining mock file implementation.

3. My Files must load real folders from MongoDB.

4. My Files must load real files from MongoDB.

5. Newly created folders must immediately appear.

6. Newly uploaded files must immediately appear.

7. Dashboard statistics must use MongoDB.

8. Search must search MongoDB.

9. Download must use MongoDB metadata.

10. Ensure every page uses the same backend services.

11. Verify there is only one canonical data source.

Do not create fake data.

Do not add placeholder data.

Do not hide errors.

Find every page still using mock data and replace it with the real MongoDB implementation.

Run npm run build.

Verify:

- Folder creation works.
- Uploaded files appear.
- Dashboard updates.
- Search finds uploaded files.
- Download works.

Only finish when the website uses real MongoDB data everywhere.

```

# Prompt: Fix Folder Database Integration
```

The upload system is working correctly.

Now fix the Folder integration.

Current runtime error:

Failed to fetch folders:
Operation `folders.find()` buffering timed out after 10000ms.

Tasks:

1. Find the exact cause of the timeout.

2. Verify MongoDB connection for the Folder model.

3. Verify the Folder schema.

4. Verify the Folder repository.

5. Verify the Folder service.

6. Verify the /api/folders endpoint.

7. Verify database initialization order.

8. Ensure Folder queries only run after MongoDB is connected.

9. Remove any remaining mock folder implementation.

10. The destination folder selector must load real folders from MongoDB.

11. Creating a new folder must immediately save it into MongoDB.

12. Newly created folders must immediately appear in the folder selector without refreshing the page.

Do NOT create fake data.

Do NOT hide the error.

Find the real root cause.

Run npm run build.

Verify:

- Folder list loads successfully.
- New folder creation works.
- Upload to selected folder works.
- Build passes.



```

# Prompt: Fix TypeScript Set Iteration Build Error
```


Fix the current TypeScript build failure.

Current error:

Type 'Set<string>' can only be iterated through when using '--downlevelIteration' or with a '--target' of 'es2015' or higher.

Requirements:

1. Do NOT change tsconfig.json only to silence the error.
2. Do NOT enable downlevelIteration unless it is already required by the project.
3. Fix the implementation instead.
4. Replace unsupported Set iteration with a compatible implementation.
5. Preserve the existing upload functionality.
6. Preserve multi-select.
7. Preserve remove selected files.
8. Preserve clear queue.
9. Preserve destination folder selection.
10. Do not modify unrelated files.

After fixing:

- Run npm run build.
- Verify the build completes successfully.
- Verify upload still works.
- List every modified file.
- Explain what was changed and why.


```

# 
```


The upload workflow is working correctly.

Do NOT modify backend logic.

Do NOT modify Telegram integration.

Do NOT modify MongoDB integration.

Improve the upload experience.

Requirements

1. Add destination folder selection before upload.

Users must be able to:

- choose an existing folder
- create a new folder
- change destination before upload

2. Optimize large batch uploads.

If selected files <= 10

Show:

- thumbnail
- filename
- size
- type

If selected files > 10

Do NOT render thumbnails.

Display a compact list:

- filename
- extension
- size
- status

This is required for better performance.

3. Queue management

Allow users to:

- remove a single file
- remove multiple selected files
- clear the entire queue
- cancel all uploads before they start

4. Upload summary

Display:

Selected Files

Uploading

Completed

Failed

Remaining

Total Size

5. Preserve existing upload behavior.

6. Verify that all features work on desktop and mobile.

Do not modify unrelated features.


```

# 
```


The upload functionality is now working correctly.

Do NOT modify backend logic.

Do NOT modify Telegram integration.

Do NOT modify MongoDB integration.

Improve the upload user experience.

Requirements:

1. After selecting files, DO NOT upload immediately.

2. Show an upload confirmation screen.

Display:

- Thumbnail (if image)
- File name
- File size
- File type
- Destination folder (if applicable)

Buttons:

- Cancel
- Upload

Only start uploading after the user presses "Upload".

During upload:

- Show progress bar
- Percentage
- Current status
- Remaining queue

After upload succeeds:

Show a success screen with:

- File name
- File size
- Upload time
- Telegram message ID
- Open File
- Copy Link
- Upload Another File

Keep all existing upload functionality.

Only improve the user experience.


```


# 
```

The file picker opens successfully.

The user can select a photo.

However, after selecting the file, nothing happens.

Investigate the upload frontend.

Check:

1. File input onChange handler.
2. React state updates after file selection.
3. Upload page navigation.
4. Upload component lifecycle.
5. JavaScript console errors.
6. API request initiation.
7. Network request execution.
8. Form submission logic.

Do not modify backend logic.

Trace the complete frontend upload flow from clicking "Select File" until the upload request is sent.

Fix the issue and verify that selecting a file immediately starts the expected upload workflow or displays the upload screen.



```

# 
```

You are continuing the Telegram Drive project.

The build is already successful.

The highest priority now is implementing a complete website upload system.

Do NOT redesign the UI.

Do NOT perform architecture refactoring.

Do NOT modify unrelated features.

Implement the complete upload workflow.

Requirements:

1. User selects a file from the website.
2. Backend validates the upload.
3. Backend sends the file to the Telegram Bot.
4. Telegram Bot uploads the file to the configured database channel.
5. Receive Telegram message_id and file information.
6. Save all metadata to MongoDB.
7. Return success to the frontend.
8. Display upload progress and final status.
9. Handle upload failures gracefully.
10. Ensure uploaded files appear in the database and are ready for My Files and Search.

After implementation:

- Verify the upload flow end-to-end.
- Confirm metadata is stored correctly.
- Confirm Telegram upload succeeds.
- List all modified files.
- Do not stop until the upload workflow is fully functional.



```
