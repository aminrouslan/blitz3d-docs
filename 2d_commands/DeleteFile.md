# DeleteFile path/filename

## Parameters

path/filename = full path/filename to the file to delete

---

## Description

Deletes a specified file from the drive. You will need to make sure the  file exists before execution and be sure its been deleted AFTER execution. Use FILETYPE to determine this.

---

## Example

```blitzbasic
; DELETEFILE example

DeleteFile "C:	estmyfile.bb"
```