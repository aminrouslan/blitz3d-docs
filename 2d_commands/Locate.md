# Locate x,y

## Parameters

x=x coordinate on the screen

y=y coordinate on the screen

---

## Description

Sometimes you want to place the PRINT and Input$ commands at a specific location on the screen.  This command locates the 'cursor' to the designated location.

---

## Example

```blitzbasic
; Locate example

strName$=Input$("What is your name?")

Locate 100,200

Print "Hello there, " + strName$

While Not KeyHit(1)

Wend
```