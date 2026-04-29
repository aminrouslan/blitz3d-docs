# LSet$ (string$, length)

## Parameters

string$ = any valid string or string variable

length = how long you want the new string to be (including padding)

---

## Description

If you have a string that is say, 10 letters long, but you want to make  it a full 25 letters, padding the rest of the string with spaces, this command  will do so, leaving the original string value left justified.

---

## Example

```blitzbasic
name$="Shane R. Monroe"

Print "New Padded Name: '" + LSet$(name$,40) + "'"
```