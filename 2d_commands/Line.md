# Line x,y,x1,y1

## Parameters

x=starting x location of the line

y=starting y location of the line

x1=ending x location of the line

y1=ending y location of the line

---

## Description

This command draws a line, in the current drawing color, from one point  on the screen to another (from the x,y to x1,y1 location). See example.

---

## Example

```blitzbasic
; Line example

Graphics 800,600,16; Wait for ESC to hit

While Not KeyHit(1); Set a random color

Color Rnd(255),Rnd(255),Rnd(255); Draw a random line

Line Rnd(800),Rnd(600),Rnd(800),Rnd(600)

Wend
```