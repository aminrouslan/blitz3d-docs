# New type_variable

## Parameters

type_variable = the actual Type name, not the custom Type name

---

## Description

If you aren't familiar with the TYPE command, please refer to that before  reading about this command.

Creates a NEW object in a Type collection. Each call to this command automatically  inserts a new object into the specified Type collection. Check the example and  other Type commands for more information.

See also: Type, Before, After, First, Last, Each, Insert, Delete.

---

## Example

```blitzbasic
; Define the CHAIR Type

Type CHAIR

Field X

Field Y

Field HEIGHT

End Type; Create 100 new chairs using FOR ... NEXT using the collection name of ROOM

For tempx = 1 to 10

For tempy = 1 to 10

room.chair = New Chair

room\x = tempx

room\y = tempy

room\height = Rnd(0,10) ; set a random height 0 to 10

Next

Next
```