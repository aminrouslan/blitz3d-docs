# CountGfxModes3D()

## Parameters

None.

---

## Description

Returns the number of 3D compatible modes available on the selected 3D graphics card, and sets up the info to be returned by GfxModeWidth, GfxModeHeight, GfxModeDepth etc (see 2D commands). 

Any difference between CountGfxModes3D and CountGfxModes has been made largely irrelevant by newer cards as they now tend to support 3D in all graphics modes. However there are a few older cards that do not support 3D in some graphics modes, hence the inclusion of the CountGfxModes3D command.

---

## Example

```blitzbasic
; CountGfxModes3D(); -----------------

Graphics 800,600,0,2

For i=1 To CountGfxModes3D()

	Print "Mode "+i+": ("+GfxModeWidth(i)+"x"+GfxModeHeight(i)+"x"+GfxModeDepth(i)+")"

Next

WaitKey()
```