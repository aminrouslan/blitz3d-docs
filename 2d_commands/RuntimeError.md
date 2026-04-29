# RuntimeError message$

## Parameters

message$ = Any valid string

---

## Description

When doing your own error trapping, use this command to pop up a fatal error  and close the program. You can specify the error message that is displayed.

---

## Example

```blitzbasic
;There was a problem - raise an error and quit

RuntimeError "Installation corrupted. Please reinstall."
```