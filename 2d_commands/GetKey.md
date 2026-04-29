# GetKey()

## Parameters

None

---

## Description

This command will check to see if a key has been pressed and will return  its ASCII value. Not all keys have ASCII values - if you need to trap SHIFT,  ALT, or other non-ASCII compliant key, try KeyHit or KeyDown.

---

## Example

```blitzbasic
; GetKey Example

Print "Please press any ASCII key ..."

While Not value

value=GetKey()

Wend 

Print "You pressed key with an ASCII value of:" + value
```