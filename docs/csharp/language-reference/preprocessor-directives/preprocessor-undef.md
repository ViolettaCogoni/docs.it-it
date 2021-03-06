---
title: "#undef (Riferimenti per C#) | Microsoft Docs"
ms.date: "2015-07-20"
ms.prod: ".net"
ms.technology: 
  - "devlang-csharp"
ms.topic: "article"
f1_keywords: 
  - "#undef"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "#undef (direttiva) [C#]"
ms.assetid: 686c92d2-7194-4be4-b2f4-80091712d513
caps.latest.revision: 12
author: "BillWagner"
ms.author: "wiwagn"
caps.handback.revision: 12
---
# #undef (Riferimenti per C#)
`#undef` consente di rimuovere la definizione di un simbolo. In questo modo, se si utilizza il simbolo come espressione in una direttiva [\#if](../../../csharp/language-reference/preprocessor-directives/preprocessor-if.md), l'espressione restituirà `false`.  
  
 Un simbolo può essere definito con la direttiva [\#define](../../../csharp/language-reference/preprocessor-directives/preprocessor-define.md) o con l'opzione di compilazione [\/define](../../../csharp/language-reference/compiler-options/define-compiler-option.md).  La direttiva `#undef` deve essere inserita in un file prima di utilizzare istruzioni che non siano anche direttive.  
  
## Esempio  
  
```  
// preprocessor_undef.cs  
// compile with: /d:DEBUG  
#undef DEBUG  
using System;  
class MyClass   
{  
    static void Main()   
    {  
#if DEBUG  
        Console.WriteLine("DEBUG is defined");  
#else  
        Console.WriteLine("DEBUG is not defined");  
#endif  
    }  
}  
```  
  
  **DEBUG non è stato definito.**   
## Vedere anche  
 [Riferimenti per C\#](../../../csharp/language-reference/index.md)   
 [Guida per programmatori C\#](../../../csharp/programming-guide/index.md)   
 [Direttive per il preprocessore C\#](../../../csharp/language-reference/preprocessor-directives/index.md)