---
UID: NF:pla.IDataCollectorSet.get_SerialNumber
title: IDataCollectorSet::get_SerialNumber (pla.h)
description: Retrieves or sets the number of times that this data collector set has been started, including segments.
old-location: pla\idatacollectorset_get_serialnumber.htm
tech.root: PLA
ms.assetid: 92bfd307-362e-4d60-9a61-d2096fbb3d19
ms.date: 12/05/2018
ms.keywords: IDataCollectorSet interface [PLA],SerialNumber property, IDataCollectorSet.SerialNumber, IDataCollectorSet.get_SerialNumber, IDataCollectorSet::SerialNumber, IDataCollectorSet::get_SerialNumber, IDataCollectorSet::put_SerialNumber, SerialNumber property [PLA], SerialNumber property [PLA],IDataCollectorSet interface, base.idatacollectorset_get_serialnumber, get_SerialNumber, pla.idatacollectorset_get_serialnumber, pla/IDataCollectorSet::SerialNumber, pla/IDataCollectorSet::get_SerialNumber, pla/IDataCollectorSet::put_SerialNumber
f1_keywords:
- pla/IDataCollectorSet.SerialNumber
dev_langs:
- c++
req.header: pla.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
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
req.dll: Pla.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Pla.dll
api_name:
- IDataCollectorSet.SerialNumber
- IDataCollectorSet.get_SerialNumber
- IDataCollectorSet.put_SerialNumber
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDataCollectorSet::get_SerialNumber


## -description


Retrieves or sets the number of times that this data collector set has been started, including segments.

This property is read/write.


## -parameters


## -remarks



Use this property if the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/pla/nf-pla-idatacollectorset-get_subdirectoryformat">IDataCollectorSet::SubdirectoryFormat</a> property is set to <b>plaSerialNumber</b>.

PLA increments the serial number after using it.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/pla/nn-pla-idatacollectorset">IDataCollectorSet</a>
 

 

