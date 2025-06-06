---
audience: end-user
title: Utilizzare l’attività Arricchimento nei flussi di lavoro
description: Scopri come utilizzare l’attività Arricchimento nei flussi di lavoro
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 35%

---


# Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Attività Arricchimento"
>abstract="L’attività di **Arricchimento** consente di migliorare i dati mirati con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di segmentazione."

L’attività **Arricchimento** è un’attività di **targeting**. Migliora i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di segmentazione.

I dati di arricchimento possono provenire da:

* **La stessa tabella di lavoro** di quella di destinazione nel flusso di lavoro:
   * Esegui il targeting di un gruppo di clienti e aggiungi il campo &quot;Data di nascita&quot; alla tabella di lavoro corrente.

* **Altra tabella di lavoro**:
   * Eseguire il targeting di un gruppo di clienti e aggiungere i campi &quot;Importo&quot; e &quot;Tipo di prodotto&quot; dalla tabella &quot;Acquisto&quot;.

Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività successive per segmentare i clienti in gruppi distinti in base a comportamenti, preferenze e esigenze. Può essere utilizzato anche per creare messaggi di marketing personalizzati e campagne che risuonano con il pubblico di destinazione.

Ad esempio, puoi aggiungere alla tabella del flusso di lavoro informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro ultimo acquisto o l’importo speso per tali acquisti.

## Aggiungere un’attività Enrichment {#enrichment-configuration}

Per configurare l’attività **Arricchimento** segui questi passaggi:

1. Aggiungi attività come **Crea pubblico** e **Combina**.
1. Aggiungi un’attività **Arricchimento**.
1. Se nel flusso di lavoro sono configurate più transizioni, utilizza il campo **[!UICONTROL Set principale]** per definire quale transizione deve essere utilizzata come set principale per l&#39;arricchimento.

## Aggiungi dati di arricchimento {#enrichment-add}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Dati di arricchimento"
>abstract="Seleziona i dati da utilizzare per arricchire il flusso di lavoro. Puoi selezionare due tipi di dati di arricchimento: un attributo di arricchimento singolo dalla dimensione target oppure un collegamento raccolta, che è un collegamento con cardinalità 1-N tra le tabelle."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di Arricchimento"
>abstract="Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività successive per segmentare la clientela in gruppi distinti in base a comportamenti, preferenze ed esigenze, o per creare messaggi e campagne di marketing personalizzati in grado suscitare interesse nel pubblico target."

1. Fare clic su **Aggiungi dati di arricchimento** e selezionare l&#39;attributo da utilizzare per l&#39;arricchimento. [Scopri come selezionare gli attributi e aggiungerli ai preferiti](../../get-started/attributes.md).

   Puoi selezionare due tipi di dati di arricchimento: un singolo attributo di arricchimento dalla dimensione di destinazione o un collegamento di raccolta. Ogni tipo è descritto negli esempi seguenti:
   * [Attributo di arricchimento singolo](#single-attribute)
   * [Collegamento di raccolta](#collection-link)

   >[!NOTE]
   >
   >Il pulsante **Modifica espressione** nella schermata di selezione degli attributi consente di creare espressioni avanzate per selezionare l&#39;attributo. [Scopri come utilizzare l&#39;editor espressioni](../../query/expression-editor.md).

   ![Schermata che mostra la schermata di selezione dei dati di arricchimento](../assets/workflow-enrichment1.png)

## Creare collegamenti tra tabelle {#create-links}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Definizione dei collegamenti"
>abstract="Crea un collegamento tra i dati della tabella di lavoro e il database di Adobe Campaign. Ad esempio, se carichi i dati da un file che contiene il numero di account, il paese e l’e-mail dei destinatari, puoi creare un collegamento alla tabella del paese per aggiornare queste informazioni nei rispettivi profili."

La sezione **[!UICONTROL Definizione collegamento]** consente di creare un collegamento tra i dati della tabella di lavoro e il database di Adobe Campaign. Ad esempio, se carichi i dati da un file che contiene il numero di account, il paese e l’e-mail dei destinatari, puoi creare un collegamento alla tabella del paese per aggiornare queste informazioni nei rispettivi profili.

Sono disponibili diversi tipi di collegamenti:

* Collegamento semplice con cardinalità **[!UICONTROL 1]**: ogni record del set principale è associato a un solo record dei dati collegati.
* Collegamento semplice **[!UICONTROL 0 o 1 cardinalità]**: ogni record del set principale è associato a 0 o 1 record dei dati collegati, ma non a più di uno.
* **[!UICONTROL N collegamento raccolta cardinalità]**: ogni record del set principale è associato a 0, 1 o più record (N) dei dati collegati.

Per creare un collegamento, effettua le seguenti operazioni:

1. Nella sezione **[!UICONTROL Definizione collegamento]**, fare clic sul pulsante **[!UICONTROL Aggiungi collegamento]**.

   ![Schermata che mostra la sezione di definizione del collegamento](../assets/workflow-enrichment-link.png)

1. Nell&#39;elenco a discesa **Tipo di relazione**, scegliere il tipo di collegamento che si desidera creare.

1. Identifica la destinazione a cui vuoi collegare il set principale:

   * Per collegare una tabella esistente nel database, scegliere **[!UICONTROL Schema del database]** e selezionare la tabella desiderata dal campo **[!UICONTROL Schema di destinazione]**.
   * Per collegare i dati della transizione di input, scegliere **Schema temporaneo** e selezionare la transizione di cui si desidera utilizzare i dati.

1. Definisci i criteri di riconciliazione per far corrispondere i dati del set principale con lo schema collegato. Sono disponibili due tipi di join:

   * **Unione semplice**: seleziona un attributo specifico che corrisponda ai dati dei due schemi. Fai clic su **Aggiungi join** e seleziona gli attributi **Source** e **Destination** da utilizzare come criteri di riconciliazione.
   * **Advanced join**: crea un join utilizzando condizioni avanzate. Fai clic su **Aggiungi join** e sul pulsante **Crea condizione** per aprire Query Modeler.

Un esempio di flusso di lavoro che utilizza i collegamenti è disponibile nella sezione [Esempi](#link-example).

## Riconciliazione dei dati {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Riconciliazione"
>abstract="L’attività di **arricchimento** del flusso di lavoro può ora essere utilizzata per riconciliare i dati dallo schema del database di Campaign con i dati di un altro schema o con i dati provenienti da uno schema temporaneo, ad esempio i dati caricati tramite un’attività Carica file. Questo tipo di collegamento definisce una riconciliazione verso un record univoco. Adobe Campaign crea un collegamento a una tabella di destinazione aggiungendo una chiave esterna per la memorizzazione di un riferimento al record univoco."

L’attività di **arricchimento** del flusso di lavoro può ora essere utilizzata per riconciliare i dati dallo schema del database di Campaign con i dati di un altro schema o con i dati provenienti da uno schema temporaneo, ad esempio i dati caricati tramite un’attività Carica file. Questo tipo di collegamento definisce una riconciliazione verso un record univoco. Adobe Campaign crea un collegamento a una tabella di destinazione aggiungendo una chiave esterna per la memorizzazione di un riferimento al record univoco.

Ad esempio, puoi utilizzare questa opzione per riconciliare il paese di un profilo, specificato in un file caricato, con uno dei paesi disponibili nella tabella dedicata del database di Campaign.

Segui i passaggi per configurare un&#39;attività **Enrichment** con un collegamento di riconciliazione:

1. Fai clic sul pulsante **Aggiungi collegamento** nella sezione **Riconciliazione**.
1. Identifica i dati con cui desideri creare un collegamento di riconciliazione.

   * Per creare un collegamento di riconciliazione con i dati del database Campaign, selezionare **Schema del database** e scegliere lo schema in cui è memorizzata la destinazione.
   * Per creare un collegamento di riconciliazione con i dati provenienti dalla transizione di input, selezionare **Schema temporaneo** e scegliere la transizione del flusso di lavoro in cui vengono memorizzati i dati di destinazione.

1. I campi **Etichetta** e **Nome** vengono compilati automaticamente in base allo schema di destinazione selezionato. Se necessario, è possibile modificarne i valori.

1. Nella sezione **Criteri di riconciliazione** specificare la modalità di riconciliazione dei dati delle tabelle di origine e di destinazione:

   * **Unione semplice**: riconciliare un campo specifico della tabella di origine con un altro campo della tabella di destinazione. A tale scopo, fare clic sul pulsante **Aggiungi join** e specificare i campi **Source** e **Destination** da utilizzare per la riconciliazione.

     >[!NOTE]
     >
     >È possibile utilizzare uno o più criteri di **Unione semplice**, nel qual caso devono essere tutti verificati in modo che i dati possano essere collegati tra loro.

   * **Unione avanzata**: utilizza il modellatore di query per configurare i criteri di riconciliazione. A questo scopo, fai clic sul pulsante **Crea condizione**, quindi definisci i criteri di riconciliazione creando la tua regola utilizzando le operazioni AND e OR.

L&#39;esempio seguente mostra un flusso di lavoro configurato per creare un collegamento tra la tabella dei destinatari del database di Adobe Campaign e una tabella temporanea generata da un&#39;attività **Load file**. In questo esempio, l’attività Enrichment esegue la riconciliazione di entrambe le tabelle utilizzando l’indirizzo e-mail come criterio di riconciliazione.

![](../assets/enrichment-reconciliation.png)

## Aggiungere offerte {#add-offers}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_offer_proposition"
>title="Proposta di offerta"
>abstract="L’attività Arricchimento ti consente di aggiungere offerte per ciascun profilo."

L&#39;attività **[!UICONTROL Enrichment]** ti consente di aggiungere offerte per ciascun profilo.

A tale scopo, segui la procedura per configurare un&#39;attività **[!UICONTROL Enrichment]** con un&#39;offerta:

1. Nell&#39;attività **[!UICONTROL Enrichment]**, nella sezione **[!UICONTROL Proposta di offerte]**, fare clic sul pulsante **[!UICONTROL Aggiungi offerta]**

   ![](../assets/enrichment-addoffer.png)

1. Sono disponibili due opzioni per la selezione dell’offerta:

   * **[!UICONTROL Cerca l&#39;offerta migliore nella categoria]**: seleziona questa opzione e specifica i parametri di chiamata del motore di offerta (spazio dell&#39;offerta, categoria o temi, data di contatto, numero di offerte da mantenere). Il motore calcolerà le offerte migliori da aggiungere in base a questi parametri. È consigliabile completare il campo Categoria o Tema, anziché entrambi contemporaneamente.

     ![](../assets/enrichment-bestoffer.png)

   * **[!UICONTROL Offerta predefinita]**: seleziona questa opzione e specifica uno spazio dell&#39;offerta, un&#39;offerta specifica e una data di contatto per configurare direttamente l&#39;offerta da aggiungere senza chiamare il motore delle offerte.

     ![](../assets/enrichment-predefinedoffer.png)

1. Dopo aver selezionato l&#39;offerta, fai clic sul pulsante **[!UICONTROL Conferma]**.

Ora puoi utilizzare l’offerta nell’attività di consegna.

### Utilizzo delle offerte dall’attività Enrichment

All’interno di un flusso di lavoro, se desideri utilizzare le offerte che ottieni da un’attività di arricchimento nella consegna, segui i passaggi seguenti:

1. Apri l’attività di consegna e vai nell’edizione dei contenuti. Fai clic sul pulsante **[!UICONTROL Impostazioni offerte]** e seleziona nell&#39;elenco a discesa lo spazio **[!UICONTROL Offerte]** corrispondente alla tua offerta.
Se si desidera visualizzare solo le offerte dell&#39;attività di arricchimento, impostare il numero di **[!UICONTROL proposte]** su 0 e salvare le modifiche.

   ![](../assets/offers-settings.png)

1. Nella finestra di progettazione e-mail, quando si aggiunge una personalizzazione con offerte, fare clic sull&#39;icona **[!UICONTROL Proposte]** per visualizzare le offerte ottenute dall&#39;attività **[!UICONTROL Arricchimento]**. Apri l’offerta da scegliere facendo clic su di essa.

   ![](../assets/offers-propositions.png)

   Accedi a **[!UICONTROL Funzioni di rendering]** e scegli **[!UICONTROL Rendering HTML]** o **[!UICONTROL Rendering testo]** in base alle tue esigenze.

   ![](../assets/offers-rendering.png)

>[!NOTE]
>
>Se scegli di avere più di un&#39;offerta nell&#39;attività **[!UICONTROL Arricchimento]** all&#39;opzione **[!UICONTROL Numero di offerte da mantenere]**, tutte le offerte vengono visualizzate quando si fa clic sull&#39;icona **[!UICONTROL Proposte]**.

## Esempi {#example}

### Attributo di arricchimento singolo {#single-attribute}

In questo caso, viene semplicemente aggiunto un attributo di arricchimento singolo, ad esempio, la data di nascita. Segui questi passaggi:

1. Fai clic all’interno del campo **Attributo**.
1. Seleziona un campo semplice dalla dimensione di targeting, nel nostro esempio la data di nascita.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment2.png)

### Collegamento di raccolta {#collection-link}

In questo caso d’uso più complesso, selezioneremo un collegamento di raccolta che è un collegamento con cardinalità 1-N tra le tabelle. Recuperiamo i tre ultimi acquisti che sono inferiori a 100 $. A questo scopo è necessario definire:

* un attributo di arricchimento: il campo **Prezzo**
* il numero di righe da recuperare: 3
* un filtro: per escludere gli articoli superiori a 100 $
* un ordinamento: ordinamento decrescente nel campo **Data ordine**.

#### Aggiungere l’attributo {#add-attribute}

Qui puoi selezionare il collegamento di raccolta da utilizzare come dati di arricchimento.

1. Fai clic all’interno del campo **Attributo**.
1. Fai clic su **Visualizza gli attributi avanzati**.
1. Selezionare il campo **Prezzo** dalla tabella **Acquisti**.

<!-- ![](../assets/workflow-enrichment3.png) -->

#### Definire le impostazioni di raccolta{#collection-settings}

A questo punto, definisci come vengono raccolti i dati e quanti record recuperare.

1. Seleziona **Raccogli dati** nel menu a discesa **Seleziona la modalità di raccolta dei dati**.
1. Digita “3” nel campo **Righe da recuperare (colonne da creare)**.

![](../assets/workflow-enrichment4bis.png)

Se, ad esempio, desideri ottenere l’importo medio degli acquisti per un cliente, seleziona **Dati aggregati** e seleziona **Media** nel menu a discesa **Funzione di aggregazione**.

Utilizza i campi **Etichetta** e **Alias** del tuo attributo per renderlo più comprensibile, come illustrato di seguito.

![](../assets/workflow-enrichment5bis.png)

#### Definire i filtri{#collection-filters}

Ora puoi definire il valore massimo per l’attributo di arricchimento. Gli elementi superiori a 100$ vengono filtrati. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

1. Fai clic su **Crea filtri**.
1. Aggiungi i due seguenti filtri: **Il prezzo** esiste E **Il prezzo** è inferiore a 100. Il primo filtra i valori NULL, in quanto apparirebbero come il valore maggiore.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment6bis.png)

#### Definire l’ordinamento{#collection-sorting}

Ora è necessario applicare l’ordinamento per recuperare i tre acquisti **più recenti**.

1. Attiva l’opzione **Abilita ordinamento**.
1. Fai clic all’interno del campo **Attributo**.
1. Seleziona il campo **Data ordine**.
1. Fai clic su **Conferma**.
1. Seleziona **Decrescente** nel menu a discesa **Ordina**.

![](../assets/workflow-enrichment7bis.png)

### Arricchimento con dati collegati {#link-example}

L’esempio seguente mostra un flusso di lavoro configurato per creare un collegamento tra due transizioni. Le prime transizioni eseguono il targeting dei dati del profilo utilizzando un&#39;attività **Query**, mentre la seconda transizione include i dati di acquisto memorizzati in un file caricato tramite un&#39;attività Load file.

![](../assets/enrichment-uc-link.png)

* La prima attività **Enrichment** collega il set principale (dati dell&#39;attività **Query**) allo schema dell&#39;attività **Load file**. Questo ci consente di far corrispondere ogni profilo target della query con i dati di acquisto corrispondenti.

  ![](../assets/enrichment-uc-link-purchases.png)

* È stata aggiunta una seconda attività **Enrichment** per arricchire i dati della tabella del flusso di lavoro con i dati di acquisto provenienti dall&#39;attività **Load file**. Questo ci consente di utilizzare tali dati in ulteriori attività, ad esempio per personalizzare i messaggi inviati ai clienti con le informazioni sul loro acquisto.

  ![](../assets/enrichment-uc-link-data.png)

