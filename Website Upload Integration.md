
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
