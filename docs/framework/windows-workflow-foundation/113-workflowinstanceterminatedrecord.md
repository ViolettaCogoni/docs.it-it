---
title: "113 - WorkflowInstanceTerminatedRecord | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: f53204ee-4ea2-45e1-8859-e86d07305efd
caps.latest.revision: 6
author: "Erikre"
ms.author: "erikre"
manager: "erikre"
caps.handback.revision: 6
---
# 113 - WorkflowInstanceTerminatedRecord
## Proprietà  
  
|||  
|-|-|  
|ID|113|  
|Parole chiave|EndToEndMonitoring, Risoluzione dei problemi, HealthMonitoring, WFTracking|  
|Livello|Errore|  
|Canale|Microsoft\-Windows\-Server applicazioni\-Applicazioni\/Analitico|  
  
## Descrizione  
 Questo evento viene creato dal partecipante del rilevamento ETW quando un'istanza del flusso di lavoro crea WorkflowInstanceTerminatedRecord.  
  
## Messaggio  
 TrackRecord \= WorkflowInstanceTerminatedRecord, InstanceID \= %1, RecordNumber \= %2, EventTime \= %3, ActivityDefinitionId \= %4, Reason \= %5, Annotations \= %6, ProfileName \= %7  
  
## Dettagli  
  
|Nome elemento dati|Tipo elemento dati|Descrizione|  
|------------------------|------------------------|-----------------|  
|InstanceId|xs:GUID|ID istanza del flusso di lavoro.|  
|RecordNumber|xs:long|Numero di sequenza del record creato.|  
|EventTime|xs:dateTime|Ora di creazione dell'evento in UTC.|  
|ActivityDefinitionId|xs:string|Nome dell'attività radice nel flusso di lavoro.|  
|Reason|xs:string|Motivo per il quale il flusso di lavoro viene terminato.|  
|Annotations|xs:string|Annotazioni aggiunte a questo evento.I valori sono archiviati in un elemento xml nel formato \<items\>\< nome elemento \= "annotationName" tipo\="System.String"\>annotationValue\<\/item\>\<\/items\>.Se non è specificata alcuna annotazione, la stringa contiene \<items\/\>.La dimensione dell'evento ETW è limitata da quella del buffer ETW o dal payload massimo per un evento ETW.Se la dimensione dell'evento supera i limiti ETW, l'evento viene troncato eliminando le annotazioni e sostituendo il valore di annotazione con \<items\>...\<\/items.\>|  
|ProfileName|xs:string|Nome o profilo di rilevamento che ha determinato la creazione di questo evento.|  
|HostReference|xs:string|Per i servizi ospitati su Web, questo campo identifica in modo univoco il servizio nella gerarchia Web.Il relativo formato è definito come 'Nome sito Web&#124;Percorso virtuale applicazione&#124;Percorso virtuale servizio&#124;NomeServizio' Esempio: 'Sito Web predefinito\/CalculatorApplication&#124;\/CalculatorService.svc&#124;CalculatorService'|  
|AppDomain|xs:string|Stringa restituita da AppDomain.CurrentDomain.FriendlyName.|