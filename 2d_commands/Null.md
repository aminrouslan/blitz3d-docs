# Null

## Parameters

None

---

## Description

Designates a Null Type object. Useful for making a Type variable point to nothing or checking if a Type object exists.  Also, useful for checking that there are still objects left on the end of a Type list using the After command.

Can used for testing and setting.

See also: Type, New, Delete, After, Before, First, Last.

---

## Example

```blitzbasic
; Null example

Type Alien

Field x,y

End Type

a.Alien = New Alien

If a <> Null Then Print "Alien exists!"

Delete a

if a = Null Then Print "Alien gone!"
```