# EntityRoll# ( entity[,global] )

## Parameters

entity - name of entity that will have roll angle returned

global (optional) - true if the roll angle returned should be relative to 0 rather than a parent entity's  roll angle. False by default.

---

## Description

Returns the roll angle of an entity.

The roll angle is also the z angle of an entity.

---

## Example

```blitzbasic
; EntityRoll Example; -------------------

Graphics3D 640,480

SetBuffer BackBuffer()

camera=CreateCamera()

light=CreateLight()

cone=CreateCone( 32 )

PositionEntity cone,0,0,5

While Not KeyDown( 1 )

pitch#=0

yaw#=0

roll#=0

If KeyDown( 208 )=True Then pitch#=-1

If KeyDown( 200 )=True Then pitch#=1

If KeyDown( 203 )=True Then yaw#=-1

If KeyDown( 205 )=True Then yaw#=1

If KeyDown( 45 )=True Then roll#=-1

If KeyDown( 44 )=True Then roll#=1

TurnEntity cone,pitch#,yaw#,roll#

RenderWorld

Text 0,0,"Use cursor/Z/X keys to turn cone"; Return entity roll angle of cone

Text 0,20,"Roll: "+EntityRoll#( cone )

Flip

Wend

End
```