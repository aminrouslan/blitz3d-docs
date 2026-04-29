# GFXModeWidth (mode)

## Parameters

None.

---

## Description

Once you determine the video modes available by the video card using CountGFXModes(), you can iterate through them  and determine the width, height, and color depth capabilities of each mode.  Use this command to get the width of the mode. Use the GFXModeHeight and  GFXModeDepth to get the remaining parameters.

---

## Example

```blitzbasic
; CountGFXModes()/GfxModeWidth/GfxModeHeight/GfxModeDepth example

intModes=CountGfxModes()

Print "There are " + intModes + "graphic modes available:"; Display all modes including width, height, and color depth

For t = 1 To intModes

Print "Mode " + t + ":

Print "Width=" + GfxModeWidth(t)

Print "Height=" + GfxModeHeight(t)

Print "Height=" + GfxModeDepth(t)

Next
```