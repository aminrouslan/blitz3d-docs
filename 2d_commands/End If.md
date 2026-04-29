# End If

## Parameters

None.

---

## Description

END IF signals the end of an IF THEN condition check. See IF for more information. You can also use ENDIF as a single  word command - it functions identically.

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