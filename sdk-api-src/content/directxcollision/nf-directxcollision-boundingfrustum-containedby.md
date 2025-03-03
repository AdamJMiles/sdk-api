---
UID: NF:directxcollision.BoundingFrustum.ContainedBy
title: BoundingFrustum::ContainedBy
description: Tests whether the BoundingFrustum is contained by the specified frustum.
old-location: dxmath\boundingfrustum_containedby.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.directxmath.BoundingFrustum.ContainedBy(XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR,XMVECTOR)
ms.date: 12/05/2018
ms.keywords: BoundingFrustum interface [DirectX Math Support APIs],ContainedBy method, BoundingFrustum.ContainedBy, BoundingFrustum::ContainedBy, ContainedBy, ContainedBy method [DirectX Math Support APIs], ContainedBy method [DirectX Math Support APIs],BoundingFrustum interface, dxmath.boundingfrustum_containedby
f1_keywords:
- directxcollision/BoundingFrustum.ContainedBy
dev_langs:
- c++
req.header: directxcollision.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
- DirectXCollision.h
api_name:
- BoundingFrustum.ContainedBy
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# BoundingFrustum::ContainedBy


## -description


Tests whether the [BoundingFrustum](/windows/win32/api/directxcollision/ns-directxcollision-boundingfrustum) is contained by the specified frustum.


## -parameters




### -param Plane0 [in]

A plane describing the frustum.


### -param Plane1 [in]

A plane describing the frustum.


### -param Plane2 [in]

A plane describing the frustum.


### -param Plane3 [in]

A plane describing the frustum.


### -param Plane4 [in]

A plane describing the frustum.


### -param Plane5 [in]

A plane describing the frustum.


## -returns



A <a href="https://msdn.microsoft.com/edc456b5-2d68-4d4e-953b-6081ad7f663c">ContainmentType</a> value indicating whether the frustum contains the [BoundingFrustum](/windows/win32/api/directxcollision/ns-directxcollision-boundingfrustum).




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




[BoundingFrustum](/windows/win32/api/directxcollision/ns-directxcollision-boundingfrustum)



<a href="https://msdn.microsoft.com/85A76263-92C4-4AF1-BFDE-C68A30CD5583">Methods</a>



<b>Reference</b>
 

 

