---
title: StopService method of the CIM\_VirtualSystemManagementService class
description: Stops the service.CIM\_Service.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 1b1fffb7-3f8a-4e3f-ab17-71ae489ee414
ms.prod: windows-server-dev
ms.technology:
- failover-cluster-hyperv
- windows-management-instrumentation
ms.tgt_platform: multiple
keywords:
- StopService method
- StopService method, CIM_VirtualSystemManagementService class
- CIM_VirtualSystemManagementService class, StopService method
topic_type:
- apiref
api_name:
- CIM_VirtualSystemManagementService.StopService
api_location:
- VMMS.exe
api_type:
- COM
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# StopService method of the CIM\_VirtualSystemManagementService class

Stops the service.

The [**StopService**](https://msdn.microsoft.com/library/aa393668) method stops the service represented by the object derived from [**CIM\_Service**](https://msdn.microsoft.com/library/aa388442).

This method is inherited from [**CIM\_Service**](cim-service.md).

## Syntax


```mof
uint32 StopService();
```



## Parameters

This method has no parameters.

## Return value

Returns "0" on success, otherwise returns a WMI error code.

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                              |
| Minimum supported server<br/> | Windows Server 2016<br/>                                                                         |
| Namespace<br/>                | Root\\HyperVCluster\\v2<br/>                                                                     |
| Header<br/>                   | <dl> <dt>Sdoias.h</dt> </dl>                    |
| MOF<br/>                      | <dl> <dt>WindowsHyperVCluster.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>VMMS.exe</dt> </dl>                    |



## See also

<dl> <dt>

[**CIM\_VirtualSystemManagementService**](cim-virtualsystemmanagementservice.md)
</dt> </dl>

 

 




