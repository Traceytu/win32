---
error-parsing-yaml: 
---

# IVMHardDisk::HostFreeDiskSpace property

The **HostFreeDiskSpace** property contains the amount of remaining disk space available on the host computer for the current hard disk image file.

This property is read-only.

## Syntax


```C++
HRESULT get_HostFreeDiskSpace(
  [out] VARIANT *freeBytes
);
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>VMHardDisk.HostFreeDiskSpace( _
  ByRef freeBytes _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The amount of remaining disk space available on the host computer for the current hard disk image file. The number is returned as a **Decimal** value.

This property value is read-only.

## Error codes



| Name                                                                                          | Meaning                                                               |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>              | The operation was successful.<br/>                              |
| <dl> <dt>E\_POINTER</dt> </dl>         | The parameter is **NULL**.<br/>                                 |
| <dl> <dt>E\_BAD\_PATHNAME</dt> </dl>   | The path to the current virtual hard disk file is invalid.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error occurred.<br/>                              |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMHardDisk**](ivmharddisk.md)
</dt> </dl>

 

 




