---
redirect_url: /dotnet/articles/csharp/linq/handle-null-values-in-query-expressions
caps.handback.revision: 6
---
# Procedura: gestire valori null nelle espressioni di query (Guida per programmatori C#)
In questo esempio viene illustrato come gestire i possibili valori null nelle raccolte di origine.  Una raccolta di oggetti quale <xref:System.Collections.Generic.IEnumerable%601> può contenere elementi il cui valore è [null](../../../csharp/language-reference/keywords/null.md).  Se una raccolta di origine è null o contiene un elemento il cui valore è null e la query non gestisce valori null, verrà generata un'eccezione <xref:System.NullReferenceException> quando si esegue la query.  
  
## Esempio  
 È possibile codificare in modo sicuro per evitare un'eccezione di riferimento null come illustrato nell'esempio seguente:  
  
 [!code-cs[csProgGuideLINQ#82](../../../csharp/programming-guide/arrays/codesnippet/csharp/csLINQProgRef/csRef30LangFeatures_2.cs#82)]  
  
 Nell'esempio precedente la clausola `where` esclude tutti gli elementi null nella sequenza di categorie.  Questa tecnica è indipendente dal controllo null nella clausola join.  In questo esempio è possibile utilizzare l'espressione condizionale con null poiché `Products.CategoryID` è di tipo `int?`, ovvero una forma abbreviata di `Nullable<int>`.  
  
## Esempio  
 Se in una clausola join solo una delle chiavi di confronto è un tipo valore che ammette valori null, è possibile eseguire il cast della altre chiavi a un tipo che ammette valori null nell'espressione di query.  Nell'esempio seguente si supponga che `EmployeeID` sia una colonna contenente valori di tipo `int?`:  
  
 [!code-cs[csProgGuideLINQ#83](../../../csharp/programming-guide/arrays/codesnippet/csharp/csLINQProgRef/csRef30LangFeatures_2.cs#83)]  
  
## Vedere anche  
 <xref:System.Nullable%601>   
 [Espressioni di query LINQ](../../../csharp/programming-guide/linq-query-expressions/index.md)   
 [Tipi nullable](../../../csharp/programming-guide/nullable-types/index.md)