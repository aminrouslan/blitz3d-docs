# False

## Parameters

None.

---

## Description

FALSE is a keyword to denote a negative result in a conditional statement.  Often times, FALSE is implied and doesn't need to be directly referenced - or  a NOT command is used in the comparison. FALSE can also  be used as a RETURN value from aFUNCTION. Also see the TRUE  command. See the example.

See also: True, If, Select, While, Repeat.

---

## Example

```blitzbasic
; FALSE example; Assign test a random number of 0 or 1

test= Rnd(0,1); FALSE is implied because of the NOT

If not test=1 Then

Print "Test was valued at 0"

End If; Let's set test to be false

test=False; Pointlessly test it

If test=False Then

Print "Test is false"

else

print "Test is true"

End If
```