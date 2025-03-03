---
UID: NF:d3d9.IDirect3DVolume9.SetPrivateData
title: IDirect3DVolume9::SetPrivateData (d3d9.h)
description: Associates data with the volume that is intended for use by the application, not by Direct3D.
old-location: direct3d9\idirect3dvolume9__setprivatedata.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3dvolume9__setprivatedata.htm
ms.date: 12/05/2018
ms.keywords: IDirect3DVolume9 interface [Direct3D 9],SetPrivateData method, IDirect3DVolume9.SetPrivateData, IDirect3DVolume9::SetPrivateData, SetPrivateData, SetPrivateData method [Direct3D 9], SetPrivateData method [Direct3D 9],IDirect3DVolume9 interface, d3d9helper/IDirect3DVolume9::SetPrivateData, direct3d9.idirect3dvolume9__setprivatedata, e78e1093-63e6-c468-61fa-034b8ab6af7a
f1_keywords:
- d3d9/IDirect3DVolume9.SetPrivateData
dev_langs:
- c++
req.header: d3d9.h
req.include-header: D3D9.h
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
req.lib: D3D9.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D9.lib
- D3D9.dll
api_name:
- IDirect3DVolume9.SetPrivateData
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDirect3DVolume9::SetPrivateData


## -description


Associates data with the volume that is intended for use by the application, not by Direct3D.


## -parameters




### -param refguid [in]

Type: <b><a href="http://go.microsoft.com/?linkid=9742306">REFGUID</a></b>

Reference to the globally unique identifier that identifies the private data to set.


### -param pData [in]

Type: <b>const void*</b>

Pointer to a buffer that contains the data to associate with the volume. 


### -param SizeOfData [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">DWORD</a></b>

Size of the buffer at pData in bytes. 


### -param Flags [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types">DWORD</a></b>

Value that describes the type of data being passed, or indicates to the application that the data should be invalidated when the resource changes. 



<table>
<tr>
<th>Item</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<a id="_none_"></a><a id="_NONE_"></a>(none)

</td>
<td width="60%">
If no flags are specified, Direct3D allocates memory to hold the data within the buffer and copies the data into the new buffer. The buffer allocated by Direct3D is automatically freed, as appropriate.

</td>
</tr>
<tr>
<td width="40%">
<a id="D3DSPD_IUNKNOWN"></a><a id="d3dspd_iunknown"></a>D3DSPD_IUNKNOWN

</td>
<td width="60%">
The data at pData is a pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. SizeOfData must be set to the size of a pointer to an <b>IUnknown</b> interface, sizeof(IUnknown*). Direct3D automatically calls <b>IUnknown</b> through pData and IUnknown when the private data is destroyed. Private data will be destroyed by a subsequent call to <b>IDirect3DVolume9::SetPrivateData</b> with the same GUID, a subsequent call to <a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nf-d3d9helper-idirect3dvolume9-freeprivatedata">IDirect3DVolume9::FreePrivateData</a>, or when the <a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nn-d3d9helper-idirect3d9">IDirect3D9</a> object is released. For more information, see Remarks.

</td>
</tr>
</table>
 


## -returns



Type: <b><a href="/windows/win32/com/structure-of-com-error-codes">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be one of the following: D3DERR_INVALIDCALL, E_OUTOFMEMORY.




## -remarks



Direct3D does not manage the memory at pData. If this buffer was dynamically allocated, it is the calling application's responsibility to free the memory.

Data is passed by value, and multiple sets of data can be associated with a single volume.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nn-d3d9helper-idirect3dvolume9">IDirect3DVolume9</a>



<a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nf-d3d9helper-idirect3dvolume9-freeprivatedata">IDirect3DVolume9::FreePrivateData</a>



<a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nf-d3d9helper-idirect3dvolume9-getprivatedata">IDirect3DVolume9::GetPrivateData</a>
 

 

