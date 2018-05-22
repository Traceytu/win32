---
title: LVM\_SUBITEMHITTEST message
description: Determines which list-view item or subitem is at a given position. You can send this message explicitly or by using the ListView\_SubItemHitTest macro.
ms.assetid: '1468febb-af0d-4c04-b0b1-cda5ec77aa2c'
keywords: ["LVM_SUBITEMHITTEST message Windows Controls"]
topic_type:
- apiref
api_name:
- LVM_SUBITEMHITTEST
api_location:
- Commctrl.h
api_type:
- HeaderDef
---

# LVM\_SUBITEMHITTEST message

Determines which list-view item or subitem is at a given position. You can send this message explicitly or by using the [**ListView\_SubItemHitTest**](listview-subitemhittest.md) macro.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>Must be 0. **Windows Vista.** Should be -1 if the **iGroup** member of *lParam* is to be retrieved.</dd> <dt>

*lParam* 
</dt> <dd>

Pointer to an [**LVHITTESTINFO**](lvhittestinfo.md) structure. The [**POINT**](https://msdn.microsoft.com/library/windows/desktop/dd162805) structure within **LVHITTESTINFO** should be set to the client coordinates to be hit-tested.

</dd> </dl>

## Return value

Returns the index of the item or subitem tested, if any, or -1 otherwise. If an item or subitem is at the given coordinates, the fields of the [**LVHITTESTINFO**](lvhittestinfo.md) structure will be filled with the applicable hit information.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



�

�




