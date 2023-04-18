---
audience: end-user
title: Utilizzare le attività di gestione dati dei flussi di lavoro
description: Scopri come utilizzare le attività di gestione dei dati nei flussi di lavoro web Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

---

# Attività di gestione dati {#data-management}

panoramica: cosa vengono utilizzati per il caso d’uso che è possibile eseguire con loro

elenco delle attività disponibili + descrizione breve + riferimento alla sezione

## Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di arricchimento"
>abstract="L’attività Arricchimento ti consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzato in un flusso di lavoro dopo le attività di targeting.<br/>Una volta aggiunti al flusso di lavoro i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività Enrichment per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno più probabilità di interessarsi al pubblico di destinazione."

L’attività Arricchimento ti consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzato in un flusso di lavoro dopo le attività di targeting.

I dati di arricchimento possono essere:

* **Dalla stessa tabella di lavoro** come target nel flusso di lavoro:

   *Eseguire il targeting di un gruppo di clienti e aggiungere il campo &quot;Data di nascita&quot; alla tabella di lavoro corrente*

* **Da un&#39;altra tabella di lavoro**:

   *Eseguire il targeting di un gruppo di clienti e aggiungere i campi &quot;Importo&quot; e &quot;Tipo di prodotto&quot; provenienti dalla tabella &quot;Acquisto&quot;*.

Una volta aggiunti al flusso di lavoro i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività Enrichment per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di interessarsi al pubblico di destinazione.

Ad esempio, puoi aggiungere al flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzarli per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

Per aggiungere un’attività Arricchimento nel flusso di lavoro, effettua le seguenti operazioni:

1. aggiungi attività
1. seleziona l’attributo da utilizzare come dati di arricchimento

   pulsante visualizza campi avanzati opzione i

   nota: attributi dalla dimensione di destinazione

1. Selezionare la modalità di raccolta dei dati
1. numero di record da recuperare se si desidera recuperare una raccolta di più record
1. Applicazione di filtri e creazione di regole

   seleziona un filtro esistente salva il filtro per riutilizzare i risultati della visualizzazione del filtro visivamente o in vista codice

1. ordinare i record utilizzando un attributo

sfruttare i dati di arricchimento nella campagna

dove possiamo utilizzare i dati di arricchimento: personalizzare e-mail e altri casi d’uso?
