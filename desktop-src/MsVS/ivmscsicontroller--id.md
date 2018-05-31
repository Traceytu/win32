---
error-parsing-yaml: 
---

# IVMSCSIController::\_ID property

The **\_ID** property contains an internal ID number for this SCSI controller.

This property is read-only.

## Syntax


```C++
HRESULT get__ID(
  [out] long *identifier
);
```



## Property value

The internal ID number for this SCSI controller.

## Error codes



| Name                                                                                           | Meaning                                             |
|------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| <dl> <dt> S\_OK</dt> </dl>              | The operation was successful.<br/>            |
| <dl> <dt>E\_POINTER</dt> </dl>          | The parameter *identifier* was **NULL**.<br/> |
| <dl> <dt> DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error has occurred.<br/>        |



## Remarks

Not usable by scripting languages.

## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMSCSIController**](ivmscsicontroller.md)
</dt> </dl>

 

 




