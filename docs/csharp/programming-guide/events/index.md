---
title: Eventi (Guida per programmatori C#) | Microsoft Docs
ms.date: 2015-07-20
ms.prod: .net
ms.technology:
- devlang-csharp
ms.topic: article
dev_langs:
- CSharp
helpviewer_keywords:
- classes [C#], events
- C# language, events
- events [C#]
ms.assetid: a8e51b22-d294-44fb-9539-0072f06c4cb3
caps.latest.revision: 43
author: BillWagner
ms.author: wiwagn
translation.priority.ht:
- de-de
- es-es
- fr-fr
- it-it
- ja-jp
- ko-kr
- ru-ru
- zh-cn
- zh-tw
translation.priority.mt:
- cs-cz
- pl-pl
- pt-br
- tr-tr
ms.translationtype: Human Translation
ms.sourcegitcommit: 31905a37f09db5f5192123f0118252fbe8b02eff
ms.openlocfilehash: b3f4673eccdbd568fa8ab042023a4b3bd8230bb3
ms.contentlocale: it-it
ms.lasthandoff: 05/26/2017

---
<a id="events-c-programming-guide" class="xliff"></a>

# Eventi (Guida per programmatori C#)
Tramite gli eventi, una [classe](../../../csharp/language-reference/keywords/class.md) o un oggetto è in grado di segnalare ad altre classi o oggetti una situazione di interesse. La classe che invia (o *genera*) l'evento è chiamata *autore* e le classi che ricevono (o *gestiscono*) l'evento sono chiamate *sottoscrittori*.  
  
 In un'applicazione C# Web o Windows Form tipica si sottoscrivono eventi generati da controlli quali pulsanti e caselle di riepilogo. È possibile usare l'ambiente di sviluppo integrato (IDE) di [!INCLUDE[csprcs](~/includes/csprcs-md.md)] per cercare gli eventi pubblicati da un controllo e selezionare quelli che si vuole gestire. L'IDE aggiunge automaticamente un metodo vuoto del gestore eventi e il codice per sottoscrivere l'evento. Per altre informazioni, vedere [Procedura: sottoscrivere e annullare la sottoscrizione di eventi](../../../csharp/programming-guide/events/how-to-subscribe-to-and-unsubscribe-from-events.md).  
  
<a id="events-overview" class="xliff"></a>

## Cenni preliminari sugli eventi  
 Di seguito sono riportate le proprietà degli eventi:  
  
-   L'autore determina quando viene generato un evento. I sottoscrittori determinano quale azione viene eseguita in risposta all'evento.  
  
-   Un evento può avere più sottoscrittori. Un sottoscrittore può gestire più eventi da più autori.  
  
-   Gli eventi che non hanno sottoscrittore non vengono mai generati.  
  
-   Gli eventi vengono in genere usati per segnalare azioni dell'utente, ad esempio la scelta di un pulsante o di una voce di menu nell'interfaccia utente grafica.  
  
-   Quando un evento ha più sottoscrittori, i gestori eventi vengono richiamati in modo sincrono al momento della generazione dell'evento. Per richiamare gli eventi in modo asincrono, vedere [Calling Synchronous Methods Asynchronously](https://msdn.microsoft.com/library/2e08f6yc).  
  
-   Nella libreria di classi di [!INCLUDE[dnprdnshort](~/includes/dnprdnshort-md.md)] gli eventi sono basati sul delegato <xref:System.EventHandler> e sulla classe di base <xref:System.EventArgs>.  
  
<a id="related-sections" class="xliff"></a>

## Sezioni correlate  
 Per altre informazioni, vedere:  
  
-   [Procedura: Eseguire e annullare la sottoscrizione a eventi](../../../csharp/programming-guide/events/how-to-subscribe-to-and-unsubscribe-from-events.md)  
  
-   [Procedura: Pubblicare eventi conformi alle linee guida di .NET Framework](../../../csharp/programming-guide/events/how-to-publish-events-that-conform-to-net-framework-guidelines.md)  
  
-   [Procedura: Generare eventi di classe base nelle classi derivate](../../../csharp/programming-guide/events/how-to-raise-base-class-events-in-derived-classes.md)  
  
-   [Procedura: Implementare eventi di interfaccia](../../../csharp/programming-guide/events/how-to-implement-interface-events.md)  
  
-   [Sincronizzazione di thread](../../../csharp/programming-guide/concepts/threading/thread-synchronization.md)  
  
-   [Procedura: Usare un dizionario per archiviare istanze di evento](../../../csharp/programming-guide/events/how-to-use-a-dictionary-to-store-event-instances.md)  
  
-   [Procedura: Implementare funzioni di accesso a eventi personalizzati](../../../csharp/programming-guide/events/how-to-implement-custom-event-accessors.md)  
  
<a id="c-language-specification" class="xliff"></a>

## Specifiche del linguaggio C#  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
<a id="featured-book-chapters" class="xliff"></a>

## Capitoli del libro rappresentati  
 [Delegates, Events, and Lambda Expressions](http://go.microsoft.com/fwlink/?LinkId=195395) (Delegati, eventi ed espressioni lambda) in [C# 3.0 Cookbook, Third Edition: More than 250 solutions for C# 3.0 programmers](http://go.microsoft.com/fwlink/?LinkId=195369)  
  
 [Delegates and Events](http://go.microsoft.com/fwlink/?LinkId=195418) in [Learning C# 3.0: Master the fundamentals of C# 3.0](http://go.microsoft.com/fwlink/?LinkId=195412)  
  
<a id="see-also" class="xliff"></a>

## Vedere anche  
 <xref:System.EventHandler>   
 [Guida per programmatori C#](../../../csharp/programming-guide/index.md)   
 [Delegati](../../../csharp/programming-guide/delegates/index.md)   
 [Creazione di gestori eventi in Windows Forms](https://msdn.microsoft.com/library/dacysss4.aspx)   
 [Programmazione multithreading con il modello asincrono basato su eventi](https://msdn.microsoft.com/library/hkasytyf)
