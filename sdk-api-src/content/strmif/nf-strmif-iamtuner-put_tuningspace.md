---
UID: NF:strmif.IAMTuner.put_TuningSpace
title: IAMTuner::put_TuningSpace (strmif.h)
description: The put_TuningSpace method sets a storage index for regional channel-to-frequency mappings.
helpviewer_keywords: ["IAMTuner interface [DirectShow]","put_TuningSpace method","IAMTuner.put_TuningSpace","IAMTuner::put_TuningSpace","IAMTunerput_TuningSpace","dshow.iamtuner_put_tuningspace","put_TuningSpace","put_TuningSpace method [DirectShow]","put_TuningSpace method [DirectShow]","IAMTuner interface","strmif/IAMTuner::put_TuningSpace"]
old-location: dshow\iamtuner_put_tuningspace.htm
tech.root: dshow
ms.assetid: fd0c0bc5-2c46-4c5a-8f93-9021f37a6e6a
ms.date: 12/05/2018
ms.keywords: IAMTuner interface [DirectShow],put_TuningSpace method, IAMTuner.put_TuningSpace, IAMTuner::put_TuningSpace, IAMTunerput_TuningSpace, dshow.iamtuner_put_tuningspace, put_TuningSpace, put_TuningSpace method [DirectShow], put_TuningSpace method [DirectShow],IAMTuner interface, strmif/IAMTuner::put_TuningSpace
f1_keywords:
- strmif/IAMTuner.put_TuningSpace
dev_langs:
- c++
req.header: strmif.h
req.include-header: Dshow.h
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
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Strmiids.lib
- Strmiids.dll
api_name:
- IAMTuner.put_TuningSpace
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAMTuner::put_TuningSpace


## -description



The <code>put_TuningSpace</code> method sets a storage index for regional channel-to-frequency mappings.




## -parameters




### -param lTuningSpace [in]

Value indicating the current locale.


## -returns



Returns an <b>HRESULT</b> value that depends on the implementation of the interface.




## -remarks



As TV tuners move into portable systems, you must retain locale-specific mappings of available channels and their actual frequencies. Formulating different <i>lTuningSpace</i> values for each locale provides a way of switching the channel-to-frequency mappings when moving from region to region.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/strmif/nn-strmif-iamtuner">IAMTuner Interface</a>
 

 

