# LoadSprite ( tex_file$[,tex_flag][,parent] )

## Parameters

text_file$ - filename of image file to be used as sprite

tex_flag (optional) - texture flag:

1: Color

2: Alpha

4: Masked

8: Mipmapped

16: Clamp U

32: Clamp V

64: Spherical reflection map

parent - parent of entity

---

## Description

Creates a sprite entity, and assigns a texture to it.

See also: LoadSprite, RotateSprite, ScaleSprite, HandleSprite, SpriteViewMode, PositionEntity, MoveEntity, TranslateEntity, EntityAlpha, FreeEntity.

---

## Example

```blitzbasic
Graphics3D 640,480

campivot = CreatePivot()

cam = CreateCamera(campivot)

MoveEntity cam,0,0,-5

sp = LoadSprite("grass.bmp")

SpriteViewMode sp,4

While Not KeyDown(1)

RenderWorld:Flip

TurnEntity campivot,1,1,3

Wend

End
```