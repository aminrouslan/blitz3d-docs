# SetBuffer buffer

## Parameters

Buffers can either be the FrontBuffer(), BackBuffer() or an ImageBuffer()  Default buffer is the FrontBuffer

---

## Description

Use this command to set the current drawing buffer. If not used the default  buffer, FrontBuffer() is used. SetBuffer also resets the origin to 0,0 and the  Viewpoint to the width and height of the buffer.

---

## Example

```blitzbasic
SetBuffer FrontBuffer() ;Sets FrontBuffer as the current drawing buffer
```