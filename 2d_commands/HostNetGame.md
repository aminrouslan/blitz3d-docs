# HostNetGame (gamename$)

## Parameters

gamename$ = string value designating the game's name

---

## Description

This allows you to bypass the 'standard' networked game dialog box (normally  using StartNetGame) and start a hosted game directly.  A value of 2 is returned if the hosted game has started successfully.

---

## Example

```blitzbasic
; HostNetGame example

joinResults=HostNetGame("ShaneGame")

Select joinResults

Case 2

Print "Successfully started host game!"

Default

Print "Game was unable to start!"

End Select 

waitkey()
```