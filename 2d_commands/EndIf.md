# EndIf

## Parameters

None.

---

## Description

Terminates an IF ... THEN condition  structure. See END IF for more information.

See also: If, Then, Else, ElseIf, Select.

---

## Example

```blitzbasic
; IF THEN Example; Input the user's name

name$=Input$("What is your name? "); Doesn't the person's name equal SHANE?

If name$ = "Shane" Then

	Print "You are recognized, Shane! Welcome!"

Else

	Print "Sorry, you don't belong here!"; End of the condition checking

EndIf
```