# MouseZ()

## Parameters

None.

---

## Description

MouseZ returns the current position of the mouse wheel on a suitable mouse.  It starts off at zero when your program begins. The value of MouseZ increases  as you move the wheel away from you and decreases as you move it towards you.

See also: MouseX, MouseY.

---

## Example

```blitzbasic
Graphics 640, 480, 0, 2

SetBuffer BackBuffer ()

Repeat

Flip:Cls

Text 20, 20, "Mouse wheel position: " + MouseZ ()

Until KeyHit (1)

End
```