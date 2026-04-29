# Until condition

## Parameters

condition = any valid expression (see example)

---

## Description

This portion of the REPEAT ... UNTIL loop dictates  what condition must be met before the loop stops execution. All commands between  the two commands will be executed endlessly until the UNTIL condition is met.

See also: Repeat, Forever, Exit, While, For.

---

## Example

```blitzbasic
; Repeat until user hits ESC key

Repeat

print "Press ESC to quit this!"

Until KeyHit(1)
```