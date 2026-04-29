# Else If

## Parameters

None.

---

## Description

During a standard IF ... THEN conditional structure, you may wish to check another condition if the original condition fails. This 'nested IF' situation can get WAY out of hand, and once you have more than two nested conditionals, you should consider a SELECT/CASE structure. See the example.

See also: ElseIf.

---

## Example

```blitzbasic
; ELSEIF Example; Input the user's name

name$=Input$("What is your name? "); Doesn't the person's name equal SHANE?

If name$ = "Shane" Then

	Print "You are recognized, Shane! Welcome!"

ElseIf name$="Ron" Then

	Print "You are recognized too, Ron! Welcome!"

Else

	Print "Sorry, you don't belong here!"; End of the condition checking

End If
```