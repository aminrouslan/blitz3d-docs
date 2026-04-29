# PointEntity entity,target[,roll#]

## Parameters

entity - entity handle

target - target entity handle

roll# (optional) - roll angle of entity

---

## Description

Points one entity at another.

The optional roll parameter allows you to  specify a roll angle as pointing an entity only sets pitch and yaw angles. 

If you wish for an entity to point at a certain position rather than another  entity, simply create a pivot entity at your desired position, point the entity  at this and then free the pivot.

---
