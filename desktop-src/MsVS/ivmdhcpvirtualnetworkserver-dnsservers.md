---
error-parsing-yaml: 
---

# IVMDHCPVirtualNetworkServer::DNSServers property

The **DNSServers** property contains a comma-separated list of the TCP/IP address representing DNS servers. The list of DNS servers is returned to the DHCP client as part of the server's response.

This property is read/write.

## Syntax


```C++
HRESULT put_DNSServers(
  [in]  BSTR dnsServers
);

HRESULT get_DNSServers(
  [out] BSTR *dnsServers
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
<td><pre><code>VMDHCPVirtualNetworkServer.DNSServers( _
  ByRef dnsServers, _
  ByVal dnsServers _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

Contains a comma-separated list of TCP/IP addresses formatted as a string in dotted-decimal notation. For example, 10.237.0.3,10.237.0.4.

This property value is read/write.

## Error codes



| Name                                                                                                   | Meaning                                                                |
|--------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>                       | The operation was successful.<br/>                               |
| <dl> <dt>E\_POINTER</dt> </dl>                  | The *dnsServers* parameter was **NULL**.<br/>                    |
| <dl> <dt>E\_INVALIDARG</dt> </dl>               | The *dnsServers* parameter was an empty string.<br/>             |
| <dl> <dt>VM\_E\_INVALID\_IP\_ADDRESS</dt> </dl> | The *dnsServers* parameter contained an invalid IP address.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl>          | An unexpected error has occurred.<br/>                           |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMDHCPVirtualNetworkServer**](ivmdhcpvirtualnetworkserver.md)
</dt> </dl>

 

 




