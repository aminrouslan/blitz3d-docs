# EntityOrder entity,order

## Parameters

entity - entity handle

order - order that entity will be drawn in

---

## Description

Sets the drawing order for an entity.

An order value of 0 will mean the  entity is drawn normally. A value greater than 0 will mean that entity is drawn  first, behind everything else. A value less than 0 will mean the entity is drawn  last, in front of everything else. 

Setting an entity's order to non-0 also disables z-buffering for the entity,  so should be only used for simple, convex entities like skyboxes, sprites etc. 

EntityOrder affects the specified entity but none of its child entities,  if any exist.

---
