# RSet$ (string$, length)

## Parameters

string$ = any valid string or string variable

length = how long you want the new string to be (including padding)

---

## Description

If you have a string that is say, 10 letters long, but you want to make  it a full 25 letters, padding the rest of the string with spaces, this command  will do so, leaving the original string value right justified. You could use  this to pad your high score names to make sure all are the same width in characters.

---

## Example

```blitzbasic
name$="Shane R. Monroe"

Print "New Padded Name: '" + RSet$(name$,40) + "'"
```