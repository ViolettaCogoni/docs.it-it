---
title: "&#39;Optional&#39; expected | Microsoft Docs"
ms.date: "2015-07-20"
ms.prod: ".net"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.topic: "article"
f1_keywords: 
  - "bc30202"
  - "vbc30202"
dev_langs: 
  - "VB"
helpviewer_keywords: 
  - "BC30202"
ms.assetid: 6f75060c-2db4-4a79-b5d1-5780c09a74cd
caps.latest.revision: 9
author: "stevehoag"
ms.author: "shoag"
caps.handback.revision: 9
---
# &#39;Optional&#39; expected
[!INCLUDE[vs2017banner](../../../visual-basic/developing-apps/includes/vs2017banner.md)]

In una dichiarazione di routine un argomento facoltativo è seguito da un argomento obbligatorio.  Qualsiasi argomento posto dopo un argomento facoltativo deve essere facoltativo.  
  
 **ID errore:** BC30202  
  
### Per correggere l'errore  
  
1.  Se l'argomento è obbligatorio, spostarlo prima del primo argomento facoltativo dell'elenco degli argomenti.  
  
2.  Se l'argomento è facoltativo, utilizzare la parola chiave `Optional`.  
  
## Vedere anche  
 [Optional Parameters](../../../visual-basic/programming-guide/language-features/procedures/optional-parameters.md)