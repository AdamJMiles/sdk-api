---
UID: NF:wbemcli.IWbemServices.ExecMethod
title: IWbemServices::ExecMethod (wbemcli.h)
description: Executes a method exported by a CIM object.
old-location: wmi\iwbemservices_execmethod.htm
tech.root: WmiSdk
ms.assetid: 9acba1aa-bcca-416a-863c-704d2e72df07
ms.date: 12/05/2018
ms.keywords: ExecMethod, ExecMethod method [Windows Management Instrumentation], ExecMethod method [Windows Management Instrumentation],IWbemServices interface, IWbemServices interface [Windows Management Instrumentation],ExecMethod method, IWbemServices.ExecMethod, IWbemServices::ExecMethod, _hmm_iwbemservices_execmethod, wbemcli/IWbemServices::ExecMethod, wmi.iwbemservices_execmethod
f1_keywords:
- wbemcli/IWbemServices.ExecMethod
dev_langs:
- c++
req.header: wbemcli.h
req.include-header: Wbemidl.h
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wbemuuid.lib
req.dll: Fastprox.dll; Esscli.dll; FrameDyn.dll; FrameDynOS.dll; Ntevt.dll; Stdprov.dll; Viewprov.dll; Wbemcomn.dll; Wbemcore.dll; Wbemess.dll; Wbemsvc.dll; Wmipicmp.dll; Wmidcprv.dll; Wmipjobj.dll; Wmiprvsd.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Fastprox.dll
- Esscli.dll
- FrameDyn.dll
- FrameDynOS.dll
- Ntevt.dll
- Stdprov.dll
- Viewprov.dll
- Wbemcomn.dll
- Wbemcore.dll
- Wbemess.dll
- Wbemsvc.dll
- Wmipicmp.dll
- Wmidcprv.dll
- Wmipjobj.dll
- Wmiprvsd.dll
api_name:
- IWbemServices.ExecMethod
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWbemServices::ExecMethod


## -description


The 
<b>IWbemServices::ExecMethod</b> method executes a method exported by a CIM object. The method call is forwarded to the appropriate provider where it executes. Information and status are returned to the caller, which blocks until the call is complete.

Methods are not directly implemented by Windows Management, but are exported by method providers. For any given CIM class, the available methods and their parameters must be specified in the documentation for the provider in question.

For more information about executing methods, see 
<a href="https://docs.microsoft.com/windows/desktop/WmiSdk/calling-a-method">Calling a Method</a>.


## -parameters




### -param strObjectPath [in]

Valid <b>BSTR</b> containing the 
<a href="https://docs.microsoft.com/windows/desktop/WmiSdk/describing-a-class-object-path">object path</a> of the object for which the method is executed.


### -param strMethodName [in]

Name of the method for the object.


### -param lFlags [in]

This parameter can be set to 0 to make this a synchronous call. To make this a semisynchronous call, set <i>lFlags</i> to <b>WBEM_FLAG_RETURN_IMMEDIATELY</b>, provide a valid pointer for the <i>ppCallResult</i> parameter, and this call returns immediately. For more information, see 
<a href="https://docs.microsoft.com/windows/desktop/WmiSdk/calling-a-method">Calling a Method</a>.


### -param pCtx [in]

Typically <b>NULL</b>;  otherwise, this is a pointer to an 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nn-wbemcli-iwbemcontext">IWbemContext</a> object that may be used by the provider executing the method. The values in the context object must be specified in the documentation for the provider in question. For more information about this parameter, see 
<a href="https://docs.microsoft.com/windows/desktop/WmiSdk/making-calls-to-wmi">Making Calls to WMI</a>.


### -param pInParams [in]

May be <b>NULL</b> if no in-parameters are required to execute the method. Otherwise, this points to an 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nn-wbemcli-iwbemclassobject">IWbemClassObject</a> that contains the properties acting as inbound parameters for the method execution. The contents of the object are method-specific, and are part of the specification for the provider in question. For more information about constructing input parameters, see <a href="https://docs.microsoft.com/windows/desktop/WmiSdk/creating-parameters-objects-in-c--">Creating Parameters Objects in C++</a>.


### -param ppOutParams [out]

If not <b>NULL</b>, receives a pointer to the outbound parameters and return values for the method execution. The contents of this object are method-specific, and are part of the specification for the provider in question. The caller must call <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nf-unknwn-iunknown-release">Release</a> on the returned object when it is no longer required.


### -param ppCallResult [out]

If <b>NULL</b>, this is not used. If <i>ppCallResult</i> is specified, it must be set to point to <b>NULL</b> on entry. In this case, the call returns immediately with <b>WBEM_S_NO_ERROR</b>. The <i>ppCallResult</i> parameter receives a pointer to a new 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nn-wbemcli-iwbemcallresult">IWbemCallResult</a> object, which must be polled to obtain the result of the method execution using the 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcallresult-getcallstatus">GetCallStatus</a> method. The out parameters for the call are available by calling 
<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcallresult-getresultobject">IWbemCallResult::GetResultObject</a>.


## -returns



This method returns an <b>HRESULT</b> indicating the status of the method call. The following list lists the value contained within an <b>HRESULT</b>.

On failure, you can obtain any available information from the COM function <a href="https://docs.microsoft.com/windows/desktop/api/oleauto/nf-oleauto-geterrorinfo">GetErrorInfo</a>.

COM-specific error codes also may be returned if network problems cause you to lose the remote connection to Windows Management.




## -remarks



If <i>ppOutParams</i> is not <b>NULL</b>, the client can determine the method's return value type by examining the <b>ReturnValue</b> property of the object pointed to by <i>ppOutParams</i>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/WmiSdk/calling-a-method">Calling a Method</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemcallresult-getresultobject">IWbemCallResult::GetResultObject</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nn-wbemcli-iwbemservices">IWbemServices</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wbemcli/nf-wbemcli-iwbemservices-execmethodasync">IWbemServices::ExecMethodAsync</a>
 

 

