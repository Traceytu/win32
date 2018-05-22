---
title: Setting Access Rights on the Entire Object
description: Certain permissions can be set only for an entire object, such as Delete and List Contents. Operation-specific permissions, such as the Read permission, can also be set for entire object so that they apply to an entire object.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\mbaldwin
ms.assetid: '786357f4-146e-4638-8bd6-82bc1a6640a1'
ms.prod: 'windows-server-dev'
ms.technology: 'active-directory-domain-services'
ms.tgt_platform: multiple
keywords: ["Setting Access Rights on the Entire Object AD", "objects AD , setting access rights on"]
---

# Setting Access Rights on the Entire Object

Certain permissions can be set only for an entire object, such as Delete and List Contents. Operation-specific permissions, such as the Read permission, can also be set for entire object so that they apply to an entire object.

The following procedure can be used to set permissions for an entire object.

**To set permissions for an entire object**

1.  Set [**IADsAccessControlEntry.AceType**](https://msdn.microsoft.com/library/aa705952) to **ADS\_ACETYPE\_ACCESS\_ALLOWED** or **ADS\_ACETYPE\_ACCESS\_DENIED**.
2.  Set [**IADsAccessControlEntry.ObjectType**](https://msdn.microsoft.com/library/aa705952) and **IADsAccessControlEntry.InheritedObjectType** to **NULL**.

For more information about how to create an ACE, see [Setting Access Rights on an Object](setting-access-rights-on-an-object.md).

For more information and a code example that can be used to set an ACE, see [Example Code for Setting an ACE on a Directory Object](example-code-for-setting-an-ace-on-a-directory-object.md).

 

 



