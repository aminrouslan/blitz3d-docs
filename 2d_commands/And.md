# And

## Parameters

None.

---

## Description

AND is a logical operator for doing conditional checks of multiple values  and/or expressions. Use this to ensure that two or more conditions are true,  usually in an IF ... THEN conditional.  See example and see OR, NOT, and XOR.

See also: Or, Not, Xor.

---

## Example

```blitzbasic
; AND example

name$=Input$("Enter your name:")

pw$=Input$("Password:")

if name$="Shane" and pw$="bluedog" then

print "Access granted! Welcome!"

else

print "Your name or password was not recognized"

end if
```