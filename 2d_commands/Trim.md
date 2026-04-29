# Trim$( string$ )

## Parameters

string$ - any valid string

---

## Description

This function removes leading and trailing spaces from the specified string.

---

## Example

```blitzbasic
Graphics 640,480,0,2

a$ = "  Weeeeee  "

Text 0,0,a$

Text 0,20,Trim$(a$)

WaitKey()
```