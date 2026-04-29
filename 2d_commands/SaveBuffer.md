# SaveBuffer (buffer,filename$)

## Parameters

buffer = The buffer to save; FrontBuffer() or BackBuffer()

filename$ = valid Windows path/filename

---

## Description

Typically, this is used to take a screen snapshot. This will save the screen  buffer you specify to a .bmp file you specify. Remember, use the proper name  for the buffer you wish to save; FrontBuffer() for the current visible  screen, and BackBuffer() for the back or invisible drawing buffer. The  filename must be valid Windows filename syntax.

---

## Example

```blitzbasic
; Save the screen when player pushes F10

If KeyHit(10) Then

SaveBuffer(FrontBuffer(),"screenshot.bmp")

End If
```