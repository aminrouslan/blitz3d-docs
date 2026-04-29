# Goto label

## Parameters

label = any valid exisiting label

---

## Description

This branches the flow of the program to a designated label. With the use  of Functions inside of Blitz, it isn't very practical to use Gotos, but you  may still find it useful. If you require the need to return execution back to  the calling statement, you may use Gosub instead. See  the example.

See also: Gosub, Function.

---

## Example

```blitzbasic
Print "The program starts ..."

Goto label1

Print "This line never gets printed .."

End.label1

Print "We just jumped here!"; wait for ESC key before ending

While Not KeyHit(1) 

Wend
```