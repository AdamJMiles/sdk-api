---
UID: NN:tuner.IESCloseMmiEvent
title: IESCloseMmiEvent (tuner.h)
description: Receives CloseMMI events from a Media Sink Device (MSD) device under the Protected Broadcast Driver Architecture (PBDA).
old-location: mstv\iesclosemmievent.htm
tech.root: mstv
ms.assetid: c470fefb-61bb-4315-ad56-ef5bc90a4ac7
ms.date: 12/05/2018
ms.keywords: IESCloseMmiEvent, IESCloseMmiEvent interface [Microsoft TV Technologies], IESCloseMmiEvent interface [Microsoft TV Technologies],described, mstv.iesclosemmievent, tuner/IESCloseMmiEvent
f1_keywords:
- tuner/IESCloseMmiEvent
dev_langs:
- c++
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Tuner.idl
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
- tuner.h
api_name:
- IESCloseMmiEvent
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IESCloseMmiEvent interface


## -description


Receives <b>CloseMMI</b> events from a Media Sink Device (MSD) device under the Protected Broadcast Driver Architecture (PBDA).  The MSD is the device that receives protected content from a Media Transform Device (MTD). This event tells the MTD that the MSD trying to close a man-machine interface (MMI) display, such as a dialog box.
      


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IESCloseMmiEvent</b> interface inherits from <b>IESEvent</b>. <b>IESCloseMmiEvent</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IESCloseMmiEvent</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tuner/nf-tuner-iesclosemmievent-getdialognumber">GetDialogNumber</a>
</td>
<td align="left" width="63%">
Gets the dialog number generated by the MSD to identify this MMI session.
          

</td>
</tr>
</table> 


## -remarks



To declare the interface identifier (IID) for this interface, use the <b>__uuidof</b> operator: <code>__uuidof(IESCloseMmiEvent)</code>.



