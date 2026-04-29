# ClsColor red,green,blue

## Parameters

red, green and blue = number between 0 and 255

---

## Description

This changes the color for subsequent CLS calls. Use  this command when you need CLS to 'clear' the screen with some other color than  black.

---

## Example

```blitzbasic
;set ClsColor to red

ClsColor 255,0,0 ;set current drawing buffer to the color set by the ClsColor command

Cls
```