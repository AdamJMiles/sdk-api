---
UID: NS:tcpmib._MIB_TCP6TABLE_OWNER_PID
title: MIB_TCP6TABLE_OWNER_PID (tcpmib.h)
description: Contains a table of process IDs (PIDs) and the IPv6 TCP links that are context bound to these PIDs.
old-location: mib\mib_tcp6table_owner_pid.htm
tech.root: MIB
ms.assetid: 93629d1d-e5f2-4ae8-b585-17e39ae4986d
ms.date: 12/05/2018
ms.keywords: '*PMIB_TCP6TABLE_OWNER_PID, MIB_TCP6TABLE_OWNER_PID, MIB_TCP6TABLE_OWNER_PID structure [MIB], PMIB_TCP6TABLE_OWNER_PID, PMIB_TCP6TABLE_OWNER_PID structure pointer [MIB], iprtrmib/MIB_TCP6TABLE_OWNER_PID, iprtrmib/PMIB_TCP6TABLE_OWNER_PID, mib.mib_tcp6table_owner_pid, tcpmib/MIB_TCP6TABLE_OWNER_PID, tcpmib/PMIB_TCP6TABLE_OWNER_PID'
f1_keywords:
- tcpmib/MIB_TCP6TABLE_OWNER_PID
dev_langs:
- c++
req.header: tcpmib.h
req.include-header: Iphlpapi.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2008, Windows Server 2003 with SP1 [desktop apps only]
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
- Tcpmib.h
- Iprtrmib.h
api_name:
- MIB_TCP6TABLE_OWNER_PID
targetos: Windows
req.typenames: MIB_TCP6TABLE_OWNER_PID, *PMIB_TCP6TABLE_OWNER_PID
req.redist: 
ms.custom: 19H1
---

# MIB_TCP6TABLE_OWNER_PID structure


## -description


The <b>MIB_TCP6TABLE_OWNER_PID</b> structure contains a table of process IDs (PIDs)  and the IPv6 TCP links that  are context bound to these PIDs.


## -struct-fields




### -field dwNumEntries

The number of <a href="https://docs.microsoft.com/windows/desktop/api/tcpmib/ns-tcpmib-mib_tcp6row_owner_pid">MIB_TCP6ROW_OWNER_PID</a> elements in the <b>table</b>.


### -field table

Array of <a href="https://docs.microsoft.com/windows/desktop/api/tcpmib/ns-tcpmib-mib_tcp6row_owner_pid">MIB_TCP6ROW_OWNER_PID</a> structures returned by a call to <a href="https://docs.microsoft.com/windows/desktop/api/iphlpapi/nf-iphlpapi-getextendedtcptable">GetExtendedTcpTable</a>.


## -remarks



The <b>MIB_TCP6TABLE_OWNER_PID</b> structure is returned by a call to <a href="https://docs.microsoft.com/windows/desktop/api/iphlpapi/nf-iphlpapi-getextendedtcptable">GetExtendedTcpTable</a> with the <i>TableClass</i> parameter set to <b>TCP_TABLE_OWNER_PID_LISTENER</b>, <b>TCP_TABLE_OWNER_PID_CONNECTIONS</b>, or <b>TCP_TABLE_OWNER_PID_ALL</b> from the <a href="https://docs.microsoft.com/windows/desktop/api/iprtrmib/ne-iprtrmib-tcp_table_class">TCP_TABLE_CLASS</a> enumeration and the <i>ulAf</i> parameter set to <b>AF_INET6</b>.

The <b>MIB_TCP6TABLE_OWNER_PID</b> structure may contain padding for alignment between the <b>dwNumEntries</b> member and the first <a href="https://docs.microsoft.com/windows/desktop/api/tcpmib/ns-tcpmib-mib_tcp6row_owner_pid">MIB_TCP6ROW_OWNER_PID</a> array entry in the <b>table</b> member. Padding for alignment may also be present between the <b>MIB_TCP6ROW_OWNER_PID</b> array entries in the <b>table</b> member. Any access to a <b>MIB_TCP6ROW_OWNER_PID</b> array entry should assume  padding may exist. 



On the Microsoft Windows Software Development Kit (SDK) released for Windows Vistaand later, the organization of header files has changed. This  structure is defined in the <i>Tcpmib.h</i> header file, not in the <i>Iprtrmib.h</i> header file. Note that the <i>Tcpmib.h</i> header file is automatically included in <i>Iprtrmib.h</i>, which is automatically included in the <i>Iphlpapi.h</i> header file. The  <i>Tcpmib.h</i> and <i>Iprtrmib.h</i> header files should never be used directly.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/IpHlp/ip-helper-start-page">IP Helper Start Page</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mib/management-information-base-reference">MIB Reference</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/mib/mib-structures">MIB Structures</a>
 

 

