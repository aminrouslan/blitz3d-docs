# CopyFile from$, to$

## Parameters

from$ = valid path/filename to the file to be copied

to$ = valid path/filename to copy the file to

---

## Description

Use this command to copy a file from one location to another. Perhaps you'll  write your own installer and need to copy files from the installation folder  to the installed location folder. Make sure you do your own validation to ensure  that the files/paths are valid and accurate before executing this command.

---

## Example

```blitzbasic
file$="c:autoexec.bat"

destination$="a:autoexec.bat"

Print "Press any key to copy your Autoexec.bat file to floppy"

WaitKey()

CopyFile file$,destination$
```