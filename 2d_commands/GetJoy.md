# GetJoy ([port])

## Parameters

port = optional joystick port to read

---

## Description

Unlike the other similar commands (JoyDown and JoyHit), this command doesn't need to know which button  you are trying to test for. It looks for any joystick button, then returns the  number the user pressed. Since you are polling all the buttons instead of just  a specific one, this may be a tad less efficient than using JoyDown or JoyHit.  Use this command in conjunction with Select/Case  for maximum efficiency!

---

## Example

```blitzbasic
; GetJoy Example

While Not KeyHit(1)

button=GetJoy()

If button <> 0 Then

Print "You pressed joystick button #" + button

End If

Wend
```