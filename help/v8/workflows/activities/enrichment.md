---
audience: end-user
title: Utilizzare l’attività Arricchimento nei flussi di lavoro
description: Scopri come utilizzare l’attività Arricchimento nei flussi di lavoro
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 82%

---

# Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Attività Arricchimento"
>abstract="L’attività di **Arricchimento** consente di migliorare i dati mirati con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di segmentazione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di Arricchimento"
>abstract="Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di Arricchimento per segmentare la clientela in gruppi distinti in base ai comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico target."

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Dati di arricchimento"
>abstract="Seleziona i dati da utilizzare per arricchire il flusso di lavoro. Puoi selezionare due tipi di dati di arricchimento: un attributo di arricchimento singolo dalla dimensione target oppure un collegamento raccolta, che è un collegamento con cardinalità 1-N tra le tabelle."

L’attività **Arricchimento** è un’attività di **targeting**. Consente di migliorare i dati target con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di segmentazione.

I dati di arricchimento possono provenire:

* **Dalla stessa tabella di lavoro** definita come target nel flusso di lavoro:

  *Eseguire il targeting di un gruppo di clienti e aggiungere il campo &quot;Data di nascita&quot; alla tabella di lavoro corrente*.

* **Da un’altra tabella di lavoro**:

  *Esegui il targeting di un gruppo di clienti e aggiungere i campi “Importo” e “Tipo di prodotto” provenienti dalla tabella “Acquisto”*.

Una volta aggiunti i dati di arricchimento al flusso di lavoro, questi possono essere utilizzati nelle attività aggiunte dopo **Arricchimento** attività per segmentare i clienti in gruppi distinti in base a comportamenti, preferenze e esigenze, oppure per creare messaggi di marketing e campagne personalizzati che hanno maggiori probabilità di risuonare con il pubblico di destinazione.

Ad esempio, è possibile aggiungere alla tabella di lavoro del flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

## Configurare l’attività di Arricchimento {#enrichment-configuration}

Per configurare l’attività **Arricchimento** segui questi passaggi:

1. Aggiungi attività come **Crea pubblico** e **Combina**.
1. Aggiungi un’attività **Arricchimento**.
1. Clic **Aggiungere dati di arricchimento** e seleziona l’attributo da utilizzare per arricchire i dati.

   È possibile selezionare due tipi di dati di arricchimento: un [attributo di arricchimento singolo](#single-attribute) dalla dimensione target, oppure un [collegamento di raccolta](#collection-link).

   >[!NOTE]
   >
   >Il **Pulsante espressione Modifica** nella schermata di selezione degli attributi consente di creare espressioni avanzate per selezionare l’attributo. [Scopri come utilizzare l’editor di espressioni](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## Attributo di arricchimento singolo {#single-attribute}

In questo caso, viene semplicemente aggiunto un attributo di arricchimento singolo, ad esempio, la data di nascita. Segui questi passaggi:

1. Fai clic all’interno del campo **Attributo**.
1. Seleziona un campo semplice dalla dimensione di targeting, nel nostro esempio la data di nascita.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment2.png)

## Collegamento di raccolta {#collection-link}

In questo caso d’uso più complesso, selezioneremo un collegamento di raccolta che è un collegamento con cardinalità 1-N tra le tabelle. Recuperiamo i tre ultimi acquisti che sono inferiori a 100 $. A questo scopo è necessario definire:

* un attributo di arricchimento: il campo **Importo totale**
* il numero di righe da recuperare: 3
* un filtro: per escludere gli articoli superiori a 100 $
* un ordinamento: ordine decrescente sul campo **Data ordine**.

### Aggiungere l’attributo {#add-attribute}

Qui puoi selezionare il collegamento di raccolta da utilizzare come dati di arricchimento.

1. Fai clic all’interno del campo **Attributo**.
1. Fai clic su **Visualizza gli attributi avanzati**.
1. Seleziona il campo **Importo totale** dalla tabella **Acquisti**.

![](../assets/workflow-enrichment3.png)

### Definire le impostazioni di raccolta{#collection-settings}

A questo punto, definisci come vengono raccolti i dati e quanti record recuperare.

1. Seleziona **Raccogli dati** nel menu a discesa **Seleziona la modalità di raccolta dei dati**.
1. Digita “3” nel campo **Righe da recuperare (colonne da creare)**.

![](../assets/workflow-enrichment4.png)

Se, ad esempio, desideri ottenere l’importo medio degli acquisti per un cliente, seleziona **Dati aggregati** e seleziona **Media** nel menu a discesa **Funzione di aggregazione**.

![](../assets/workflow-enrichment5.png)

### Definire i filtri{#collection-filters}

Ora puoi definire il valore massimo per l’attributo di arricchimento. Gli elementi superiori a 100$ vengono filtrati. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

1. Fai clic su **Modifica filtri**.
1. Aggiungi i due filtri seguenti: **Importo totale** esiste E **Importo totale** è minore di 100. Il primo filtra i valori NULL, in quanto apparirebbero come il valore maggiore.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment6.png)

### Definire l’ordinamento{#collection-sorting}

Ora è necessario applicare l’ordinamento per recuperare i tre acquisti **più recenti**.

1. Attiva l’opzione **Abilita ordinamento**.
1. Fai clic all’interno del campo **Attributo**.
1. Seleziona il campo **Data ordine**.
1. Fai clic su **Conferma**.
1. Seleziona **Decrescente** nel menu a discesa **Ordina**.

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->
