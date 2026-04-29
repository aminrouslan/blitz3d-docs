# ResizeBank bankhandle,new_size

## Parameters

bankhandle = handle assigned to bank when created

new_size = new size of bank in bytes

---

## Description

Resizes a previously created memory bank. Existing bank data is unmodified,  but may be moved in memory. Also see CreateBank, CopyBank, and BankSize.

---

## Example

```blitzbasic
; BankSize, ResizeBank, CopyBank Example; create a bank

bnkTest=CreateBank(5000); Fill it with rand Integers

For t = 0 To 4999

PokeByte bnkTest,t,Rand(9)

Next; Resize the bank

ResizeBank bnkTest,10000; Copy the first half of the bank to the second half

CopyBank bnkTest,0,bnkTest,5000,5000 ; Print final banksize

Print BankSize(bnkTest)
```