---
Description: The SetPreviewMode method sets the preview mode for the group.
ms.assetid: 40b7e9ac-30b3-454e-82ac-10ac99f1b86f
title: IAMTimelineGroup::SetPreviewMode method
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- IAMTimelineGroup.SetPreviewMode
api_type: 
- COM
api_location: 
- strmiids.lib
- strmiids.dll
---

# IAMTimelineGroup::SetPreviewMode method

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The SetPreviewMode method sets the preview mode for the group.

## Syntax


```C++
HRESULT SetPreviewMode(
   BOOL fPreview
);
```



## Parameters

<dl> <dt>

*fPreview* 
</dt> <dd>

The preview mode. If **TRUE**, the group is in preview mode. If **FALSE**, the group is in authoring mode.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

In preview mode, frames are dropped during slow effects or transitions to keep the video synchronized with the audio. The video might look choppy as a result. In authoring mode, every frame is rendered. Authoring mode is appropriate for writing files; for on-screen preview, the video might be out of sync with the audio.

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](https://go.microsoft.com/fwlink/p/?linkid=129787). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IAMTimelineGroup Interface**](iamtimelinegroup.md)
</dt> <dt>

[Error and Success Codes](error-and-success-codes.md)
</dt> </dl>

 

 




