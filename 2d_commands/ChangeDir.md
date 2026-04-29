# ChangeDir directory/path

## Parameters

directory/path = full path to directory/folder

---

## Description

This command will change the currently selected directory for disk operations,  useful for advanced file operations. Use CURRENTDIR$()  to see what the current directory is.

Use a directory/path of ".." to change to the parent of the current directory,  unless you are at the root directory of the drive, then no change happens.

---

## Example

```blitzbasic
; ChangeDir example

ChangeDir "c:winntsystem32"

Print "The folder has been changed to: " + currentdir$()
```