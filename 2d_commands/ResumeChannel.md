# ResumeChannel channel

## Parameters

channel - a music or sound channel previously allocated via LoadSound, PlayMusic,  etc.

---

## Description

ResumeChannel is used to continue the playing of a sound sample or music  track on the given channel after you have temporarily halted playback on that  channel (via PauseChannel).

---

## Example

```blitzbasic
Graphics 640, 480, 0, 2

musicchannel = PlayMusic ("oohyeahbaby.mp3") ; Replace with a music file on  your hard drive!

Repeat

    Print "Press a key to pause the music..."

    WaitKey

    PauseChannel musicchannel

    Print "Press a key to continue the music..."

    WaitKey

    ResumeChannel musicchannel

Until KeyHit (1)

End
```