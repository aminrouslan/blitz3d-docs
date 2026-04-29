# HideEntity entity

## Parameters

entity - entity handle

---

## Description

Hides an entity, so that it is no longer visible, and is no longer involved  in collisions.

The main purpose of hide entity is to allow you to create entities  at the beginning of a program, hide them, then copy them and show as necessary  in the main game. This is more efficient than creating entities mid-game. 

If you wish to hide an entity so that it is no longer visible but still involved  in collisions, then use EntityAlpha 0 instead.  This will make an entity completely transparent. 

HideEntity affects the specified entity and all of its child entities, if  any exist.

---
