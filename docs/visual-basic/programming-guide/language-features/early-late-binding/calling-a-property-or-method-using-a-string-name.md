---
title: "Calling a Property or Method Using a String Name (Visual Basic) | Microsoft Docs"
ms.custom: ""
ms.date: "2015-07-20"
ms.prod: ".net"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.topic: "article"
dev_langs: 
  - "VB"
helpviewer_keywords: 
  - "passing operators"
  - "strings [Visual Basic], passing new operators as"
  - "objects [Visual Basic], setting properties"
  - "setting properties, object properties at run time"
  - "method calls, strings"
  - "methods [Visual Basic], calling with string names"
  - "calling methods, string names"
  - "properties [Visual Basic], setting at run time"
  - "CallByName function"
ms.assetid: 79a7b8b4-b8c7-4ad8-aca8-12a9a2b32f03
caps.latest.revision: 17
author: "stevehoag"
ms.author: "shoag"
caps.handback.revision: 17
---
# Calling a Property or Method Using a String Name (Visual Basic)
[!INCLUDE[vs2017banner](../../../../visual-basic/developing-apps/includes/vs2017banner.md)]

Nella maggior parte dei casi è possibile determinare le proprietà e i metodi di un oggetto in fase di progettazione e scrivere codice che ne consenta la gestione.  In alcuni casi, tuttavia, non è possibile conoscere in anticipo le proprietà e i metodi di un oggetto oppure si preferisce semplicemente una maggiore flessibilità che consenta agli utenti finali di specificare le proprietà o eseguire i metodi in fase di esecuzione.  
  
## Funzione CallByName  
 Si consideri, ad esempio, un'applicazione client che valuta espressioni immesse dall'utente finale passando un operatore a un componente COM.  Si supponga di dover aggiungere continuamente al componente nuove funzioni che richiedono nuovi operatori.  Quando si utilizzano le tecniche standard di accesso agli oggetti, è necessario ricompilare e ridistribuire l'applicazione client affinché essa possa utilizzare i nuovi operatori.  Per evitare l'esecuzione di tali operazioni, è possibile utilizzare la funzione `CallByName` per passare i nuovi operatori come stringhe, senza apportare modifiche all'applicazione.  
  
 La funzione `CallByName` consente di utilizzare una stringa per specificare una proprietà o un metodo in fase di esecuzione.  La firma per la funzione `CallByName` ha il seguente aspetto:  
  
 *Result* \= `CallByName`\(*Object*, *ProcedureName*, *CallType*, *Arguments*\(\)\)  
  
 Il primo argomento *Object* prende il nome dell'oggetto sul quale si desidera agire.  L'argomento *ProcedureName* prende una stringa contenente il nome del metodo o della routine della proprietà da richiamare.  L'argomento *CallType* prende una costante che rappresenta il tipo di routine da richiamare, ovvero un metodo \(`Microsoft.VisualBasic.CallType.Method`\), una proprietà letta \(`Microsoft.VisualBasic.CallType.Get`\) o una proprietà impostata \(`Microsoft.VisualBasic.CallType.Set`\).  L'argomento facoltativo *Arguments* prende una matrice di tipo `Object` contenente qualsiasi argomento per la routine.  
  
 È possibile utilizzare `CallByName` con classi della soluzione corrente, ma nella maggior parte dei casi se ne fa uso per accedere a oggetti COM o a oggetti degli assembly [!INCLUDE[dnprdnshort](../../../../csharp/getting-started/includes/dnprdnshort-md.md)].  
  
 Si supponga di aggiungere un riferimento a un assembly contenente una classe denominata `MathClass`, in cui è presente una nuova funzione denominata `SquareRoot`, come illustrato nel codice seguente:  
  
 [!code-vb[VbVbalrOOP#53](../../../../visual-basic/misc/codesnippet/visualbasic/VbVbalrOOP/OOP.vb#53)]  
  
 È possibile che l'applicazione utilizzi i controlli della casella di testo per controllare il metodo chiamato e i relativi argomenti.  Se, ad esempio, `TextBox1` contiene l'espressione da valutare e `TextBox2` viene utilizzato per immettere il nome della funzione, è possibile utilizzare il codice seguente per richiamare la funzione `SquareRoot` per l'espressione in `TextBox1`:  
  
 [!code-vb[VbVbalrOOP#54](../../../../visual-basic/misc/codesnippet/visualbasic/VbVbalrOOP/OOP.vb#54)]  
  
 Se si immette "64" in `TextBox1` "SquareRoot" in `TextBox2`, quindi si chiama la routine `CallMath`, verrà valutata la radice quadrata del numero specificato in `TextBox1`.  Il codice riportato nell'esempio richiama la funzione `SquareRoot` \(che accetta una stringa contenente l'espressione da valutare come argomento obbligatorio\) e restituisce "8" in `TextBox1` \(la radice quadrata di 64\).  Naturalmente, se l'utente immette una stringa non valida in `TextBox2`, se la stringa contiene il nome di una proprietà anziché di un metodo o se il metodo richiede un ulteriore argomento, verrà generato un errore di runtime.  Quando si utilizza `CallByName` è necessario aggiungere un efficace codice di gestione degli errori per prevenire errori di questo o altro tipo.  
  
> [!NOTE]
>  Sebbene la funzione `CallByName` possa risultare utile in alcuni casi, è necessario valutarne attentamente, a fronte dell'utilità, anche le implicazioni in termini di prestazioni, in quanto il ricorso a `CallByName` per richiamare una routine risulta leggermente più lento rispetto a una chiamata ad associazione tardiva.  Se si invoca una funzione che viene poi chiamata ripetutamente, ad esempio all'interno di un ciclo, `CallByName` può compromettere seriamente le prestazioni.  
  
## Vedere anche  
 <xref:Microsoft.VisualBasic.Interaction.CallByName%2A>   
 [Determining Object Type](../../../../visual-basic/programming-guide/language-features/early-late-binding/determining-object-type.md)