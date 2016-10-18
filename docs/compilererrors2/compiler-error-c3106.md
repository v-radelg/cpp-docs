---
title: "Compiler Error C3106"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "error-reference"
f1_keywords: 
  - "C3106"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "C3106"
ms.assetid: 39d97a32-0905-4702-87d3-7f8ce473fb93
caps.latest.revision: 6
ms.author: "corob"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# Compiler Error C3106
'attribute': unnamed arguments must precede named arguments  
  
 Unnamed arguments must be passed to an attribute before named arguments.  
  
 For more information, see [User-Defined Attributes](../windows/user-defined-attributes---c---component-extensions-.md).  
  
## Example  
 The following sample generates C3106.  
  
```  
// C3106.cpp  
// compile with: /c  
[module(name="MyLib", dll)];   // C3106  
[module(dll, name="MyLib")];   // OK  
```