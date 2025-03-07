---
UID: NF:setupapi.SetupDiGetClassRegistryPropertyW
title: SetupDiGetClassRegistryPropertyW function (setupapi.h)
description: The SetupDiGetClassRegistryProperty function retrieves a property for a specified device setup class from the registry.
old-location: devinst\setupdigetclassregistryproperty.htm
tech.root: devinst
ms.assetid: 79a600af-15c1-4afc-a2cd-568b97d979dc
ms.date: 12/05/2018
ms.keywords: SetupDiGetClassRegistryProperty, SetupDiGetClassRegistryProperty function [Device and Driver Installation], SetupDiGetClassRegistryPropertyA, SetupDiGetClassRegistryPropertyW, devinst.setupdigetclassregistryproperty, di-rtns_98a6c47a-6fb5-4752-9f0e-23ad00f4e5f2.xml, setupapi/SetupDiGetClassRegistryProperty
f1_keywords:
- setupapi/SetupDiGetClassRegistryProperty
dev_langs:
- c++
req.header: setupapi.h
req.include-header: Setupapi.h
req.target-type: DesktopFor universal, call CM_Get_Class_Registry_Property
req.target-min-winverclnt: Available in Windows XP and later versions of Windows.
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
req.lib: Setupapi.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- LibDef
api_location:
- Setupapi.lib
- Setupapi.dll
api_name:
- SetupDiGetClassRegistryProperty - SetupDiGetClassRegistryPropertyW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# SetupDiGetClassRegistryPropertyW function


## -description


The <b>SetupDiGetClassRegistryProperty</b> function retrieves a property for a specified <a href="https://docs.microsoft.com/windows/desktop/api/setupapi/ns-setupapi-sp_devinfo_data">device setup class</a> from the registry.


## -parameters




### -param ClassGuid [in]

A pointer to a GUID representing the device setup class for which a property is to be retrieved.


### -param Property [in]

A value that identifies the property to be retrieved. This must be one of the following values:





#### SPCRP_CHARACTERISTICS

The function returns flags indicating device characteristics for the class. For a list of characteristics flags, see the <i>DeviceCharacteristics</i> parameter to <a href="https://docs.microsoft.com/windows-hardware/drivers/ddi/content/wdm/nf-wdm-iocreatedevice">IoCreateDevice</a>.



#### SPCRP_DEVTYPE

The function returns a DWORD value that represents the device type for the class. For more information, see <a href="https://docs.microsoft.com/windows-hardware/drivers/kernel/specifying-device-types">Specifying Device Types</a>.



#### SPCRP_EXCLUSIVE

The function returns a DWORD value indicating whether users can obtain exclusive access to devices for this class. The returned value is one if exclusive access is allowed, or zero otherwise.



#### SPCRP_LOWERFILTERS

(Windows Vista and later) The function returns a REG_MULTI_SZ list of the service names of the lower filter drivers that are installed for the device setup class.



#### SPCRP_SECURITY

The function returns the device's security descriptor as a SECURITY_DESCRIPTOR structure in self-relative format (described in the Microsoft Windows SDK documentation).



#### SPCRP_SECURITY_SDS

The function returns the device's security descriptor as a text string. For information about security descriptor strings, see <a href="https://docs.microsoft.com/windows/desktop/SecAuthZ/security-descriptor-definition-language">Security Descriptor Definition Language (Windows)</a>. For information about the format of security descriptor strings, see Security Descriptor Definition Language (Windows).



#### SPCRP_UPPERFILTERS

(Windows Vista and later) The function returns a REG_MULTI_SZ list of the service names of the upper filter drivers that are installed for the device setup class.


### -param PropertyRegDataType [out, optional]

A pointer to a variable of type DWORD that receives the property data type as one of the REG_-prefixed registry data types. This parameter is optional and can be <b>NULL</b>. If this parameter is <b>NULL</b>, S<b>etupDiGetClassRegistryProperty</b> does not return the data type.


### -param PropertyBuffer [out]

A pointer to a buffer that receives the requested property. 


### -param PropertyBufferSize [in]

The size, in bytes, of the <i>PropertyBuffer </i>buffer.


### -param RequiredSize [out, optional]

A pointer to a variable of type DWORD that receives the required size, in bytes, of the <i>PropertyBuffer </i>buffer. If the <i>PropertyBuffer</i> buffer is too small, and <i>RequiredSize</i> is not <b>NULL</b>, the function sets <i>RequiredSize</i> to the minimum buffer size that is required to receive the requested property.


### -param MachineName [in, optional]

A pointer to a NULL-terminated string that contains the name of a remote system from which to retrieve the specified device class property. This parameter is optional and can be <b>NULL</b>. If this parameter is <b>NULL</b>, the property is retrieved from the local system.


### -param Reserved

Reserved, must be <b>NULL</b>.


##### - Property.SPCRP_CHARACTERISTICS

The function returns flags indicating device characteristics for the class. For a list of characteristics flags, see the <i>DeviceCharacteristics</i> parameter to <a href="https://docs.microsoft.com/windows-hardware/drivers/ddi/content/wdm/nf-wdm-iocreatedevice">IoCreateDevice</a>.


##### - Property.SPCRP_DEVTYPE

The function returns a DWORD value that represents the device type for the class. For more information, see <a href="https://docs.microsoft.com/windows-hardware/drivers/kernel/specifying-device-types">Specifying Device Types</a>.


##### - Property.SPCRP_EXCLUSIVE

The function returns a DWORD value indicating whether users can obtain exclusive access to devices for this class. The returned value is one if exclusive access is allowed, or zero otherwise.


##### - Property.SPCRP_LOWERFILTERS

(Windows Vista and later) The function returns a REG_MULTI_SZ list of the service names of the lower filter drivers that are installed for the device setup class.


##### - Property.SPCRP_SECURITY

The function returns the device's security descriptor as a SECURITY_DESCRIPTOR structure in self-relative format (described in the Microsoft Windows SDK documentation).


##### - Property.SPCRP_SECURITY_SDS

The function returns the device's security descriptor as a text string. For information about security descriptor strings, see <a href="https://docs.microsoft.com/windows/desktop/SecAuthZ/security-descriptor-definition-language">Security Descriptor Definition Language (Windows)</a>. For information about the format of security descriptor strings, see Security Descriptor Definition Language (Windows).


##### - Property.SPCRP_UPPERFILTERS

(Windows Vista and later) The function returns a REG_MULTI_SZ list of the service names of the upper filter drivers that are installed for the device setup class.


## -returns



The function returns <b>TRUE</b> if it is successful. Otherwise, it returns <b>FALSE</b> and the logged error can be retrieved with a call to <a href="https://go.microsoft.com/fwlink/p/?linkid=169416">GetLastError</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdigetdeviceregistrypropertya">SetupDiGetDeviceRegistryProperty</a>



<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdisetclassregistrypropertya">SetupDiSetClassRegistryProperty</a>



<a href="https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdisetdeviceregistrypropertya">SetupDiSetDeviceRegistryProperty</a>
 

 

