# JoyHit (button,[port])

## Parameters

button = number of joystick button to check

port = number of joystick port to check (optional)

---

## Description

This command returns the number of times a specified joystick button has  been hit since the last time you called the JoyHit() command. Also see KeyHit and MouseHit.

---

## Example

```blitzbasic
; JoyHit Example; Set up the timer

current=MilliSecs()

Print "Press FireButton 1 a bunch of times for five seconds..."; Wait 5 seconds

While MilliSecs() < current+5000

Wend; Print the results

Print "Pressed button " + JoyHit(1) + " times."
```