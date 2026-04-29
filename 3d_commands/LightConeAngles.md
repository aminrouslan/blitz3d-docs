# LightConeAngles light,inner_angle#,outer_angle#

## Parameters

light - light handle

inner_angle# - inner angle of cone

outer_angle# - outer angle of cone

---

## Description

Sets the 'cone' angle for a 'spot' light.

The default light cone angles setting  is 0,90.

See also: CreateLight, LightRange, LightColor.

---

## Example

```blitzbasic
Graphics3D 640,480

camera = CreateCamera()

MoveEntity camera,0,0,-40

flat = CreatePlane(10)

TurnEntity flat,-90,0,0

lite = CreateLight(3) ; try different lights 1 to 3

MoveEntity lite,0,0,-15

While Not KeyDown(1)

RenderWorld:Flip

If KeyHit(57) Then ; press SPACEBAR to randomly change the 'cone' of light

LightConeAngles lite, Rand(120),Rand(120)

EndIf

Wend

End
```