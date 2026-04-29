# MD2AnimTime ( md2 )

## Parameters

md2 - md2 handle

---

## Description

Returns the animation time of an md2 model.

The animation time is the  exact moment that the md2 is at with regards its frames of animation. For example,  if the md2 at a certain moment in time is moving between the third and fourth  frames, then MD2AnimTime will return a number in the region 3-4.

---

## Example

```blitzbasic
; MD2AnimTime Example; -------------------

Graphics3D 640,480

SetBuffer BackBuffer()

camera=CreateCamera()

light=CreateLight()

RotateEntity light,90,0,0; Load md2

gargoyle=LoadMD2( "media/gargoyle/gargoyle.md2"); Load md2 texture

garg_tex=LoadTexture( "media/gargoyle/gargoyle.bmp" ); Apply md2 texture to md2

EntityTexture gargoyle,garg_tex; Animate md2

AnimateMD2 gargoyle,1,0.1,32,46

PositionEntity gargoyle,0,-45,100

RotateEntity gargoyle,0,180,0

While Not KeyDown( 1 )

UpdateWorld

RenderWorld; Output current animation frame to screen

Text 0,0,"MD2AnimTime: "+MD2AnimTime( gargoyle )

Flip

Wend

End
```