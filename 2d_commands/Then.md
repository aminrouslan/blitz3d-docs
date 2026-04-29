# Then

## Parameters

None.

---

## Description

Used in an IF statement to denote the end of the conditional  to be checked. Famous for its participation in the IF ... THEN structure. See  example and IF statement for more information.

See also: If, Else, ElseIf, EndIf, Select.

---

## Example

```blitzbasic
; IF THEN Example; Input the user's name

name$=Input$("What is your name? "); Doesn't the person's name equal SHANE?

If name$ = "Shane" Then

	Print "You are recognized, Shane! Welcome!"

Else

	Print "Sorry, you don't belong here!"; End of the condition checking

End If
```