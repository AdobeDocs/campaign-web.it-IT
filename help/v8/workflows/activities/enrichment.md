---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Arricchimento
description: Scopri come utilizzare l’attività del flusso di lavoro Arricchimento
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 99%

---


# Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di arricchimento"
>abstract="L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di targeting.<br/>Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico target."

L’attività **Arricchimento** è un’attività di **targeting**. Consente di migliorare i dati target con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di segmentazione.

I dati di arricchimento possono provenire:

* **Dalla stessa tabella di lavoro** come quella che è stata inserita nel flusso di lavoro:

  *Eseguire il targeting di un gruppo di clienti e aggiungere il campo “Data di nascita” alla tabella di lavoro corrente*

* **Da un’altra tabella di lavoro**:

  *Eseguire il targeting di un gruppo di clienti e aggiungere i campi “Importo” e “Tipo di prodotto” provenienti dalla tabella “Acquisto”*.

Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di **Arricchimento** per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico target.

Ad esempio, è possibile aggiungere alla tabella di lavoro del flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

## Configurazione generale {#general}

Per configurare l’attività di **Arricchimento** segui questi passaggi:

1. Aggiungi attività come **Creazione del pubblico** e **Combina**.
1. Aggiungi un’attività di **Arricchimento**.
1. Fai clic su **Aggiungi dati di arricchimento**.

![](../assets/workflow-enrichment1.png)

È possibile selezionare due tipi di dati di arricchimento: un [attributo di arricchimento singolo](#single-attribute) dalla dimensione target, oppure un [collegamento raccolta](#collection-link).

## Attributo di arricchimento singolo {#single-attribute}

In questo caso, stiamo semplicemente aggiungendo un attributo di arricchimento singolo, ad esempio, la data di nascita. Segui questi passaggi:

1. Fai clic all’interno del campo **Attributo**.
1. Seleziona un campo semplice dalla dimensione di targeting, nel nostro esempio la data di nascita.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment2.png)

## Collegamento raccolta {#collection-link}

In questo caso d’uso più complesso, selezioneremo un collegamento raccolta che è un collegamento con cardinalità 1-N tra le tabelle. Recuperiamo i tre ultimi acquisti che sono inferiori a 100 $. A questo scopo è necessario definire:

* un attributo di arricchimento: il campo **Importo totale**
* il numero di righe da recuperare: 3
* un filtro: esclusione dal filtro degli elementi superiori a 100 $
* un ordinamento: ordinamento discendente sul campo **Data ordine**.

### Aggiungi l’attributo

In questa posizione è possibile selezionare il collegamento raccolta da utilizzare come dati di arricchimento.

1. Fai clic all’interno del campo **Attributo**.
1. Fai clic su **Mostra attributi avanzati**.
1. Seleziona il campo **Importo totale** dalla tabella **Acquisti**.

![](../assets/workflow-enrichment3.png)

### Definisci le impostazioni della raccolta

Quindi, definisci come vengono raccolti i dati e il numero di record da recuperare.

1. Seleziona **Raccogli dati** nel menu a discesa **Seleziona la modalità di raccolta dei dati**.
1. Digita “3” nel campo **Righe da recuperare (colonne da creare)**.

![](../assets/workflow-enrichment4.png)

Se, ad esempio, desideri ottenere l’importo medio degli acquisti per un cliente, seleziona **Dati aggregati** e seleziona **Media** nel menu a discesa **Funzione di aggregazione**.

![](../assets/workflow-enrichment5.png)

### Definisci i filtri

In questo caso, viene definito il valore massimo per l’attributo di arricchimento. Gli elementi superiori a 100 $ vengono esclusi dal filtro.

1. Fai clic su **Modifica i filtri**.
1. Aggiungi i due filtri seguenti: l’**Importo totale** esiste E l’**Importo totale** è minore di 100. Il primo filtra i valori NULL così come apparirebbero come il valore maggiore.
1. Fai clic su **Conferma**.

![](../assets/workflow-enrichment6.png)

### Definisci l’ordinamento

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