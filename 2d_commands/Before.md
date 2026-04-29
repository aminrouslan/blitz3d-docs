# Before custom_type_variable

## Parameters

custom_type_variable = not the Type name, but the custom Type name

---

## Description

If you haven't read up on the TYPE command, you might  want to do so before continuing.

Use this to assign a custom Type object to the previous object in the collection.  See the example.

See also: Type, New, After, First, Last, Each, Insert, Delete.

---

## Example

```blitzbasic
; Define a crafts Type

Type crafts

Field x

Field y

Field dead

Field graphic

End Type ; Create 100 crafts, with the unique name of alien

For t = 1 To 100 

alien.crafts = New crafts

alien\x = Rnd(0,640)

alien\y = Rnd(0,480)

alien\dead = 0

alien\graphic = 1

Next ; Move to the first object

alien.crafts = First crafts 

Print alien\x

Print alien\y

Print alien\dead

Print alien\graphic ; move to the next alien object

alien = After alien 

Print alien\x

Print alien\y

Print alien\dead

Print alien\graphic ; move to the last alien object

alien.crafts = Last crafts 

Print alien\x

Print alien\y

Print alien\dead

Print alien\graphic ; move to the second to the last alien object

alien = Before alien 

Print alien\x

Print alien\y

Print alien\dead

Print alien\graphic
```