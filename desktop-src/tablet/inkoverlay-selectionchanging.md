---
Description: 'Occurs when the selection of ink within the control is about to change, such as through alterations to the user interface, cut-and-paste procedures, or the Selection property.'
ms.assetid: 'dffdb183-d363-40d3-81a2-d496433f7075'
title: 'InkOverlay.SelectionChanging event'
---

# InkOverlay.SelectionChanging event

Occurs when the selection of ink within the control is about to change, such as through alterations to the user interface, cut-and-paste procedures, or the [**Selection**](inkoverlay-selection.md) property.

## Syntax


```C++
void SelectionChanging(
  [in]�IInkStrokes *NewSelection
);
```



## Parameters

<dl> <dt>

*NewSelection* \[in\]
</dt> <dd>

The new collection of [InkStrokes](inkstrokes-collection.md) that is being selected.

</dd> </dl>

## Return value

This event does not return a value.

## Remarks

This event method is defined in the \_IInkOverlayEvents and \_IInkPictureEvents dispatch-only interfaces (dispinterfaces) with an ID of DISPID\_IOESelectionChanging.

## Requirements



|                                     |                                                                                                                     |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP Tablet PC Edition \[desktop apps only\]<br/>                                                       |
| Minimum supported server<br/> | None supported<br/>                                                                                           |
| Header<br/>                   | <dl> <dt>Msinkaut.h (also requires Msinkaut\_i.c)</dt> </dl> |
| Library<br/>                  | <dl> <dt>InkObj.dll</dt> </dl>                               |



## See also

<dl> <dt>

[**InkOverlay Class**](inkoverlay-class.md)
</dt> <dt>

[**Selection Property**](inkoverlay-selection.md)
</dt> </dl>

�

�



