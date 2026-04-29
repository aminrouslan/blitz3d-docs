# Len (string$)

## Parameters

string$ = any valid string variable

---

## Description

This will let you determine the length (number of letters, spaces, characters,  numbers, etc) inside a string. You can use this to ensure the player enters  the right number of letters (like 3 letters for a high score table). Quite useful  for 'string parsing' with other commands.

---

## Example

```blitzbasic
name$="Shane Monroe"

Print "There are " + Len(name$) + " characters in your name!"
```