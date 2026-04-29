# Or

## Parameters

None

---

## Description

A logical expression to return a boolean TRUE or FALSE comparison of expressions  or values. Use this to check two expressions or more and act upon its return  value. See the example.

See also: And, Not, Xor.

---

## Example

```blitzbasic
; OR Example

myNum1=Rnd(0,10)

myNum2=Rnd(0,10)

If myNum1 = 0 OR myNum2 = 0 then

print "One of my numbers is a Zero"

end if
```