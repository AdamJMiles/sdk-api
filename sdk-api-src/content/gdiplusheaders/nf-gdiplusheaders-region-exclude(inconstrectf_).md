---
UID: NF:gdiplusheaders.Region.Exclude(IN const RectF &)
title: Region::Exclude(IN const RectF &) (gdiplusheaders.h)
description: The Region::Exclude method updates this region to the portion of itself that does not intersect the specified rectangle's interior.
old-location: gdiplus\_gdiplus_CLASS_Region_Exclude_RectF_rect_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\regionclass\regionmethods\regionexcludemethods\exclude_59rectfamprect.htm
ms.date: 12/05/2018
ms.keywords: Exclude, Exclude method [GDI+], Exclude method [GDI+],Region class, Region class [GDI+],Exclude method, Region.Exclude, Region.Exclude(IN const RectF &), Region.Exclude(const RectF&), Region::Exclude, Region::Exclude(IN const RectF &), _gdiplus_CLASS_Region_Exclude_RectF_rect_, gdiplus._gdiplus_CLASS_Region_Exclude_RectF_rect_
f1_keywords:
- gdiplusheaders/Region.Exclude
dev_langs:
- c++
req.header: gdiplusheaders.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
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
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Gdiplus.dll
api_name:
- Region.Exclude
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
ms.custom: 19H1
---

# Region::Exclude(IN const RectF &)


## -description


The <b>Region::Exclude</b> method updates this region to the portion of itself that does not intersect the specified rectangle's interior.


## -parameters




### -param rect [in, ref]

Type: <b>const <a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/nl-gdiplustypes-rectf">RectF</a></b>

Reference to a rectangle to use to update this 
					<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-region">Region</a>object. 


## -returns



Type: <strong>Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a> enumeration.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/nl-gdiplustypes-rectf">RectF</a>



<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-region">Region</a>



<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a>
 

 

