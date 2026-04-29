# Each type_variable

## Parameters

type_variable = A previously declared TYPE object

---

## Description

If you haven't read up on the TYPE command, you might  want to do so before continuing.

The For .. Each loop allows you to walk through each object in the Type collection.  This is perfect for updating a large group of objects (such as a group of alien  invaders). Do look over the Type command.

See also: Type, New, Before, After, First, Last, Insert, Delete.

---

## Example

```blitzbasic
; Move them all over 1 (like the description example from TYPE command)

For room.chair = Each chair

room\x = room\x + 1

Next
```