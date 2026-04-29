# JoyY ([port])

## Parameters

port = number of joystick port to check (optional)

---

## Description

This command returns the value of the x-axis of the joystick. The range  is -1 to 1 (full up to full down). The value returned is a floating point number.  See the example.

---

## Example

```blitzbasic
; JoyX()/JoyY() example

While Not KeyHit(1)

Cls

Text 0,0,"Joy X Value: " + JoyX() + " - Joy Y Value:" + JoyY()

Wend
```