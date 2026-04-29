# SoundPan sound_variable,pan#

## Parameters

sound_variable = any valid sound variable previously created with the  LoadSound command.

pan# = floating point number from -1 (left) to 0 (center) to 1 (right)

---

## Description

Use this command to pan your sound effect between the left and right speakers  (or restore the panning to the center). Use this for cool panning stereo sounds  during your game.

---

## Example

```blitzbasic
; Load sound sample

sndDeath=LoadSound("audiodeath.wav"); Pan sound effect half to the left

SoundPan sndDeath,-.5; Play sound

PlaySound sndDeath
```