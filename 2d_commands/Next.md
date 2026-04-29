# Next

## Parameters

None

---

## Description

This command closes the FOR ... NEXT loop, causing program execution to  start again at the FOR command unless the loop condition has been met (the last  value has been met). Check the example for more info. Note: Do NOT use the FOR  command's variable as a parameter (i.e. NEXT T) as you would in most BASIC languages.  Blitz will automatically match it with the nearest FOR command.

See also: For, To, Step, Each, Exit, While, Repeat.

---

## Example

```blitzbasic
; Print the values 1 through 10

For t = 1 To 10

Print t

Next; Print the values 1,3,5,7,9

For t = 1 To 10 Step 2

Print t

Next
```