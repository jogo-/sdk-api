---
UID: NF:fwpmu.IkeextSaDbSetSecurityInfo0
title: IkeextSaDbSetSecurityInfo0 function (fwpmu.h)
description: The IkeextSaDbSetSecurityInfo0 function sets specified security information in the security descriptor of the IKE/AuthIP security association database.
helpviewer_keywords: ["IkeextSaDbSetSecurityInfo0","IkeextSaDbSetSecurityInfo0 function [Filtering]","fwp.ikeextsadbsetsecurityinfo0","fwpmu/IkeextSaDbSetSecurityInfo0"]
old-location: fwp\ikeextsadbsetsecurityinfo0.htm
tech.root: fwp
ms.assetid: a1707cc4-7b61-4626-b98b-e9fb853d1ccf
ms.date: 12/05/2018
ms.keywords: IkeextSaDbSetSecurityInfo0, IkeextSaDbSetSecurityInfo0 function [Filtering], fwp.ikeextsadbsetsecurityinfo0, fwpmu/IkeextSaDbSetSecurityInfo0
f1_keywords:
- fwpmu/IkeextSaDbSetSecurityInfo0
dev_langs:
- c++
req.header: fwpmu.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Fwpuclnt.lib
req.dll: Fwpuclnt.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Fwpuclnt.dll
api_name:
- IkeextSaDbSetSecurityInfo0
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IkeextSaDbSetSecurityInfo0 function


## -description


The <b>IkeextSaDbSetSecurityInfo0</b> function sets specified security information in the security descriptor of the IKE/AuthIP security association database.


## -parameters




### -param engineHandle [in]

Type: <b>HANDLE</b>

Handle for an open session to the filter engine generated by a previous  call to  <a href="https://docs.microsoft.com/windows/desktop/api/fwpmu/nf-fwpmu-fwpmengineopen0">FwpmEngineOpen0</a>.


### -param securityInfo [in]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/SecAuthZ/security-information">SECURITY_INFORMATION</a></b>

The type of security information to set.


### -param sidOwner [in, optional]

Type: <b>const <a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-sid">SID</a>*</b>

The owner's security identifier (SID) to be set in the security descriptor.


### -param sidGroup [in, optional]

Type: <b>const <a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-sid">SID</a>*</b>

The group's SID to be set in the security descriptor.


### -param dacl [in, optional]

Type: <b>const <a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-acl">ACL</a>*</b>

The discretionary access control list (DACL) to be set in the security descriptor.


### -param sacl [in, optional]

Type: <b>const <a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-acl">ACL</a>*</b>

The system access control list (SACL) to be set in the security descriptor.


## -returns



Type: <b>DWORD</b>

<table>
<tr>
<th>Return code/value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>ERROR_SUCCESS</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The security information was set successfully.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>FWP_E_* error code</b></dt>
<dt>0x80320001—0x80320039</dt>
</dl>
</td>
<td width="60%">
A Windows Filtering Platform (WFP) specific error. See <a href="https://docs.microsoft.com/windows/desktop/FWP/wfp-error-codes">WFP Error Codes</a> for details.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>RPC_* error code</b></dt>
<dt>0x80010001—0x80010122</dt>
</dl>
</td>
<td width="60%">
Failure to communicate with the remote or local firewall engine.

</td>
</tr>
</table>
 




## -remarks



This function behaves like the standard Win32 	 <a href="https://docs.microsoft.com/windows/desktop/api/aclapi/nf-aclapi-setsecurityinfo">SetSecurityInfo</a> function. The caller needs the same standard access rights as described in the <b>SetSecurityInfo</b> reference topic.

<b>IkeextSaDbSetSecurityInfo0</b> is a specific implementation of IkeextSaDbSetSecurityInfo. See <a href="https://docs.microsoft.com/windows/desktop/FWP/wfp-version-independent-names-and-targeting-specific-versions-of-windows">WFP Version-Independent Names and Targeting Specific Versions of Windows</a>  for more information.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/fwpmu/nf-fwpmu-ikeextsadbgetsecurityinfo0">IkeextSaDbGetSecurityInfo0</a>
 

 

