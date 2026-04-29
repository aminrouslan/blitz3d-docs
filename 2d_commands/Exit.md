# Exit

## Parameters

None

---

## Description

This command will allow you to leave a For .. Next loop as well as many other types of loops prematurely  (assuming a condition was met or other planned event). It exits the IMMEDIATE  loop - you'll need one for each 'nest' of loops you want to exit from.

See also: For, While, Repeat.

---

## Example

```blitzbasic
; EXIT Command sample

For t = 1 To 100

Print t

If t = 50 Then Exit

Next
```