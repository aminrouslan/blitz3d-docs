# Asc (string$)

## Parameters

string$ = any valid string variable (only the first character's ASCII value  will be returned).

---

## Description

This will return the ASCII value of the first letter of a string.

---

## Example

```blitzbasic
a$=Input$("Enter a letter:")

Print "The ASCII value of the letter is:" + Asc(a$)
```