# TotalVidMem()

## Parameters

None.

---

## Description

TotalVidMem () simply returns the total available memory on a graphics  card, in bytes. Note that to retrieve the currently available number  of bytes, you should use AvailVidMem ().

---

## Example

```blitzbasic
Print "Total graphics memory available: " + TotalVidMem () + " bytes."; NOTE: To retrieve the *available* graphics memory, use AvailVidMem ()!
```