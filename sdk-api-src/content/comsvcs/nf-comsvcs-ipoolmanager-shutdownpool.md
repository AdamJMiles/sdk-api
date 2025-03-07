---
UID: NF:comsvcs.IPoolManager.ShutdownPool
title: IPoolManager::ShutdownPool (comsvcs.h)
description: Shuts down the object pool.
old-location: cos\ipoolmanager_shutdownpool.htm
tech.root: cossdk
ms.assetid: c374b0a4-d984-4fa6-80a7-8bc4d0aff284
ms.date: 12/05/2018
ms.keywords: IPoolManager interface [COM+],ShutdownPool method, IPoolManager.ShutdownPool, IPoolManager::ShutdownPool, ShutdownPool, ShutdownPool method [COM+], ShutdownPool method [COM+],IPoolManager interface, _cos_IPoolManager_ShutdownPool, comsvcs/IPoolManager::ShutdownPool, cos.ipoolmanager_shutdownpool
f1_keywords:
- comsvcs/IPoolManager.ShutdownPool
dev_langs:
- c++
req.header: comsvcs.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- ComSvcs.h
api_name:
- IPoolManager.ShutdownPool
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPoolManager::ShutdownPool


## -description


Shuts down the object pool.


## -parameters




### -param CLSIDOrProgID [in]

A string containing the CLSID or ProgID of the pool to be shut down.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, E_FAIL, and S_OK.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/comsvcs/nn-comsvcs-ipoolmanager">IPoolManager</a>
 

 

