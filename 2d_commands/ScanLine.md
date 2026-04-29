# ScanLine()

## Parameters

None.

---

## Description

If for some reason you need to know the current scanline location of the  drawing system, here is how you get it.

See also: VWait, Flip.

---

## Example

```blitzbasic
; ScanLine() Example

While Not KeyHit(1)

Print ScanLine()

Wend
```