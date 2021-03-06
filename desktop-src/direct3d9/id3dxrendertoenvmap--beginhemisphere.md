---
Description: Initiate the rendering of a hemispheric environment map.
ms.assetid: 1150aad9-dd8c-4943-afaf-90794faaaf70
title: ID3DXRenderToEnvMap::BeginHemisphere method
ms.topic: article
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ID3DXRenderToEnvMap.BeginHemisphere
api_type:
- COM
api_location:
- d3dx9.lib
- d3dx9.dll
---

# ID3DXRenderToEnvMap::BeginHemisphere method

Initiate the rendering of a hemispheric environment map.

## Syntax


```C++
HRESULT BeginHemisphere(
  [in] LPDIRECT3DTEXTURE9 pTexZPos,
  [in] LPDIRECT3DTEXTURE9 pTexZNeg
);
```



## Parameters

<dl> <dt>

*pTexZPos* \[in\]
</dt> <dd>

Type: **[**LPDIRECT3DTEXTURE9**](https://msdn.microsoft.com/library/Bb205909(v=VS.85).aspx)**

Pointer to an [**IDirect3DTexture9**](https://msdn.microsoft.com/library/Bb205909(v=VS.85).aspx) interface that represents the positive texture render surface.

</dd> <dt>

*pTexZNeg* \[in\]
</dt> <dd>

Type: **[**LPDIRECT3DTEXTURE9**](https://msdn.microsoft.com/library/Bb205909(v=VS.85).aspx)**

Pointer to an [**IDirect3DTexture9**](https://msdn.microsoft.com/library/Bb205909(v=VS.85).aspx) interface that represents the negative texture render surface.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/en-us/library/Bb401631(v=MSDN.10).aspx)**

If the method succeeds, the return value is D3D\_OK. If the method fails, the return value can be one of the following: D3DERR\_INVALIDCALL.E\_FAIL

## Remarks

See [**ID3DXRenderToEnvMap::Face**](id3dxrendertoenvmap--face.md) to draw the face.

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx9core.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[ID3DXRenderToEnvMap](id3dxrendertoenvmap.md)
</dt> <dt>

[**ID3DXRenderToEnvMap::End**](id3dxrendertoenvmap--end.md)
</dt> </dl>

 

 




