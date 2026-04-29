# PeekFloat(bank,offset)

## Parameters

bank - bank handle

offset - offset in bytes, that the peek operation will be started at

---

## Description

Reads a float from a memory bank and returns the value.

A float takes  up four bytes of a memory bank.

See also: PeekByte, PeekShort, PeekInt.

---

## Example

```blitzbasic
; Bank Commands Example; ---------------------

bnkTest=CreateBank(12)

PokeByte bnkTest,0,Rand(255)

PokeShort bnkTest,1,Rand(65535)

PokeInt bnkTest,3,Rand(-2147483648,2147483647)

PokeFloat bnkTest,7,0.5

Print PeekByte(bnkTest,0)

Print PeekShort(bnkTest,1)

Print PeekInt(bnkTest,3)

Print PeekFloat(bnkTest,7)

FreeBank bnkTest
```