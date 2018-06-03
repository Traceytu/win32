---
title: Security Descriptor
description: Stores the security descriptor of a file share.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 98f0c008-8a16-4549-a83c-b31a0d112e16
ms.prod: windows-server-dev
ms.technology: failover-clustering
ms.tgt_platform: multiple
keywords:
- Security Descriptor Failover Cluster ,for file shares
- Security Descriptor Failover Cluster
topic_type:
- apiref
api_name:
- Security Descriptor
api_type:
- NA
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Security Descriptor

\[

The **Security Descriptor** property is no longer available for use as of Windows Server 2012.



| Attribute | Value                                                            |
|-----------|------------------------------------------------------------------|
| Data type | Byte array                                                       |
| Access    | [Read/write](read-write-properties.md) (see Remarks)            |
| Structure | [**CLUSPROP\_BINARY**](/previous-versions/windows/desktop/api/ClusAPI/ns-clusapi-clusprop_binary)                      |
| Maximum   | None (but see [Maximum Property Size](maximum-string-size.md).) |
| Default   | 0                                                                |



 

\]

This property is not supported.

**Windows Server 2003:  **

Stores the [security descriptor](https://msdn.microsoft.com/library/windows/desktop/aa379563) of a [file share](file-share.md). The following table summarizes the attributes of the **Security Descriptor** property.

## Remarks

Although the property value is read/write, the underlying security descriptor can be changed only through the [Access Control](https://msdn.microsoft.com/library/windows/desktop/aa374860) or [Network Management](https://msdn.microsoft.com/library/windows/desktop/aa370672) APIs.

To change the value of the **Security Descriptor** property.

-   Retrieve the value of the property.
-   Assign the value to a [**SECURITY\_DESCRIPTOR**](https://msdn.microsoft.com/library/windows/desktop/aa379561) structure.
-   Pass the value to any Access Control or Network Management API function that will change the discretionary access control list (DACL) of the descriptor, such as [**SetSecurityDescriptorDacl**](https://msdn.microsoft.com/library/windows/desktop/aa379583) or [**NetShareSetInfo**](https://msdn.microsoft.com/library/windows/desktop/bb525389).
-   Once the value has been modified, update the **Security Descriptor** property.
-   Take the [File Share](file-share.md) resource offline and bring it back online to activate the new security settings.

**Note**  When you use Cluster Administrator to create a new File Share resource, permissions for the "Everyone" group for that file share are set to read-only by default. However, if you use cluster.exe or the Cluster API to create the File Share resource, permissions for the "Everyone" group for that file share are set to full control by default. You can modify this property as previously described to change the default permissions.

## Requirements



|                                     |                                                                           |
|-------------------------------------|---------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                 |
| Minimum supported server<br/> | Windows Server 2003 Enterprise, Windows Server 2003 Datacenter<br/> |
| End of server support<br/>    | Windows Server 2003 Datacenter, Windows Server 2003 Enterprise<br/> |



## See also

<dl> <dt>

[File Share Private Properties](file-share-private-properties.md)
</dt> <dt>

[Access Control](https://msdn.microsoft.com/library/windows/desktop/aa374860)
</dt> <dt>

[**CLUSPROP\_BINARY**](/previous-versions/windows/desktop/api/ClusAPI/ns-clusapi-clusprop_binary)
</dt> <dt>

[Network Management](https://msdn.microsoft.com/library/windows/desktop/aa370672)
</dt> <dt>

[**NetShareSetInfo**](https://msdn.microsoft.com/library/windows/desktop/bb525389)
</dt> <dt>

[**Security**](file-shares-security.md)
</dt> <dt>

[**SECURITY\_DESCRIPTOR**](https://msdn.microsoft.com/library/windows/desktop/aa379561)
</dt> <dt>

[**SetSecurityDescriptorDacl**](https://msdn.microsoft.com/library/windows/desktop/aa379583)
</dt> </dl>

 

 




