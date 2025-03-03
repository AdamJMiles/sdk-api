---
UID: NS:winsvc._SERVICE_DESCRIPTIONW
title: SERVICE_DESCRIPTIONW (winsvc.h)
description: Contains a service description.
old-location: base\service_description_str.htm
tech.root: Services
ms.assetid: 1b4e18d5-6086-4d1b-b39c-1d919bfdc0b9
ms.date: 12/05/2018
ms.keywords: '*LPSERVICE_DESCRIPTIONW, LPSERVICE_DESCRIPTION, LPSERVICE_DESCRIPTION structure pointer, SERVICE_DESCRIPTION, SERVICE_DESCRIPTION structure, SERVICE_DESCRIPTIONA, SERVICE_DESCRIPTIONW, _win32_service_description_str, base.service_description_str, winsvc/LPSERVICE_DESCRIPTION, winsvc/SERVICE_DESCRIPTION, winsvc/SERVICE_DESCRIPTIONA, winsvc/SERVICE_DESCRIPTIONW'
f1_keywords:
- winsvc/SERVICE_DESCRIPTION
dev_langs:
- c++
req.header: winsvc.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: SERVICE_DESCRIPTIONW (Unicode) and SERVICE_DESCRIPTIONA (ANSI)
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
- HeaderDef
api_location:
- Winsvc.h
api_name:
- SERVICE_DESCRIPTION
- SERVICE_DESCRIPTIONA
- SERVICE_DESCRIPTIONW
targetos: Windows
req.typenames: SERVICE_DESCRIPTIONW, *LPSERVICE_DESCRIPTIONW
req.redist: 
ms.custom: 19H1
---

# SERVICE_DESCRIPTIONW structure


## -description


Contains a service description.


## -struct-fields




### -field lpDescription

The description of the service. If this member is <b>NULL</b>, the description remains unchanged. If this value is an empty string (""), the current description is deleted. 




The service description must not exceed the size of a registry value of type <b>REG_SZ</b>.

This member can specify a localized string using the following format:

@[<i>path</i>\]<i>dllname</i>,-<i>strID</i>

The string with identifier <i>strID</i> is loaded from <i>dllname</i>; the <i>path</i> is optional. For more information, see <a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regloadmuistringa">RegLoadMUIString</a>.

<b>Windows Server 2003 and Windows XP:  </b>Localized strings are not supported until Windows Vista.


## -remarks



A description of <b>NULL</b> indicates no service description exists. The service description is NULL when the service is created.

The description is simply a comment that explains the purpose of the service. For example, for the DHCP service, you could use the description "Provides internet addresses for computer on your network."

You can set the description using the 
<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-changeserviceconfig2a">ChangeServiceConfig2</a> function. You can retrieve the description using the 
<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-queryserviceconfig2a">QueryServiceConfig2</a> function. The description is also displayed by the Services snap-in.


#### Examples

For an example, see 
<a href="https://docs.microsoft.com/windows/desktop/Services/changing-a-service-configuration">Changing a Service's Configuration</a> or <a href="https://docs.microsoft.com/windows/desktop/Services/querying-a-service-s-configuration">Querying a Service's Configuration</a>.

<div class="code"></div>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-changeserviceconfig2a">ChangeServiceConfig2</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-queryserviceconfig2a">QueryServiceConfig2</a>
 

 

