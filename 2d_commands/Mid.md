# Mid$ (string$, offset, characters)

## Parameters

string$ = any valid string

offset = location within the string to start reading

characters = how many characters to read frm the offset point

---

## Description

Use this command to grab a set of characters from within a string. You can  choose WHERE to start in the string, and how many characters to pick. You'll  probably use this to 'decode' or 'walk through' a string to get each character  out of it for conversion or validation. See the Example.

---

## Example

```blitzbasic
name$="Shane Monroe"

For T = 1 To Len(name$)

Print Mid$(name$,t,1)

Next
```