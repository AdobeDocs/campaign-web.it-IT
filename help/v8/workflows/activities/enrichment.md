---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Arricchimento
description: Scopri come utilizzare l’attività del flusso di lavoro Arricchimento
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 93%

---


# Arricchimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Attività di arricchimento"
>abstract="L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzato in un flusso di lavoro dopo le attività di targeting.<br/>Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico di destinazione."

L’attività di arricchimento consente di migliorare i dati di destinazione con informazioni aggiuntive provenienti dal database. Viene comunemente utilizzata in un flusso di lavoro dopo le attività di targeting.

I dati di arricchimento possono provenire:

* **Dalla stessa tabella di lavoro** come quella che è stata inserita nel flusso di lavoro:

   *Eseguire il targeting di un gruppo di clienti e aggiungere il campo “Data di nascita” alla tabella di lavoro corrente*

* **Da un’altra tabella di lavoro**:

   *Eseguire il targeting di un gruppo di clienti e aggiungere i campi “Importo” e “Tipo di prodotto” provenienti dalla tabella “Acquisto”*.

Una volta aggiunti al flusso di lavoro, i dati di arricchimento possono essere utilizzati nelle attività aggiunte dopo l’attività di arricchimento per segmentare i clienti in gruppi distinti in base ai loro comportamenti, preferenze e esigenze, o per creare messaggi e campagne di marketing personalizzati che hanno maggiori probabilità di risonanza nel pubblico di destinazione.

Ad esempio, è possibile aggiungere alla tabella di lavoro del flusso di lavoro le informazioni relative agli acquisti dei clienti e utilizzare questi dati per personalizzare le e-mail con il loro acquisto più recente o con l’importo speso per tali acquisti.

Per aggiungere un’attività di arricchimento nel flusso di lavoro, segui i passaggi seguenti:

1. aggiungi attività
1. seleziona l’attributo da utilizzare come dato di arricchimento

   visualizza opzione campi avanzati
pulsante

   nota: attributi dalla dimensione di destinazione

1. Seleziona la modalità di raccolta dei dati
1. numero di record da recuperare se si desidera recuperare una raccolta di più record
1. Applica filtri e crea regole

   seleziona un filtro esistente
salva filtro per riutilizzo
visualizza risultati del filtro visivamente o in vista codice

1. ordina i record utilizzando un attributo

riutilizza i dati di arricchimento nella campagna

dove si possono utilizzare i dati di arricchimento: personalizzazione e-mail, altri casi d’uso?

