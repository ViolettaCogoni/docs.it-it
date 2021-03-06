---
title: "Procedura: formattare il controllo DataGrid di Windows Form | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-winforms"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "jsharp"
helpviewer_keywords: 
  - "colori, applicazione a controlli DataGrid"
  - "colonne [Windows Form], controllo DataGrid"
  - "colonne [Windows Form], formattazione nel controllo DataGrid"
  - "DataGrid (controllo) [Windows Form], stili predefiniti"
  - "DataGrid (controllo) [Windows Form], formattazione"
  - "formattazione [Windows Form]"
  - "tabelle [Windows Form], formattazione nel controllo DataGrid"
ms.assetid: a50fcc3b-8abf-47ec-9029-7f268af4ddb1
caps.latest.revision: 14
author: "dotnet-bot"
ms.author: "dotnetcontent"
manager: "wpickett"
caps.handback.revision: 14
---
# Procedura: formattare il controllo DataGrid di Windows Form
> [!NOTE]
>  Benché il controllo <xref:System.Windows.Forms.DataGridView> sostituisca il controllo <xref:System.Windows.Forms.DataGrid> aggiungendovi funzionalità, il controllo <xref:System.Windows.Forms.DataGrid> viene mantenuto per compatibilità con le versioni precedenti e per un eventuale utilizzo futuro.  Per ulteriori informazioni vedere [Differenze tra i controlli DataGridView e DataGrid di Windows Form](../../../../docs/framework/winforms/controls/differences-between-the-windows-forms-datagridview-and-datagrid-controls.md).  
  
 L'utilizzo di colori diversi per le parti di un controllo <xref:System.Windows.Forms.DataGrid> può contribuire ad agevolare la lettura e l'interpretazione delle informazioni in esso contenute.  È possibile applicare i colori alle righe e alle colonne.  La visualizzazione delle righe e delle colonne può inoltre essere attivata o disattivata a discrezione dell'utente.  
  
 La formattazione del controllo <xref:System.Windows.Forms.DataGrid> è caratterizzata da tre aspetti di base.  È possibile impostare proprietà per stabilire uno stile predefinito da utilizzare per la visualizzazione dei dati.  A partire da tale base, è quindi possibile personalizzare l'aspetto di alcune tabelle visualizzate in fase di esecuzione.  È infine possibile modificare le colonne da visualizzare nella griglia dei dati, nonché i colori e gli altri attributi di formattazione.  
  
 Il primo passaggio per la formattazione di una griglia dei dati può prevedere l'impostazione delle proprietà del controllo <xref:System.Windows.Forms.DataGrid>.  Le selezioni relative al colore e al formato costituiscono la base di partenza per apportare modifiche sulla base delle tabelle e delle colonne dati visualizzate.  
  
### Per stabilire uno stile predefinito per il controllo DataGrid  
  
1.  Impostare le seguenti proprietà a seconda dei casi:  
  
    |Proprietà|Descrizione|  
    |---------------|-----------------|  
    |<xref:System.Windows.Forms.DataGrid.AlternatingBackColor%2A>|La proprietà <xref:System.Windows.Forms.DataGrid.BackColor%2A> consente di definire il colore delle righe pari della griglia.  Quando si imposta la proprietà <xref:System.Windows.Forms.DataGrid.AlternatingBackColor%2A> su un colore diverso, tutte le righe dispari vengono impostate sul nuovo colore \(righe 1, 3, 5 e così via\).|  
    |<xref:System.Windows.Forms.DataGrid.BackColor%2A>|Colore di sfondo delle righe pari della griglia \(righe 0, 2, 4, 6 e così via\).|  
    |<xref:System.Windows.Forms.DataGrid.BackgroundColor%2A>|Mentre le proprietà <xref:System.Windows.Forms.DataGrid.BackColor%2A> e <xref:System.Windows.Forms.DataGrid.AlternatingBackColor%2A> determinano il colore delle righe della griglia, la proprietà <xref:System.Windows.Forms.DataGrid.BackgroundColor%2A> consente di stabilire il colore dell'area non occupata da righe, visibile solo quando si scorre la griglia fino alla fine, oppure se la griglia comprende solo poche righe.|  
    |<xref:System.Windows.Forms.DataGrid.BorderStyle%2A>|Stile del bordo della griglia; uno dei valori di enumerazione di <xref:System.Windows.Forms.BorderStyle>.|  
    |<xref:System.Windows.Forms.DataGrid.CaptionBackColor%2A>|Colore di sfondo della didascalia della finestra della griglia, visualizzata appena sopra la griglia.|  
    |<xref:System.Windows.Forms.DataGrid.CaptionFont%2A>|Carattere della didascalia nella parte superiore della griglia.|  
    |<xref:System.Windows.Forms.DataGrid.CaptionForeColor%2A>|Colore di sfondo della didascalia della finestra della griglia.|  
    |<xref:System.Windows.Forms.Control.Font%2A>|Carattere utilizzato per visualizzare il testo nella griglia.|  
    |<xref:System.Windows.Forms.DataGrid.ForeColor%2A>|Colore del carattere utilizzato per la visualizzazione dei dati nelle righe della griglia.|  
    |<xref:System.Windows.Forms.DataGrid.GridLineColor%2A>|Colore delle linee della griglia dei dati.|  
    |<xref:System.Windows.Forms.DataGrid.GridLineStyle%2A>|Stile delle linee di separazione delle celle nella griglia; uno dei valori di enumerazione di <xref:System.Windows.Forms.DataGridLineStyle>.|  
    |<xref:System.Windows.Forms.DataGrid.HeaderBackColor%2A>|Colore di sfondo delle intestazioni di riga e colonna.|  
    |<xref:System.Windows.Forms.DataGrid.HeaderFont%2A>|Carattere utilizzato per le intestazioni di colonna.|  
    |<xref:System.Windows.Forms.DataGrid.HeaderForeColor%2A>|Colore di primo piano delle intestazioni di colonna della griglia, compreso il testo dell'intestazione e i segni più\/meno \(\+\/\-\) che consentono di espandere le righe quando vengono visualizzate più tabelle correlate.|  
    |<xref:System.Windows.Forms.DataGrid.LinkColor%2A>|Colore del testo di tutti i collegamenti presenti nella griglia dei dati, compresi quelli alle tabelle figlio, al nome della relazione e così via.|  
    |<xref:System.Windows.Forms.DataGrid.ParentRowsBackColor%2A>|Colore di sfondo delle righe padre in una tabella figlio.|  
    |<xref:System.Windows.Forms.DataGrid.ParentRowsForeColor%2A>|Colore di primo piano delle righe padre in una tabella figlio.|  
    |<xref:System.Windows.Forms.DataGrid.ParentRowsLabelStyle%2A>|Consente di stabilire se i nomi della tabella e delle colonne vengono visualizzati nella riga padre tramite l'enumerazione <xref:System.Windows.Forms.DataGridParentRowsLabelStyle>.|  
    |<xref:System.Windows.Forms.DataGrid.PreferredColumnWidth%2A>|Larghezza predefinita \(in pixel\) delle colonne della griglia.  Impostare questa proprietà prima di reimpostare le proprietà <xref:System.Windows.Forms.DataGrid.DataSource%2A> e <xref:System.Windows.Forms.DataGrid.DataMember%2A> \(singolarmente o tramite il metodo <xref:System.Windows.Forms.DataGrid.SetDataBinding%2A>\). In caso contrario, la proprietà non avrà effetto.<br /><br /> Specificare un valore superiore a 0.|  
    |<xref:System.Windows.Forms.DataGrid.PreferredRowHeight%2A>|Altezza predefinita \(in pixel\) delle righe della griglia.  Impostare questa proprietà prima di reimpostare le proprietà <xref:System.Windows.Forms.DataGrid.DataSource%2A> e <xref:System.Windows.Forms.DataGrid.DataMember%2A> \(singolarmente o tramite il metodo <xref:System.Windows.Forms.DataGrid.SetDataBinding%2A>\). In caso contrario, la proprietà non avrà effetto.<br /><br /> Specificare un valore superiore a 0.|  
    |<xref:System.Windows.Forms.DataGrid.RowHeaderWidth%2A>|Larghezza delle intestazioni di riga della griglia.|  
    |<xref:System.Windows.Forms.DataGrid.SelectionBackColor%2A>|Colore di sfondo quando si seleziona una cella o una riga.|  
    |<xref:System.Windows.Forms.DataGrid.SelectionForeColor%2A>|Colore di primo piano quando si seleziona una cella o una riga.|  
  
    > [!NOTE]
    >  Durante la personalizzazione dei colori dei controlli, tenere presente che il controllo potrebbe risultare inaccessibile se il numero di colori disponibili è limitato, ad esempio a rosso e verde.  Per ovviare a questo problema, utilizzare i colori disponibili nella tavolozza **Colori di sistema**.  
  
     Nelle procedure riportate di seguito si presuppone che il form contenga un controllo <xref:System.Windows.Forms.DataGrid> associato a una tabella dati.  Per ulteriori informazioni, vedere [Associazione del controllo DataGrid Windows Form a un'origine dati](../../../../docs/framework/winforms/controls/how-to-bind-the-windows-forms-datagrid-control-to-a-data-source.md).  
  
### Per impostare lo stile di tabella e colonne di una tabella dati a livello di codice  
  
1.  Creare un nuovo stile di tabella e impostarne le proprietà.  
  
2.  Creare un nuovo stile di colonna e impostarne le proprietà.  
  
3.  Aggiungere lo stile di colonna alla raccolta degli stili di colonna degli stili di tabella.  
  
4.  Aggiungere lo stile di tabella alla raccolta degli stili di tabella della griglia.  
  
5.  Nell'esempio riportato di seguito, creare un'istanza di un nuovo <xref:System.Windows.Forms.DataGridTableStyle> e impostare la relativa proprietà <xref:System.Windows.Forms.DataGridTableStyle.MappingName%2A>.  
  
6.  Creare una nuova istanza di un controllo **GridColumnStyle** e impostarne la proprietà **MappingName** ed eventuali altre proprietà relative al layout e alla visualizzazione.  
  
7.  Ripetere i passaggi da 2 a 6 per ogni stile di colonna da creare.  
  
     Nell'esempio seguente viene illustrata la creazione di un controllo <xref:System.Windows.Forms.DataGridTextBoxColumn>, poiché nella colonna deve essere visualizzato un nome.  Viene inoltre aggiunto lo stile di colonna all'insieme <xref:System.Windows.Forms.GridColumnStylesCollection> dello stile di tabella e lo stile di tabella all'insieme <xref:System.Windows.Forms.GridTableStylesCollection> della griglia dei dati.  
  
    ```vb  
    Private Sub CreateAuthorFirstNameColumn()  
       ' Add a GridTableStyle and set the MappingName   
       ' to the name of the DataTable.  
       Dim TSAuthors As New DataGridTableStyle()  
       TSAuthors.MappingName = "Authors"  
  
       ' Add a GridColumnStyle and set the MappingName   
       ' to the name of a DataColumn in the DataTable.   
       ' Set the HeaderText and Width properties.   
       Dim TCFirstName As New DataGridTextBoxColumn()  
       TCFirstName.MappingName = "AV_FName"  
       TCFirstName.HeaderText = "First Name"  
       TCFirstName.Width = 75  
       TSAuthors.GridColumnStyles.Add(TCFirstName)  
  
       ' Add the DataGridTableStyle instance to   
       ' the GridTableStylesCollection.   
       myDataGrid.TableStyles.Add(TSAuthors)  
    End Sub  
  
    ```  
  
    ```csharp  
    private void addCustomDataTableStyle()  
    {  
       // Add a GridTableStyle and set the MappingName   
       // to the name of the DataTable.  
       DataGridTableStyle TSAuthors = new DataGridTableStyle();  
       TSAuthors.MappingName = "Authors";  
  
       // Add a GridColumnStyle and set the MappingName   
       // to the name of a DataColumn in the DataTable.   
       // Set the HeaderText and Width properties.   
       DataGridColumnStyle TCFirstName = new DataGridTextBoxColumn();  
       TCFirstName.MappingName = " AV_FName";  
       TCFirstName.HeaderText = "First Name";  
       TCFirstName.Width = 75;  
       TSAuthors.GridColumnStyles.Add(TCFirstName);  
  
       // Add the DataGridTableStyle instance to   
       // the GridTableStylesCollection.   
       dataGrid1.TableStyles.Add(TSAuthors);  
    }  
  
    ```  
  
    ```cpp  
    private:  
       void addCustomDataTableStyle()  
       {  
          // Add a GridTableStyle and set the MappingName   
          // to the name of the DataTable.  
          DataGridTableStyle^ TSAuthors = new DataGridTableStyle();  
          TSAuthors->MappingName = "Authors";  
  
          // Add a GridColumnStyle and set the MappingName   
          // to the name of a DataColumn in the DataTable.   
          // Set the HeaderText and Width properties.   
          DataGridColumnStyle^ TCFirstName = gcnew DataGridTextBoxColumn();  
          TCFirstName->MappingName = "AV_FName";  
          TCFirstName->HeaderText = "First Name";  
          TCFirstName->Width = 75;  
          TSAuthors->GridColumnStyles->Add(TCFirstName);  
  
          // Add the DataGridTableStyle instance to   
          // the GridTableStylesCollection.   
          dataGrid1->TableStyles->Add(TSAuthors);  
       }  
    ```  
  
## Vedere anche  
 <xref:System.Windows.Forms.GridTableStylesCollection>   
 <xref:System.Windows.Forms.GridColumnStylesCollection>   
 <xref:System.Windows.Forms.DataGrid>   
 [Procedura: eliminare o nascondere colonne nel controllo DataGrid Windows Form](../../../../docs/framework/winforms/controls/how-to-delete-or-hide-columns-in-the-windows-forms-datagrid-control.md)   
 [Controllo DataGrid](../../../../docs/framework/winforms/controls/datagrid-control-windows-forms.md)