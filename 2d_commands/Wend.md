# Wend

## Parameters

None.

---

## Description

This is the command that tells program execution to branch to the beginning  of the WHILE/WEND loop at the WHILE command. See the WHILE  command for complete details.

See also: While, Exit, Repeat, For.

---

## Example

```blitzbasic
; While/Wend Example; The loop condition is at the TOP of the loop

While Not KeyHit(1) ; As long as the user hasn't hit ESC yet ...

Print "Press Esc to end this mess!" ; Print this

Wend ; Go back to the start of the WHILE loop
```