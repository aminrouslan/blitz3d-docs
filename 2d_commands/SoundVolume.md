# SoundVolume sound_variable,volume#

## Parameters

sound_variable = any valid sound variable previously created with the LoadSound  command.

volume# = floating point number from 0 (silence) to 1 (full volume)

---

## Description

Alter the playback volume of your sound effect with this command. This command  uses a floating point number from 0 to 1 to control the volume level.

Please see ChannelVolume for more options!

---

## Example

```blitzbasic
; Load sound sample

sndDeath=LoadSound("audiodeath.wav"); Change volume level to half

SoundVolume sndDeath,.5; Play sound

PlaySound sndDeath
```