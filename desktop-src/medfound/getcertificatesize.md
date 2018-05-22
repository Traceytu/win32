﻿---
Description: 'Gets the size of a certificate for a display driver.'
ms.assetid: 'fd52e939-127a-4493-8406-31f7767921cd'
title: GetCertificateSize function
---

# GetCertificateSize function

> \[!Important\]  
> This function is used by [Output Protection Manager](output-protection-manager.md) (OPM) to access functionality in the display driver. Applications should not call this function.

 

Gets the size of a certificate for a display driver.

## Syntax


```C++
NTSTATUS WINAPI GetCertificateSize(
  _In_  PUNICODE_STRING          pstrDeviceName,
  _In_  DXGKMDT_CERTIFICATE_TYPE ctPVPCertificateType,
  _Out_ ULONG                    *pulCertificateLength
);
```



## Parameters

<dl> <dt>

*pstrDeviceName* \[in\]
</dt> <dd>

A pointer to a [**UNICODE\_STRING**](security.unicode_string) structure that contains the name of the display device, as returned by the [**GetMonitorInfo**](gdi.getmonitorinfo) function.

</dd> <dt>

*ctPVPCertificateType* \[in\]
</dt> <dd>

The type of certificate, specified as a member of the **DXGKMDT\_CERTIFICATE\_TYPE** enumeration.

</dd> <dt>

*pulCertificateLength* \[out\]
</dt> <dd>

Receives the size of the certificate, in bytes.

</dd> </dl>

## Return value

If the method succeeds, it returns **STATUS\_SUCCESS**. Otherwise, it returns an **NTSTATUS** error code.

## Remarks

Applications should call the [**IOPMVideoOutput::StartInitialization**](iopmvideooutput-iopmvideooutput--startinitialization.md) method instead of this function.

This function has no associated import library. To call this function, you must use the [**LoadLibrary**](base.loadlibrary) and [**GetProcAddress**](base.getprocaddress) functions to dynamically link to Gdi32.dll.

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                       |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                 |
| DLL<br/>                      | <dl> <dt>Gdi32.dll</dt> </dl> |



## See also

<dl> <dt>

[OPM Functions](opm-functions.md)
</dt> <dt>

[Output Protection Manager](output-protection-manager.md)
</dt> </dl>

 

 



