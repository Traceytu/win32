---
error-parsing-yaml: 
---

# IScopeAdm::Rescan method

\[Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/library/windows/desktop/aa965362) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.\]

Initiates a full or incremental rescan.

## Syntax


```C++
HRESULT Rescan(
   VARIANT_BOOL fFull
);
```



## Parameters

<dl> <dt>

*fFull* 
</dt> <dd>

If **VARIANT\_TRUE**, this is a full scan of the scope. If **VARIANT\_FALSE**, this is an incremental scan of the scope.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

This method assumes that Indexing Service is already running. It initiates the scanning process and returns control to the caller.

## Requirements



|                                     |                                                            |
|-------------------------------------|------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/> |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>       |
| End of client support<br/>    | Windows 7<br/>                                       |
| End of server support<br/>    | Windows Server 2008 R2<br/>                          |



## See also

<dl> <dt>

[**IScopeAdm**](iscopeadm.md)
</dt> </dl>

 

 




