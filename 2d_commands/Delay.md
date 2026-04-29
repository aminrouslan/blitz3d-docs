# Delay milliseconds

## Parameters

milliseconds = the amount of milliseconds to delay. 1000=1 second

---

## Description

This command stops all program execution for the designated time period.  All execution stops. If you need program execution to continue, consider trapping  time elapsed with a custom timer function using Millisecs().

---

## Example

```blitzbasic
; Delay for 5 seconds

Delay 5000
```