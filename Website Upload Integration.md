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
