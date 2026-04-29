# PokeFloat bank,offset,value

## Parameters

bank - bank handle

offset - offset in bytes, that the poke operation will be started at

value - value that will be written to bank

---

## Description

Writes a float into a memory bank.

A float takes up four bytes of a memory bank.

See also: PokeByte, PokeShort, PokeInt.

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