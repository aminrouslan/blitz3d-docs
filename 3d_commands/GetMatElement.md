# GetMatElement# ( entity,row,column )

## Parameters

entity - entity handle

row - matrix row index

column - matrix column index

---

## Description

Returns the value of an element from within an entity's transformation matrix.

The transformation matrix is what is used by Blitz internally to position, scale and rotate entities.

GetMatElement is intended for use by advanced users only.

---

## Example

```blitzbasic
; GetMatElement Example; ---------------------

Graphics3D 640,480

SetBuffer BackBuffer()

camera=CreateCamera()

PositionEntity camera,0,0,-5

light=CreateLight()

RotateEntity light,90,0,0; Create sphere

sphere=CreateSphere(); Position, scale, rotate entity - try messing with these values to change GetMatElement value

PositionEntity sphere,0,0,0

ScaleEntity sphere,1,2,3

RotateEntity sphere,0,0,0

While Not KeyDown(1)

	RenderWorld

	Text 0,0,GetMatElement#(sphere,1,1)

	Flip

Wend

End
```