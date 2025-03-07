---
UID: NS:shobjidl_core.PREVIEWHANDLERFRAMEINFO
title: PREVIEWHANDLERFRAMEINFO (shobjidl_core.h)
description: Accelerator table structure. Used by IPreviewHandlerFrame::GetWindowContext.
old-location: shell\PREVIEWHANDLERFRAMEINFO.htm
tech.root: shell
ms.assetid: dd93675e-fd69-4fa3-a8e7-5238c27783d8
ms.date: 12/05/2018
ms.keywords: PREVIEWHANDLERFRAMEINFO, PREVIEWHANDLERFRAMEINFO structure [Windows Shell], _shell_PREVIEWHANDLERFRAMEINFO, shell.PREVIEWHANDLERFRAMEINFO, shobjidl_core/PREVIEWHANDLERFRAMEINFO
f1_keywords:
- shobjidl_core/PREVIEWHANDLERFRAMEINFO
dev_langs:
- c++
req.header: shobjidl_core.h
req.include-header: Shobjidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shobjidl.idl
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
- Shobjidl_core.h
api_name:
- PREVIEWHANDLERFRAMEINFO
targetos: Windows
req.typenames: PREVIEWHANDLERFRAMEINFO
req.redist: 
ms.custom: 19H1
---

# PREVIEWHANDLERFRAMEINFO structure


## -description


Accelerator table structure. Used by <a href="https://docs.microsoft.com/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ipreviewhandlerframe-getwindowcontext">IPreviewHandlerFrame::GetWindowContext</a>.


## -struct-fields




### -field haccel

Type: <b>HACCEL</b>

A handle to the accelerator table.


### -field cAccelEntries

Type: <b>UINT</b>

The number of entries in the accelerator table.

