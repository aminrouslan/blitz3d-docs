# CountChildren ( entity )

## Parameters

entity - entity handle

---

## Description

Returns the number of children of an entity.

---

## Example

```blitzbasic
If CountChildren(entity) > 0

For childcount = 1 to CountChildren(entity)

child = GetChild(entity,childcount)

Next

Endif
```