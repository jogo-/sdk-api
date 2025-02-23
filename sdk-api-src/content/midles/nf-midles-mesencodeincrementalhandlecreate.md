---
UID: NF:midles.MesEncodeIncrementalHandleCreate
title: MesEncodeIncrementalHandleCreate function (midles.h)
description: The MesEncodeIncrementalHandleCreate function creates an encoding and then initializes it for the incremental style of serialization.
helpviewer_keywords: ["MesEncodeIncrementalHandleCreate","MesEncodeIncrementalHandleCreate function [RPC]","_rpc_mesencodeincrementalhandlecreate","midles/MesEncodeIncrementalHandleCreate","rpc.mesencodeincrementalhandlecreate"]
old-location: rpc\mesencodeincrementalhandlecreate.htm
tech.root: Rpc
ms.assetid: 54bbe560-08a9-4e41-9121-37aab0c209a9
ms.date: 12/05/2018
ms.keywords: MesEncodeIncrementalHandleCreate, MesEncodeIncrementalHandleCreate function [RPC], _rpc_mesencodeincrementalhandlecreate, midles/MesEncodeIncrementalHandleCreate, rpc.mesencodeincrementalhandlecreate
f1_keywords:
- midles/MesEncodeIncrementalHandleCreate
dev_langs:
- c++
req.header: midles.h
req.include-header: Rpc.h
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
req.lib: Rpcrt4.lib
req.dll: Rpcrt4.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Rpcrt4.dll
api_name:
- MesEncodeIncrementalHandleCreate
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# MesEncodeIncrementalHandleCreate function


## -description


The 
<b>MesEncodeIncrementalHandleCreate</b> function creates an encoding and then initializes it for the incremental style of serialization.


## -parameters




### -param UserState

Pointer to the user-supplied state object that coordinates the user-supplied <b>Alloc</b>, <b>Write</b>, and <b>Read</b> functions.


### -param AllocFn

Pointer to the user-supplied <b>Alloc</b> function.


### -param WriteFn

Pointer to the user-supplied <b>Write</b> function.


### -param pHandle

Pointer to the newly created handle.


## -returns



<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_OK</b></dt>
</dl>
</td>
<td width="60%">
The call succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_INVALID_ARG</b></dt>
</dl>
</td>
<td width="60%">
The argument was invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_S_OUT_OF_MEMORY</b></dt>
</dl>
</td>
<td width="60%">
Out of memory.

</td>
</tr>
</table>
 

<div class="alert"><b>Note</b>  For a list of valid error codes, see 
<a href="https://docs.microsoft.com/windows/desktop/Rpc/rpc-return-values">RPC Return Values</a>.</div>
<div> </div>



## -remarks



The 
<b>MesEncodeIncrementalHandleCreate</b> function is used by applications to create and initialize the handle for the incremental style of encoding or decoding. When using the incremental style of encoding, the user supplies an <b>Alloc</b> function to provide an empty buffer into which the encoded data is placed, and a <b>Write</b> function to call when the buffer is full or the encoding is complete. For additional information on the user-supplied <b>Alloc</b>, <b>Write</b>, and <b>Read</b> functions, see 
<a href="https://docs.microsoft.com/windows/desktop/Rpc/serialization-services">Serialization Services</a>.

When a stub is compiled using <b>-protocol all</b> or <b>-protocol ndr64</b> and the buffer is to be encoded using the NDR64 transfer syntax, the 
<a href="https://docs.microsoft.com/windows/desktop/api/midles/nf-midles-mesbufferhandlereset">MesIncrementalHandleReset</a> function must be called with its <i>OpCode</i> parameter set to MES_ENCODE_NDR64.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/Rpc/incremental-serialization">Alloc</a>



<a href="https://docs.microsoft.com/windows/desktop/api/midles/nf-midles-mesbufferhandlereset">MesBufferHandleReset</a>



<a href="https://docs.microsoft.com/windows/desktop/api/midles/nf-midles-meshandlefree">MesHandleFree</a>



<a href="https://docs.microsoft.com/windows/desktop/api/midles/nf-midles-mesincrementalhandlereset">MesIncrementalHandleReset</a>
 

 

