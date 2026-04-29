# ScaleSprite sprite,x_scale#,y_scale#

## Parameters

sprite - sprite handle

x_scale# - x scale of sprite

y scale# - y scale of sprite

---

## Description

Scales a sprite.

See also: LoadSprite, CreateSprite.

---

## Example

```blitzbasic
Graphics3D 640,480

cam = CreateCamera()

MoveEntity cam,0,0,-5

sp = CreateSprite()

size# = 1.0

While Not KeyDown(1)

RenderWorld:Flip

ScaleSprite sp,size,size

size = size + 0.01

Wend

End
```