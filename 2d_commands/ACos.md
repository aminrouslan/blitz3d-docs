# ACos# ( c# )

## Parameters

c = a number in the range -1 to +1.

It is considered to be the cosine of an angle.

---

## Description

ACos( c ) is an angle which has cosine = c.

It is in the range 0 to +180 degrees.

---

## Example

```blitzbasic
; ACos example; NaN means "Not a Number", the numerical result is invalid.

Const width = 640, height = 480

Graphics width, height

Local C#, AC#   ; Cos and ACos

Print "    C    ACos( C )"

Print "=================="

For n = -11 To 11

C = n / 10.0

AC = ACos( C ) 

Print RSet(C, 6) + RSet( AC, 10)

Next

WaitKey()  :  End
```