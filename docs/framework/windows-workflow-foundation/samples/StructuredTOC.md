# [Esempi di flussi di lavoro di Windows](index.md)
## [Applicazione](application.md)
### [Processo di approvazione dei documenti](document-approval-process.md)
### [Processo di acquisto aziendale](corporate-purchase-process.md)
### [Processo di assunzione](hiring-process.md)
### [Rilevamento visivo del flusso di lavoro](visual-workflow-tracking.md)
### [Gestione dell'istanza sospesa](suspended-instance-management.md)
## [Basic](basic.md)
### [Attività predefinite](built-in-activities.md)
#### [Gestione errori in un'attività Flowchart utilizzando TryCatch](fault-handling-in-a-flowchart-activity-using-trycatch.md)
#### [Emulazione di interruzione in un'attività While](emulating-breaking-in-a-while-activity.md)
#### [DynamicActivityCreation](dynamicactivity-creation.md)
#### [Utilizzo di variabili con un set di regole di .NET Framework 3.5](using-variables-with-dotnet-ruleset.md)
#### [Caricare da XAML](load-from-xaml.md)
#### [Utilizzo delle attività di raccolta](using-collection-activities.md)
#### [Utilizzo dell'attività InvokeMethod](using-the-invokemethod-activity.md)
#### [Utilizzo dell'attività Pick](using-the-pick-activity.md)
#### [Utilizzo di attività procedurali](using-procedural-activities.md)
#### [Utilizzo dell'attività CancellationScope](using-cancellationscope.md)
#### [InvokeMethod](invokemethod.md)
#### [Utilizzo dell'attività Switch con tipi personalizzati](usage-of-the-switch-activity-with-custom-types.md)
#### [Interoperabilità con il set di regole 3.5](interop-with-3-5-rule-set.md)
### [Compensazione](compensation-samples.md)
#### [CompensableActivity](compensable-activity-sample.md)
#### [Compensazione personalizzata](custom-compensation-sample.md)
#### [Conferma](confirmation.md)
#### [Gestore di annullamento nell'attività compensabile](cancellation-handler-on-compensable-activity.md)
### [Attività personalizzate](custom-activities.md)
#### [Attività Code-Bodied](code-bodied.md)
##### [Segnalibri](bookmarks.md)
##### [Attività composta personalizzata tramite l'oggetto NativeActivity](custom-composite-using-native-activity.md)
##### [Proprietà di esecuzione](execution-properties.md)
##### [Esposizione e richiamo di ActivityAction](exposing-and-invoking-activityactions.md)
##### [Utilizzo di AsyncOperationContext in un'attività](using-asyncoperationcontext-in-an-activity-sample.md)
##### [Attività personalizzata Hello World](hello-world-custom-activity.md)
##### [Argomenti dinamici](dynamic-arguments.md)
#### [Composito](composite.md)
##### [Composizione dell'attività di base](basic-activity-composition.md)
##### [Guida introduttiva alla scrittura di un'attività personalizzata](getting-started-writing-a-custom-activity.md)
#### [ActivityDesigner personalizzati](custom-activity-designers.md)
##### [Finestre di progettazione composte personalizzate - relatore dell'elemento del flusso di lavoro](custom-composite-designers-workflow-item-presenter.md)
##### [Finestre di progettazione composite personalizzate - Relatore di elementi del flusso di lavoro](custom-composite-designers-workflow-items-presenter.md)
##### [Programmabilità dell'archivio di metadati](metadata-store-programmability.md)
##### [Utilizzo di ExpressionTextBox in un ActivityDesigner personalizzato](using-the-expressiontextbox-in-a-custom-activity-designer.md)
##### [Utilizzo dell'ambito di modifica](using-editing-scope.md)
#### [Convalida](validation.md)
##### [Tipi di vincoli](constraint-types.md)
### [Finestra di progettazione](designer.md)
#### [Rimozione dello stato di visualizzazione della finestra di progettazione per l'aggiunta a un file XAML](removing-the-view-state-the-designer-adds-to-an-xaml-file.md)
#### [Programmazione dell'albero degli elementi del modello](programming-model-item-tree.md)
#### [Estensibilità della griglia delle proprietà](property-grid-extensibliity.md)
#### [Servizio casella degli strumenti](toolbox-service.md)
### [Riallocazione della finestra di progettazione](designer-rehosting.md)
### [Esecuzione](execution.md)
#### [Esempio di endpoint di gestione del flusso di lavoro](workflow-management-endpoint-sample.md)
#### [Utilizzo della classe WorkflowInvoker](using-the-workflowinvoker-class.md)
#### [Host ReadLine di WorkflowApplication](workflowapplication-readline-host.md)
#### [Creazione ed esecuzione di un'istanza del flusso di lavoro](creating-and-running-a-workflow-instance.md)
#### [Segnalibro di ripresa WorkflowHostingEndpoint](workflowhostingendpoint-resume-bookmark.md)
#### [Risolver di segnalibri per WorkflowHostingEndpoint](bookmark-resolver-for-workflowhostingendpoint.md)
### [Espressioni](expressions.md)
### [Migrazione](migration.md)
#### [Utilizzo di un'attività di .NET Framework 3.0 o .NET Framework 3.5 in un flusso di lavoro di .NET Framework 4.5](using-a-net-3-0-or-net-3-5-activity-in-a-net-4-5-workflow.md)
#### [Utilizzo di interoperabilità con scambio di dati esterni](using-interop-with-external-data-exchange.md)
### [Persistenza](persistence.md)
#### [Persistenza di un'applicazione flusso di lavoro](persisting-a-workflow-application.md)
#### [Configurazione predefinita](built-in-configuration.md)
#### [SQLStoreExtensibility](sqlstoreextensibility.md)
#### [Attività di promozione proprietà](property-promotion-activity.md)
### [Esempi di regole](rules-samples.md)
#### [Criteri avanzati](advanced-policy.md)
#### [Criteri semplici](simple-policy.md)
#### [IfElse con regole](ifelse-with-rules.md)
#### [ConditionedActivityGroup](conditioned-activity-group.md)
#### [Elaborazione di ordini con criteri](order-processing-with-policy.md)
### [Servizi](services.md)
#### [Ritardo assoluto](absolute-delay.md)
#### [Ritardo durevole](durable-delay.md)
#### [Invio e gestione di errori](sending-and-handling-faults.md)
#### [Utilizzo di base delle attività SendParameters e ReceiveParameters](basic-usage-of-sendparameters-and-receiveparameters-activities.md)
#### [Servizio solo XAML di base](basic-xaml-only-service.md)
#### [Formattazione di messaggi nei servizi flusso di lavoro](formatting-messages-in-workflow-services.md)
#### [Duplex durevole](durable-duplex.md)
#### [Correlazione basata sul contenuto](content-based-correlation.md)
#### [Memorizzazione nella cache dei canali con l'attività Send](channel-caching-with-send.md)
#### [Ritardo durevole in XAMLX](durable-delay-in-xamlx.md)
#### [Ricezione memorizzata nel buffer](buffered-receive.md)
#### [Attivazione XAML](xaml-activation.md)
### [Rilevamento](tracking.md)
#### [Rilevamento personalizzato](custom-tracking.md)
#### [Eventi di rilevamento in Traccia eventi per Windows](tracking-events-into-event-tracing-in-windows.md)
#### [Rilevamento SQL](sql-tracking.md)
#### [Estrarre dati di WF utilizzando il rilevamento](extract-wf-data-using-tracking.md)
#### [Rilevamento tramite un file di testo](tracking-using-a-text-file.md)
### [Transazioni](basic-transactions.md)
#### [TransactionScope di base](basic-transactionscope.md)
#### [Utilizzo di TransactedReceiveScope](use-of-transactedreceivescope.md)
#### [Annidamento di TransactionScope all'interno di un servizio](nesting-of-transactionscope-within-a-service.md)
### [Convalida](validation.md)
#### [Convalida di attività esterna](external-activity-validation.md)
#### [Convalida di base](basic-validation.md)
#### [OverloadGroups](overloadgroups.md)
#### [Convalida di relazioni tra attività](activity-relationships-validation.md)
## [Scenario](scenario.md)
### [Libreria di attività](activity-library.md)
#### [Attività Policy in .NET Framework 4.5](policy-activity-in-net-framework-4-5.md)
#### [Attività personalizzata per il passaggio in base a un intervallo di valori](custom-activity-to-switch-on-a-range-of-values.md)
#### [Attività LINQ to Objects](linq-to-objects-activity.md)
#### [LINQ to SQL](linq-to-sql-sample.md)
#### [Utilizzo dell'attività InvokePowerShell](using-the-invokepowershell-activity.md)
#### [Attività RangeEnumeration](rangeenumeration-activity.md)
#### [Attività di espressioni regolari](regular-expression-activities.md)
#### [Attività personalizzata SendMail](sendmail-custom-activity.md)
#### [Attività For](for-activity.md)
#### [Attività WaitForInput](wait-for-input-activity.md)
#### [ThrottledParallelForEach](throttled-parallel-foreach.md)
#### [Attività dell'entità](entity-activities.md)
#### [Attività di accesso al database](database-access-activities.md)
#### [Attività CommentOut](commentout-activity.md)
#### [Attività ExternalizedPolicy in .NET Framework 4.5](externalized-policy-activity-in-net-framework-4-5.md)
#### [Attività NoPersistScope](nopersistscope-activity.md)
#### [ForEach non generica](non-generic-foreach.md)
#### [Attività ParallelForEach non generica](non-generic-parallelforeach.md)
#### [Ottenere WorkflowInstanceId](get-workflowinstanceid.md)
### [Services](services.md)
#### [OperationScope](operationscope.md)
#### [Accesso a OperationContext](accessing-operationcontext.md)
#### [Correlazione di query del messaggio LINQ](linq-message-query-correlation.md)
#### [Calcolatrice correlata](correlated-calculator.md)
#### [Protezione di servizi flusso di lavoro](securing-workflow-services.md)
#### [Comunicazione asincrona](asynchronous-communication.md)
### [Transazioni](transactions.md)
#### [Eseguire un flusso di lavoro in un oggetto TransactionScope imperativo](execute-a-workflow-in-an-imperative-transactionscope.md)
#### [Ambito di istruzioni della transazione](transaction-convoy-scope.md)
#### [Rollback di transazioni](transaction-rollback.md)
#### [Eliminare l'ambito della transazione](suppress-transaction-scope.md)
#### [Code transazionali](transacted-queues.md)
### [Modello di conferma automatica](auto-confirm-pattern.md)
### [Scenario StateMachine utilizzando una combinazione attività FlowChart e Pick](statemachine-scenario-using-a-combination-of-flowchart-and-pick.md)
### [Integrazione di WPF e WF in XAML](wpf-and-wf-integration-in-xaml.md)
### [Toolkit di RuleSet esterno](external-ruleset-toolkit.md)