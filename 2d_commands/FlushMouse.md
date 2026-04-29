# FlushMouse

## Parameters

None.

---

## Description

There are many times when you aren't interested in the dozens of possible  mouse button pressed the player might have made before you are checking for  one in particular. Or perhaps you want to pause the game and wait for any mouse  button to be hit, but you don't want a 'queued' button press bypassing this.  Use this command before you specifically want to poll a mouse button hit from  the user.

---

## Example

```blitzbasic
; Flushmouse sample

FlushMouse

Print "Press a mouse button to exit!"

WaitMouse()

End
```