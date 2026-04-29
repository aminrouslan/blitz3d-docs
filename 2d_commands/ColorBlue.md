# ColorBlue()

## Parameters

None.

---

## Description

Use this command to return the blue component of the RGB color of the current  drawing color. Use ColorRed() and ColorGreen() for the other two color components.

---

## Example

```blitzbasic
; Color, ColorRed(), ColorBlue(), ColorGreen() Example; Gotta be in graphics mode

Graphics 640,480; Change the random seed

SeedRnd MilliSecs(); Let's set the color to something random

Color Rnd(0,255),Rnd(0,255),Rnd(0,255); Now let's see what they are!

While Not KeyHit(1)

Text 0,0,"This Text is printed in Red=" + ColorRed() + " Green=" + ColorGreen()  + " Blue=" + ColorBlue() + "!"

Wend
```