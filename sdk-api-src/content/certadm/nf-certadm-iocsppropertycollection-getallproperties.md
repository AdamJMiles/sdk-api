---
UID: NF:certadm.IOCSPPropertyCollection.GetAllProperties
title: IOCSPPropertyCollection::GetAllProperties (certadm.h)
description: Gets all properties in a property set.
old-location: security\iocsppropertycollection_getallproperties_method.htm
tech.root: SecCrypto
ms.assetid: 46a20d55-a673-4f9b-9fb9-bfc631d70f99
ms.date: 12/05/2018
ms.keywords: GetAllProperties, GetAllProperties method [Security], GetAllProperties method [Security],IOCSPPropertyCollection interface, IOCSPPropertyCollection interface [Security],GetAllProperties method, IOCSPPropertyCollection.GetAllProperties, IOCSPPropertyCollection::GetAllProperties, certadm/IOCSPPropertyCollection::GetAllProperties, security.iocsppropertycollection_getallproperties_method
f1_keywords:
- certadm/IOCSPPropertyCollection.GetAllProperties
dev_langs:
- c++
req.header: certadm.h
req.include-header: Certserv.h
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 Datacenter, Windows Server 2008 Enterprise [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Certadm.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Certadm.lib
req.dll: Certadm.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Certadm.dll
api_name:
- IOCSPPropertyCollection.GetAllProperties
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOCSPPropertyCollection::GetAllProperties


## -description


The <b>GetAllProperties</b> method gets all properties in a property set.


## -parameters




### -param pVarProperties [out]

A pointer to a safe array that contains the properties as name-value pairs.

This array is a two-dimensional array of elements, each of type <b>VARIANT</b>. The array contains one row for each named property in the collection. Each row contains two columns: the property name and the property value.


## -returns



<h3>C++</h3>
If the method succeeds, it returns <b>S_OK</b>.


If the method fails, it returns an <b>HRESULT</b> value that indicates the error. For a list of common error codes, see <a href="https://docs.microsoft.com/windows/desktop/SecCrypto/common-hresult-values">Common HRESULT Values</a>.

<h3>VB</h3>
A safe array that contains the properties as name-value pairs.

This array is a two-dimensional array of elements, each of type <b>Variant</b>. The array contains one row for each named property in the collection. Each row contains two columns: the property name and the property value.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/certadm/nn-certadm-iocsppropertycollection">IOCSPPropertyCollection</a>
 

 

