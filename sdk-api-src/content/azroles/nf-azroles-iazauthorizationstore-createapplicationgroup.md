---
UID: NF:azroles.IAzAuthorizationStore.CreateApplicationGroup
title: IAzAuthorizationStore::CreateApplicationGroup (azroles.h)
description: Creates an IAzApplicationGroup object with the specified name.
old-location: security\azauthorizationstore_createapplicationgroup.htm
tech.root: SecAuthZ
ms.assetid: d9a78aaa-189b-4878-a5ba-fb6fb8927c5e
ms.date: 12/05/2018
ms.keywords: AzAuthorizationStore object [Security],CreateApplicationGroup method, CreateApplicationGroup, CreateApplicationGroup method [Security], CreateApplicationGroup method [Security],AzAuthorizationStore object, CreateApplicationGroup method [Security],IAzAuthorizationStore interface, IAzAuthorizationStore interface [Security],CreateApplicationGroup method, IAzAuthorizationStore.CreateApplicationGroup, IAzAuthorizationStore::CreateApplicationGroup, azroles/IAzAuthorizationStore::CreateApplicationGroup, security.azauthorizationstore_createapplicationgroup
f1_keywords:
- azroles/AzAuthorizationStore.CreateApplicationGroup
dev_langs:
- c++
req.header: azroles.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Azroles.lib
req.dll: Azroles.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Azroles.dll
api_name:
- AzAuthorizationStore.CreateApplicationGroup
- IAzAuthorizationStore.CreateApplicationGroup
targetos: Windows
req.typenames: 
req.redist: Windows Server 2003 Administration Tools Pack on Windows XP
ms.custom: 19H1
---

# IAzAuthorizationStore::CreateApplicationGroup


## -description


The <b>CreateApplicationGroup</b> method creates an <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iazapplicationgroup">IAzApplicationGroup</a> object with the specified name.


## -parameters




### -param bstrGroupName [in]

Name for the new <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iazapplicationgroup">IAzApplicationGroup</a> object.


### -param varReserved [in, optional]

Reserved for future use.


### -param ppGroup [out]

A pointer to a pointer to the created <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iazapplicationgroup">IAzApplicationGroup</a> object.


## -returns



 If the method succeeds, the method returns S_OK.

Any other <b>HRESULT</b> value indicates that the operation failed.




## -remarks



You must call the <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nf-azroles-iazapplicationgroup-submit">IAzApplicationGroup::Submit</a> method to persist any changes made to the returned object.

The returned <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iazapplicationgroup">IAzApplicationGroup</a> object is an immediate child object of the <a href="https://docs.microsoft.com/windows/desktop/api/azroles/nn-azroles-iazauthorizationstore">AzAuthorizationStore</a> object.



