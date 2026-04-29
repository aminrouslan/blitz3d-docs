# ClearSurface surface,[clear_verts][,clear_triangles]

## Parameters

surface - surface handle

clear_verts (optional) - true to remove all vertices from the specified surface,  false not to. Defaults to true.

clear_triangles (optional) - true to remove all triangles from the specified  surface, false not to. Defaults to true.

---

## Description

Removes all vertices and/or triangles from a surface.

This is useful for  clearing sections of mesh. The results will be instantly visible. 

After clearing a surface, you may wish to add vertices and triangles to it  again but with a slightly different polygon count for dynamic level of detail  (LOD).

---
