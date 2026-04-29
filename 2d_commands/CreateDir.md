# CreateDir path/name

## Parameters

path/name = full path and name for new directory

---

## Description

Creates a directory (file folder) at the destination specified. Do not use  a trailing slash at the end of the path/name parameter. You cannot be sure the  directory was created with this command, so you will need to verify its existance  yourself (use the FILETYPE command).

---

## Example

```blitzbasic
; CREATEDIR example

fldr$="c:winntsystem32myfolder"

createDir fldr$

Print "Folder created!"
```