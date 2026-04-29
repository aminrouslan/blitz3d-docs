# Input$ (prompt$)

## Parameters

prompt$ = any valid string (optional)

---

## Description

This command will retrieve a string value from the user with an optional  prompt on the screen (if not in a graphic mode) or on the current drawing buffer  being used by the program. Usually you will assign this command's value to a  string for later use.

---

## Example

```blitzbasic
; Get the user's name and print a welcome

name$=Input$("What is your name?")

Write "Hello there, " + name$ + "!"
```