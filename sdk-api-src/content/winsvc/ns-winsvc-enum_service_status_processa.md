---
UID: NS:winsvc._ENUM_SERVICE_STATUS_PROCESSA
title: ENUM_SERVICE_STATUS_PROCESSA (winsvc.h)
description: Contains the name of a service in a service control manager database and information about the service. It is used by the EnumServicesStatusEx function.
old-location: base\enum_service_status_process_str.htm
tech.root: Services
ms.assetid: 6a683cc8-c2ac-4093-aed7-33e6bdd02d79
ms.date: 12/05/2018
ms.keywords: '*LPENUM_SERVICE_STATUS_PROCESSA, ENUM_SERVICE_STATUS_PROCESS, ENUM_SERVICE_STATUS_PROCESS structure, ENUM_SERVICE_STATUS_PROCESSA, ENUM_SERVICE_STATUS_PROCESSW, LPENUM_SERVICE_STATUS_PROCESS, LPENUM_SERVICE_STATUS_PROCESS structure pointer, _win32_enum_service_status_process_str, base.enum_service_status_process_str, winsvc/ENUM_SERVICE_STATUS_PROCESS, winsvc/ENUM_SERVICE_STATUS_PROCESSA, winsvc/ENUM_SERVICE_STATUS_PROCESSW, winsvc/LPENUM_SERVICE_STATUS_PROCESS'
f1_keywords:
- winsvc/ENUM_SERVICE_STATUS_PROCESS
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
req.unicode-ansi: ENUM_SERVICE_STATUS_PROCESSW (Unicode) and ENUM_SERVICE_STATUS_PROCESSA (ANSI)
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
- ENUM_SERVICE_STATUS_PROCESS
- ENUM_SERVICE_STATUS_PROCESSA
- ENUM_SERVICE_STATUS_PROCESSW
targetos: Windows
req.typenames: ENUM_SERVICE_STATUS_PROCESSA, *LPENUM_SERVICE_STATUS_PROCESSA
req.redist: 
ms.custom: 19H1
---

# ENUM_SERVICE_STATUS_PROCESSA structure


## -description


Contains the name of a service in a service control manager database and information about the service. It is used by the 
<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-enumservicesstatusexa">EnumServicesStatusEx</a> function.


## -struct-fields




### -field lpServiceName

The name of a service in the service control manager database. The maximum string length is 256 characters. The service control manager database preserves the case of the characters, but service name comparisons are always case insensitive. A slash (/), backslash (\), comma, and space are invalid service name characters.


### -field lpDisplayName

A display name that can be used by service control programs, such as Services in Control Panel, to identify the service. This string has a maximum length of 256 characters. The case is preserved in the service control manager. Display name comparisons are always case-insensitive.


### -field ServiceStatusProcess

A 
<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/ns-winsvc-service_status_process">SERVICE_STATUS_PROCESS</a> structure that contains status information for the <b>lpServiceName</b> service.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/nf-winsvc-enumservicesstatusexa">EnumServicesStatusEx</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winsvc/ns-winsvc-service_status_process">SERVICE_STATUS_PROCESS</a>
 

 

