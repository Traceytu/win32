---
title: SetGenerationalGuid\_IN structure
description: The SetGenerationalGuid\_IN structure holds the input data for the SetGenerationalGuid method.
ms.assetid: '24568c37-9641-4e3e-b788-f71db4f3f70f'
keywords: ["SetGenerationalGuid_IN structure Storage Devices", "PSetGenerationalGuid_IN structure pointer Storage Devices"]
topic_type:
- apiref
api_name:
- SetGenerationalGuid_IN
api_location:
- iscsiop.h
api_type:
- HeaderDef
---

# SetGenerationalGuid\_IN structure

The SetGenerationalGuid\_IN structure holds the input data for the [SetGenerationalGuid](https://msdn.microsoft.com/library/windows/hardware/ff565678) method.

## Syntax


```C++
typedef struct _SetGenerationalGuid_IN {
  UCHAR GenerationalGuid[16];
} SetGenerationalGuid_IN, *PSetGenerationalGuid_IN;
```



## Members

<dl> <dt>

**GenerationalGuid**
</dt> <dd>

A 16-byte GUID that identifies the version of the information that is currently in the initiator cache.

</dd> </dl>

## Remarks

You must implement this method.

## Requirements



|                   |                                                                                                          |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Iscsiop.h (include Iscsiop.h)</dt> </dl> |



## See also

<dl> <dt>

[SetGenerationalGuid](https://msdn.microsoft.com/library/windows/hardware/ff565678)
</dt> <dt>

[**SetGenerationalGuid\_OUT**](setgenerationalguid-out.md)
</dt> </dl>

�

�

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bstorage\storage%5D:%20SetGenerationalGuid_IN%20structure%20%20RELEASE:%20%283/29/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





