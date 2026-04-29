# KeyHit (scancode)

## Parameters

scancode = the scancode for the key to test

---

## Description

This command returns the number of times a specified key has been hit since  the last time you called the KeyHit() command. Check the ScanCodes for a complete listing of scancodes.

---

## Example

```blitzbasic
; KeyHit Example; Set up the timer

current=MilliSecs()

Print "Press ESC a bunch of times for five seconds..."; Wait 5 seconds

While MilliSecs() < current+5000

Wend; Print the results

Print "Pressed ESC " + KeyHit(1) + " times."
```