# Step

## Parameters

None.

---

## Description

Use this to tell your FOR ... NEXT  loop to increment a certain value each pass through the loop. STEP 1 is assumed  and need not be declared. STEP 2 would skip every other value, STEP 3 would  skip every third value, etc.

See also: For, To, Each, Next, Exit, While, Repeat.

---

## Example

```blitzbasic
; Print 1 through 100, by tens

For t = 1 To 100 Step 10

Print t

Next
```