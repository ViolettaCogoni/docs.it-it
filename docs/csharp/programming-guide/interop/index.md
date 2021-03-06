---
title: "Interoperabilità (Guida per programmatori C#) | Microsoft Docs"
ms.date: 2015-07-20
ms.prod: .net
ms.technology:
- devlang-csharp
ms.topic: article
dev_langs:
- CSharp
helpviewer_keywords:
- COM interop
- interoperability
- platform invoke, accessing APIs with C#
- C# language, interoperability
ms.assetid: 238bb95a-e962-4026-bbd5-197055bdb8ee
caps.latest.revision: 31
author: BillWagner
ms.author: wiwagn
translation.priority.ht:
- cs-cz
- de-de
- es-es
- fr-fr
- it-it
- ja-jp
- ko-kr
- pl-pl
- pt-br
- ru-ru
- tr-tr
- zh-cn
- zh-tw
ms.translationtype: Human Translation
ms.sourcegitcommit: 31905a37f09db5f5192123f0118252fbe8b02eff
ms.openlocfilehash: be95d675d22dedcbf45c8eb1e8fd8d9f5ce0b56c
ms.contentlocale: it-it
ms.lasthandoff: 05/26/2017

---
<a id="interoperability-c-programming-guide" class="xliff"></a>

# Interoperabilità (Guida per programmatori C#)
L'interoperabilità consente di preservare e sfruttare appieno gli investimenti effettuati in codice non gestito. Il codice eseguito sotto il controllo del Common Language Runtime (CLR) è detto *codice gestito*, mentre quello eseguito all'esterno è detto *codice non gestito*. Esempi di codice non gestito sono i componenti COM, COM+, C++, i componenti ActiveX e le API Microsoft Win32.  
  
 [!INCLUDE[dnprdnshort](~/includes/dnprdnshort-md.md)] consente l'interoperabilità con il codice non gestito tramite i servizi platform invoke, lo spazio dei nomi <xref:System.Runtime.InteropServices>, l'interoperabilità C++ e l'interoperabilità COM.  
  
<a id="in-this-section" class="xliff"></a>

## Contenuto della sezione  
 [Cenni preliminari sull'interoperabilità](../../../csharp/programming-guide/interop/interoperability-overview.md)  
 Vengono descritti i metodi per l'interoperabilità tra codice C# gestito e non gestito.  
  
 [Procedura: Accedere agli oggetti di interoperabilità di Office usando le funzionalità di Visual C#](../../../csharp/programming-guide/interop/how-to-access-office-onterop-objects.md)  
 Vengono descritte le funzionalità introdotte in Visual C# per facilitare la programmazione di Office.  
  
 [Procedura: Usare proprietà indicizzate nella programmazione dell'interoperabilità COM](../../../csharp/programming-guide/interop/how-to-use-indexed-properties-in-com-interop-rogramming.md)  
 Viene illustrato come usare le proprietà indicizzate per accedere alle proprietà COM con parametri.  
  
 [Procedura: Usare platform invoke per riprodurre un file audio](../../../csharp/programming-guide/interop/how-to-use-platform-invoke-to-play-a-wave-file.md)  
 Viene descritto come usare i servizi platform invoke per riprodurre un file audio con estensione wav nel sistema operativo Windows.  
  
 [Procedura dettagliata: Programmazione di Office](../../../csharp/programming-guide/interop/walkthrough-office-programming.md)  
 Viene illustrato come creare una cartella di lavoro di Excel o un documento di Word contenente un collegamento alla cartella di lavoro.  
  
 [Esempio di classe COM](../../../csharp/programming-guide/interop/example-com-class.md)  
 Viene illustrato come esporre una classe C# come oggetto COM.  
  
<a id="c-language-specification" class="xliff"></a>

## Specifiche del linguaggio C#  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
<a id="see-also" class="xliff"></a>

## Vedere anche  
 <xref:System.Runtime.InteropServices.Marshal.ReleaseComObject%2A?displayProperty=fullName>   
 [Guida per programmatori C#](../../../csharp/programming-guide/index.md)   
 [Interoperabilità con codice non gestito](https://msdn.microsoft.com/library/sd10k43k)   
 [Procedura dettagliata: Programmazione di Office](../../../csharp/programming-guide/interop/walkthrough-office-programming.md)
