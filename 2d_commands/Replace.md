# Replace$ (string$, find$, replace$)

## Parameters

string$ = any valid string variable

find$ = any valid string

replace$ = any valid string

---

## Description

This command will allow you to replace characters within a string with another.  Use this to strip or convert letters out of your strings (like removing spaces  or turning them into underscores). Pretty straight forward.

---

## Example

```blitzbasic
name$="Bill Wallace"

Print "Your name before replacing: " + name$

Print "Your name with L changed to B: " + Replace$(name$,"l","b")
```