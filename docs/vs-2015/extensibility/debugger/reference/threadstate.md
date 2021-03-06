---
title: "THREADSTATE | Microsoft Docs"
ms.date: 11/15/2016
ms.prod: "visual-studio-dev14"
ms.technology: "vs-ide-sdk"
ms.topic: reference
f1_keywords: 
  - "THREADSTATE"
helpviewer_keywords: 
  - "THREADSTATE enumeration"
ms.assetid: 62efdd7c-25b1-4fd3-9d06-ac1830a418a9
caps.latest.revision: 10
ms.author: gregvanl
manager: jillfra
---
# THREADSTATE
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

Specifies the state of the thread.  
  
## Syntax  
  
```cpp#  
enum enum_THREADSTATE {   
   THREADSTATE_RUNNING = 0x0001,  
   THREADSTATE_STOPPED = 0x0002,  
   THREADSTATE_FRESH   = 0x0003,  
   THREADSTATE_DEAD    = 0x0004,  
   THREADSTATE_FROZEN  = 0x0005  
};  
typedef DWORD THREADSTATE;  
```  
  
```csharp  
public enum enum_THREADSTATE {   
   THREADSTATE_RUNNING = 0x0001,  
   THREADSTATE_STOPPED = 0x0002,  
   THREADSTATE_FRESH   = 0x0003,  
   THREADSTATE_DEAD    = 0x0004,  
   THREADSTATE_FROZEN  = 0x0005  
};  
```  
  
## Members  
 THREADSTATE_RUNNING  
 Indicates that the thread is running.  
  
 THREADSTATE_STOPPED  
 Indicates that the thread is stopped because of a breakpoint.  
  
 THREADSTATE_FRESH  
 Indicates that the thread has been created, but is not yet running code.  
  
 THREADSTATE_DEAD  
 Indicates that the thread is dead.  
  
 THREADSTATE_FROZEN  
 Indicates that the thread is frozen (no execution can be performed).  
  
## Remarks  
 Used for the `dwThreadState` field of the [THREADPROPERTIES](../../../extensibility/debugger/reference/threadproperties.md) structure.  
  
## Requirements  
 Header: msdbg.h  
  
 Namespace: Microsoft.VisualStudio.Debugger.Interop  
  
 Assembly: Microsoft.VisualStudio.Debugger.Interop.dll  
  
## See Also  
 [Enumerations](../../../extensibility/debugger/reference/enumerations-visual-studio-debugging.md)   
 [THREADPROPERTIES](../../../extensibility/debugger/reference/threadproperties.md)
