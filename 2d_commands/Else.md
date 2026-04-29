# Else

## Parameters

None.

---

## Description

There are times during an IF ...  THEN conditional that you will want code to execute in the event that the  conditional is NOT met. The ELSE command begins that block of code, and is terminated  by the END IF command. See example.

See also: If, Then, ElseIf, EndIf, Select.

---

## Example

```blitzbasic
; ELSE example 

name$=Input$("What is your name?") 

If name$="Shane" then 

	Print "Hello Shane!" 

Else 

	Print "I have NO clue who you are!" 

End If
```