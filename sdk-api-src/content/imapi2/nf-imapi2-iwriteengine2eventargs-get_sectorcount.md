---
UID: NF:imapi2.IWriteEngine2EventArgs.get_SectorCount
title: IWriteEngine2EventArgs::get_SectorCount (imapi2.h)
description: Retrieves the number of sectors to write to the device in the current write operation.
old-location: imapi\iwriteengine2eventargs_get_sectorcount.htm
tech.root: imapi
ms.assetid: b23c81c2-792e-45fc-b862-6daf5b1a6fd1
ms.date: 12/05/2018
ms.keywords: IWriteEngine2EventArgs interface [IMAPI],get_SectorCount method, IWriteEngine2EventArgs.get_SectorCount, IWriteEngine2EventArgs::get_SectorCount, get_SectorCount, get_SectorCount method [IMAPI], get_SectorCount method [IMAPI],IWriteEngine2EventArgs interface, imapi.iwriteengine2eventargs_get_sectorcount, imapi2/IWriteEngine2EventArgs::get_SectorCount
f1_keywords:
- imapi2/IWriteEngine2EventArgs.get_SectorCount
dev_langs:
- c++
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
- imapi2.h
api_name:
- IWriteEngine2EventArgs.get_SectorCount
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWriteEngine2EventArgs::get_SectorCount


## -description


Retrieves the number of sectors to write to the device in the current write operation.


## -parameters




### -param value [out]

The number of sectors to write in the current write operation.  


## -returns



S_OK is returned on success, but other success codes may be returned as a result of implementation. The following error codes are commonly returned on operation failure, but do not represent the only possible error values:

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
Pointer is not valid.

Value: 0x80004003

</td>
</tr>
</table>
 




## -remarks



This is the same value passed to the <a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nf-imapi2-iwriteengine2-writesection">IWriteEngine2::WriteSection</a> method. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nf-imapi2-iwriteengine2-writesection">IWriteEngine2::WriteSection</a>



<a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nn-imapi2-iwriteengine2eventargs">IWriteEngine2EventArgs</a>
 

 

