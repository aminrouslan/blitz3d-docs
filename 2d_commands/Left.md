# Left$ (string$, length)

## Parameters

string$ = any valid string variable

length = a valid integer value up to the length of the string.

---

## Description

Use this command to get a certain number of the leftmost letters of a string.  You will use this to truncate strings to make them fit somewhere, or to control  the number of characters input.

---

## Example

```blitzbasic
name$="Shane Monroe"

Print "The left 3 letters of your name are: " + Left$(name$,3)
```