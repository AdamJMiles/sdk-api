---
UID: NF:d3d10effect.ID3D10Effect.GetConstantBufferByName
title: ID3D10Effect::GetConstantBufferByName (d3d10effect.h)
description: Get a constant buffer by name.
old-location: direct3d10\id3d10effect_getconstantbufferbyname.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effect_getconstantbufferbyname.htm
ms.date: 12/05/2018
ms.keywords: GetConstantBufferByName, GetConstantBufferByName method [Direct3D 10], GetConstantBufferByName method [Direct3D 10],ID3D10Effect interface, ID3D10Effect interface [Direct3D 10],GetConstantBufferByName method, ID3D10Effect.GetConstantBufferByName, ID3D10Effect::GetConstantBufferByName, d3d10effect/ID3D10Effect::GetConstantBufferByName, direct3d10.id3d10effect_getconstantbufferbyname, ee9f35f2-1d6f-f921-a7a3-825ac2b49866
f1_keywords:
- d3d10effect/ID3D10Effect.GetConstantBufferByName
dev_langs:
- c++
req.header: d3d10effect.h
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
- D3D10Effect.h
api_name:
- ID3D10Effect.GetConstantBufferByName
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D10Effect::GetConstantBufferByName


## -description


Get a constant buffer by name.


## -parameters




### -param Name [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">LPCSTR</a></b>

The constant-buffer name.


## -returns



Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/d3d10effect/nn-d3d10effect-id3d10effectconstantbuffer">ID3D10EffectConstantBuffer</a>*</b>

A pointer to the constant buffer indicated by the Name. See <a href="https://docs.microsoft.com/windows/desktop/api/d3d10effect/nn-d3d10effect-id3d10effectconstantbuffer">ID3D10EffectConstantBuffer</a>.




## -remarks



An effect that contains a variable that will be read/written by an application requires at least one constant buffer. For best performance, an effect should organize variables into one or more constant buffers based on their frequency of update.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/d3d10effect/nn-d3d10effect-id3d10effect">ID3D10Effect Interface</a>
 

 

