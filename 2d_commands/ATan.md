# ATan# ( t# )

## Parameters

t = any number.

It is considered to be the tangent of an angle.

---

## Description

ATan( t ) is an angle which has tangent = t.

It is in the range -90 to +90 degrees.

See also ATan2 for an extended version with 360 degree range.

---

## Example

```blitzbasic
; ATan example

Const width = 640, height = 480

Graphics width, height

Local T#, AT#   ; Tan and ATan

zero# = 0

Print "       T      ATan( T )"

Print "======================="; First, an extreme case...

T# = 1 / zero    ; +Infinity

AT = ATan( T ) 

Print RSet(T, 10) + RSet( AT, 11); Now, back to normal usage...

For n = -10 To 10

T = Sgn( n ) * n * n

AT = ATan( T ) 

Print RSet(T, 10) + RSet( AT, 11)

Next; Finally, another extreme case.

T# = -1 / zero    ; -Infinity

AT = ATan( T ) 

Print RSet(T, 10) + RSet( AT, 11)

WaitKey()  :  End
```