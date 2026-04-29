# AppTitle title$[,close_prompt$]

## Parameters

title$ - the text that will be displayed in the title bar of the program  window

close_prompt$ (optional) - the text that will be displayed in a message box  with 'OK/Cancel' options when a user clicks on the close button. If nothing  is specified, the message box will not be displayed and the program will close  immediately.

---

## Description

Allows you to set the text of the program's title bar, and 'close program?'  message box.

---

## Example

```blitzbasic
; Set the title bar

AppTitle "Super Invaders V1.0", "Are you sure?"
```