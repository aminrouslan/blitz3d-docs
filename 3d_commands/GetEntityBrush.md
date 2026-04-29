# GetEntityBrush(entity)

## Parameters

entity - entity handle

---

## Description

Returns a brush with the same properties as is applied to the specified entity.

If this command does not appear to be returning a valid brush, try using 
GetSurfaceBrush
 instead with the first surface available.

Remember, GetEntityBrush actually creates a new brush so don't forget to free it afterwards using FreeBrush to prevent memory leaks.

Once you have got the brush handle from an entity, you can use GetBrushTexture and TextureName to get the details of what texture(s) are applied to the brush.

See also: GetSurfaceBrush, FreeBrush, GetBrushTexture, TextureName.

---
