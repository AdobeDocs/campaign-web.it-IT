---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Arricchimento
description: Scopri come utilizzare l’attività del flusso di lavoro Arricchimento
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 28%

---


# Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di arricchimento"
>abstract="L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzato in un flusso di lavoro dopo le attività di targeting.<br/>Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico di destinazione."

Il **Arricchimento** l&#39;attività è un **Targeting** attività. Consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzato in un flusso di lavoro dopo le attività di segmentazione.

I dati di arricchimento possono provenire:

* **Dalla stessa tabella di lavoro** come quella che è stata inserita nel flusso di lavoro:

   *Eseguire il targeting di un gruppo di clienti e aggiungere il campo “Data di nascita” alla tabella di lavoro corrente*

* **Da un’altra tabella di lavoro**:

   *Eseguire il targeting di un gruppo di clienti e aggiungere i campi “Importo” e “Tipo di prodotto” provenienti dalla tabella “Acquisto”*.

Una volta aggiunti i dati di arricchimento al flusso di lavoro, questi possono essere utilizzati nelle attività aggiunte dopo **Arricchimento** attività per segmentare i clienti in gruppi distinti in base a comportamenti, preferenze e esigenze, oppure per creare messaggi di marketing e campagne personalizzati che hanno maggiori probabilità di risuonare con il pubblico di destinazione.

Ad esempio, è possibile aggiungere alla tabella di lavoro del flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

## Configurazione generale

Per configurare il **Arricchimento** attività:

1. Aggiungi attività come **Creare un pubblico** e **Combina** attività.
1. Aggiungi un **Arricchimento** attività.
1. Clic **Aggiungere dati di arricchimento**.

![](../assets/workflow-enrichment1.png)

Puoi selezionare due tipi di dati: un singolo attributo dalla dimensione di destinazione o un collegamento di raccolta.

## Attributo singolo

Qui stiamo solo aggiungendo un singolo attributo di arricchimento, per esempio, i dati di nascita. Segui questi passaggi:

1. Fai clic all’interno del **Attributo** campo.
1. Seleziona un campo semplice dalla dimensione di targeting, nel nostro esempio la data di nascita.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment2.png)

## Collegamento raccolta

In questo caso d’uso più complesso, selezioneremo un collegamento di raccolta che è un collegamento con cardinalità 1-N tra le tabelle. Recuperiamo i tre ultimi acquisti che sono inferiori a 100$. A questo scopo è necessario definire:

* un attributo: **Importo totale** campo
* numero di righe da recuperare: 3
* un filtro: filtra gli elementi superiori a 100$
* a ordinamento: ordinamento discendente sul **Data ordine** campo.

Segui questi passaggi:

### Aggiungi l’attributo

In questa posizione è possibile selezionare il collegamento di raccolta da utilizzare come dati di arricchimento.

1. Fai clic all’interno del **Attributo** campo.
1. Clic **Visualizzare attributi avanzati**.
1. Seleziona la **Importo totale** campo da **Acquisti** tabella.

![](../assets/workflow-enrichment3.png)

### Definire le impostazioni della raccolta

Quindi, definisci come vengono raccolti i dati e il numero di record da recuperare.

1. Seleziona **Raccogliere dati** nel **Seleziona la modalità di raccolta dei dati** a discesa.
1. Digita &quot;3&quot; nella **Righe da recuperare (colonne da creare)** campo.

![](../assets/workflow-enrichment4.png)

Se ad esempio si desidera ottenere l&#39;importo medio degli acquisti per un cliente, selezionare **Dati aggregati** e seleziona **Media** nel **Funzione di aggregazione** a discesa.

![](../assets/workflow-enrichment5.png)

### Definire i filtri

In questo caso, viene definito il valore massimo per l’attributo. Gli elementi superiori a 100$ vengono filtrati.

1. Clic **Modificare i filtri**.
1. Aggiungi i due seguenti filtri: **Importo totale** esiste AND **Importo totale** è minore di 100. Il primo filtra i valori NULL così come apparirebbero come il valore maggiore.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment6.png)

### Definire l’ordinamento

Ora è necessario applicare l’ordinamento per recuperare i tre **più recente** acquisti.

1. Attiva il **Abilita ordinamento** opzione.
1. Fai clic all’interno del **Attributo** campo.
1. Seleziona la **Data ordine** campo.
1. Fai clic su **Conferma**.
1. Seleziona **Decrescente** dal **Ordina** a discesa.

![](../assets/workflow-enrichment7.png)

<!--
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