---
title: IPOP3Transport CommandDELE method
description: Sends the DELE command to the server for the specified message or messages.
ms.assetid: '03cfe4c4-76e4-45cc-969a-295119c784cf'
keywords: ["CommandDELE method Windows Mail (formerly Outlook Express)", "CommandDELE method Windows Mail (formerly Outlook Express) , IPOP3Transport interface", "IPOP3Transport interface Windows Mail (formerly Outlook Express) , CommandDELE method"]
topic_type:
- apiref
api_name:
- IPOP3Transport.CommandDELE
api_location:
- Inetcomm.dll
api_type:
- COM
---

# IPOP3Transport::CommandDELE method

\[**IPOP3Transport::CommandDELE** is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions.\]

Sends the DELE command to the server for the specified message or messages.

## Syntax


```C++
HRESULT CommandDELE(
  [in]�POP3CMDTYPE cmdtype,
  [in]�DWORD ������dwPopId
);
```



## Parameters

<dl> <dt>

*cmdtype* \[in\]
</dt> <dd>

Type: **[**POP3CMDTYPE**](oe-pop3cmdtype.md)**

Specifies a [**POP3CMDTYPE**](oe-pop3cmdtype.md) value that indicates how to apply the command.

</dd> <dt>

*dwPopId* \[in\]
</dt> <dd>

Type: **DWORD**

Specifies a **DWORD** that contains the ID of the message to mark for deletion. This parameter can be **NULL** when the *cmdtype* is [**POP3CMD\_GET\_MARKED**](oe-pop3cmdtype.md) or **POP3CMD\_GET\_ALL**.

</dd> </dl>

## Return value

Type: **HRESULT**

Returns one of the following values.



| Return code                                                                                                        | Description                                                                                   |
|--------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>                               | Indicates success. <br/>                                                                |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>                       | Indicates that *cmdtype* is [**POP3\_NONE**](oe-pop3cmdtype.md) or is invalid. <br/>   |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl>                      | Indicates that an attempt to allocate memory failed. <br/>                              |
| <dl> <dt>**IXP\_E\_NOT\_INIT**</dt> </dl>                   | Indicates that a connection to the server has not been established. <br/>               |
| <dl> <dt>**IXP\_E\_BUSY**</dt> </dl>                        | Indicates that the server connection is busy. <br/>                                     |
| <dl> <dt>**IXP\_E\_POP3\_POPID\_OUT\_OF\_RANGE**</dt> </dl> | Indicates that *dwPopId* is invalid. <br/>                                              |
| <dl> <dt>**IXP\_E\_POP3\_NEED\_STAT**</dt> </dl>            | Indicates that status has not been requested from the server during this session. <br/> |
| <dl> <dt>**IXP\_E\_POP3\_NO\_MESSAGES**</dt> </dl>          | Indicates that there are no messages. <br/>                                             |
| <dl> <dt>**IXP\_E\_POP3\_NO\_MARKED\_MESSAGES**</dt> </dl>  | Indicates that no messages are marked for this command. <br/>                           |
| <dl> <dt>**IXP\_E\_SOCKET\_WRITE\_ERROR**</dt> </dl>        | Indicates that a transmission error occurred. <br/>                                     |



�

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP \[desktop apps only\]<br/>                                                                    |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                           |
| Product<br/>                  | Outlook Express 6.0<br/>                                                                                 |
| Header<br/>                   | <dl> <dt>Imnxport.h</dt> </dl>                          |
| IDL<br/>                      | <dl> <dt>Imnxport.idl</dt> </dl>                        |
| DLL<br/>                      | <dl> <dt>Inetcomm.dll (version 6.0 or later)</dt> </dl> |



�

�




