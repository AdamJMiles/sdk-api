---
UID: NS:mprapi._RAS_USER_0
title: RAS_USER_0 (mprapi.h)
description: The RAS_USER_0 structure contains information for a particular Remote Access Service user.
old-location: rras\ras_user_0.htm
tech.root: RRAS
ms.assetid: f034c6c2-2dac-40bf-b810-9bf6f3eb3c41
ms.date: 12/05/2018
ms.keywords: '*PRAS_USER_0, PRAS_USER_0, PRAS_USER_0 structure pointer [RAS], RASPRIV_AdminSetCallback, RASPRIV_CallerSetCallback, RASPRIV_DialinPrivilege, RASPRIV_NoCallback, RAS_USER_0, RAS_USER_0 structure [RAS], _mpr_ras_user_0, mprapi/PRAS_USER_0, mprapi/RAS_USER_0, rras.ras_user_0'
f1_keywords:
- mprapi/RAS_USER_0
dev_langs:
- c++
req.header: mprapi.h
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
- HeaderDef
api_location:
- Mprapi.h
api_name:
- RAS_USER_0
targetos: Windows
req.typenames: RAS_USER_0, *PRAS_USER_0
req.redist: 
ms.custom: 19H1
---

# RAS_USER_0 structure


## -description


The 
<b>RAS_USER_0</b> structure contains information for a particular Remote Access Service user.


## -struct-fields




### -field bfPrivilege

Specifies the types of remote access privilege available to the RAS user. 




The following remote access privilege constants are defined in Mprapi.h.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="RASPRIV_DialinPrivilege"></a><a id="raspriv_dialinprivilege"></a><a id="RASPRIV_DIALINPRIVILEGE"></a><dl>
<dt><b>RASPRIV_DialinPrivilege</b></dt>
</dl>
</td>
<td width="60%">
The user has permission to dial in to the RAS server.

</td>
</tr>
<tr>
<td width="40%"><a id="RASPRIV_NoCallback"></a><a id="raspriv_nocallback"></a><a id="RASPRIV_NOCALLBACK"></a><dl>
<dt><b>RASPRIV_NoCallback</b></dt>
</dl>
</td>
<td width="60%">
The RAS server will not call back the user to establish a connection.

</td>
</tr>
<tr>
<td width="40%"><a id="RASPRIV_AdminSetCallback"></a><a id="raspriv_adminsetcallback"></a><a id="RASPRIV_ADMINSETCALLBACK"></a><dl>
<dt><b>RASPRIV_AdminSetCallback</b></dt>
</dl>
</td>
<td width="60%">
When the user calls, the RAS server hangs up and calls a preset call-back phone number stored in the user account database. The <b>wszPhoneNumber</b> member of the 
<b>RAS_USER_0</b> structure contains the user's call-back phone number.

</td>
</tr>
<tr>
<td width="40%"><a id="RASPRIV_CallerSetCallback"></a><a id="raspriv_callersetcallback"></a><a id="RASPRIV_CALLERSETCALLBACK"></a><dl>
<dt><b>RASPRIV_CallerSetCallback</b></dt>
</dl>
</td>
<td width="60%">
When the user calls, the RAS server provides the option of specifying a call-back phone number. The user can also choose to connect immediately without a call back. The <b>wszPhoneNumber</b> member contains a default number that the user can override.

</td>
</tr>
</table>
 


<div> </div>


Use the following constant as a mask to isolate the call-back privilege. (This constant is also defined in Mprapi.h.)

RASPRIV_CallbackType


### -field wszPhoneNumber

Pointer to a Unicode string containing the phone number at which the RAS user should be called back.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mprapi/nf-mprapi-mpradminusergetinfo">MprAdminUserGetInfo</a>



<a href="https://docs.microsoft.com/windows/desktop/api/mprapi/nf-mprapi-mpradminusersetinfo">MprAdminUserSetInfo</a>



<a href="https://docs.microsoft.com/windows/desktop/RRAS/ras-administration-structures">RAS
		  Administration Structures</a>



<a href="https://docs.microsoft.com/windows/desktop/api/mprapi/ns-mprapi-ras_user_1">RAS_USER_1</a>



<a href="https://docs.microsoft.com/windows/desktop/RRAS/remote-access-service-administration-reference">Remote Access Service Administration Reference</a>
 

 

