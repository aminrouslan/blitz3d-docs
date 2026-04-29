# Sgn (number)

## Parameters

number=float or integer

---

## Description

This function is used to determine whether a number or value is greater  than 0, equal to 0 or less than 0. Note: non-integer values return the sign  to 7 signigicant figures. (e.g. -1.000000)

---

## Example

```blitzbasic
Print Sgn(10) ; prints 1

Print Sgn(5.5) ; prints 1.000000

Print Sgn(0) ; prints 0

Print Sgn(0.0) ; prints 0.000000

Print Sgn(-5.5) ; prints -1.000000

Print Sgn(-10) ; prints -1
```