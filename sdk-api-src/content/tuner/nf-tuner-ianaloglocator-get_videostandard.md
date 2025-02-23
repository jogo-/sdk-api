---
UID: NF:tuner.IAnalogLocator.get_VideoStandard
title: IAnalogLocator::get_VideoStandard (tuner.h)
description: The get_VideoStandard method retrieves the format of the analog television signal.
helpviewer_keywords: ["IAnalogLocator interface [Microsoft TV Technologies]","get_VideoStandard method","IAnalogLocator.get_VideoStandard","IAnalogLocator::get_VideoStandard","IAnalogLocatorget_VideoStandard","get_VideoStandard","get_VideoStandard method [Microsoft TV Technologies]","get_VideoStandard method [Microsoft TV Technologies]","IAnalogLocator interface","mstv.ianaloglocator_get_videostandard","tuner/IAnalogLocator::get_VideoStandard"]
old-location: mstv\ianaloglocator_get_videostandard.htm
tech.root: mstv
ms.assetid: 8530f436-8067-43bd-8f64-45e042ccb466
ms.date: 12/05/2018
ms.keywords: IAnalogLocator interface [Microsoft TV Technologies],get_VideoStandard method, IAnalogLocator.get_VideoStandard, IAnalogLocator::get_VideoStandard, IAnalogLocatorget_VideoStandard, get_VideoStandard, get_VideoStandard method [Microsoft TV Technologies], get_VideoStandard method [Microsoft TV Technologies],IAnalogLocator interface, mstv.ianaloglocator_get_videostandard, tuner/IAnalogLocator::get_VideoStandard
f1_keywords:
- tuner/IAnalogLocator.get_VideoStandard
dev_langs:
- c++
req.header: tuner.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
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
- IAnalogLocator.get_VideoStandard
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAnalogLocator::get_VideoStandard


## -description



The <b>get_VideoStandard</b> method retrieves the format of the analog television signal.




## -parameters




### -param AVS [out]

Pointer to an <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/strmif/ne-strmif-analogvideostandard">AnalogVideoStandard</a> variable that receives the format of the analog television signal.


## -returns



Returns S_OK if successful. If the method fails, error information can be retrieved by using the standard COM <b>IErrorInfo</b> interface.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tuner/nn-tuner-ianaloglocator">IAnalogLocator Interface</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tuner/nf-tuner-ianaloglocator-put_videostandard">put_VideoStandard</a>
 

 

