# Repeat

## Parameters

None

---

## Description

The REPEAT ... UNTIL loop allows you to perform  a series of commands until a specific condition has been met. This lets the  conditional appear after the commands have been executed before checking,  not before like the WHILE ... WEND  loop does. In general, use REPEAT ... UNTIL if you know you will have the commands  enclosed between them execute at least once.

See also: Until, Forever, Exit, While, For.

---

## Example

```blitzbasic
; Repeat until user hits ESC key

Repeat

print "Press ESC to quit this!"

Until KeyHit(1)
```