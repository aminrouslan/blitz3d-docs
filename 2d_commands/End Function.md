# End Function

## Parameters

None.

---

## Description

This line terminates a FUNCTION structure. Upon  reaching this line, Blitz will branch program execution to the next command  following the original call to the function. See the  FUNCTION command for more information.

---

## Example

```blitzbasic
; End Function Example; Get the user's name

name$=Input$("Enter Your Name:"); Call a function to print how many letters the name has

numletters(name$);;The program basically ends here, because functions don't run unless called.; The actual function

Function numletters(passedname$)

Print "Your name has " + Len(passedname$) + " letters in it."

End Function
```