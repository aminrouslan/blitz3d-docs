# DeleteDir directory/path

## Parameters

directory/path = full path/name of directory

---

## Description

Deletes a specified folder/directory from the device. Note: This only works  on EMPTY directories - you cannot delete a folder with other folders or files  inside with this command. Do not apply a trailing slash.

---

## Example

```blitzbasic
; DeleteDir example

DeleteDir "C:	est"
```