---
audience: end-user
title: Utilizzare le attività dei flussi di lavoro
description: Scopri come utilizzare le attività dei flussi di lavoro
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 21%

---

# Informazioni sulle attività dei flussi di lavoro {#workflow-activities}

Le attività dei flussi di lavoro sono raggruppate in tre categorie. A seconda del contesto, le attività disponibili possono variare.

Tutte le attività sono descritte nelle sezioni seguenti:

* [Attività di targeting e gestione dei dati](#targeting)
* [Attività di canale](#channel)
* [Attività di controllo del flusso](#flow-control)

![Panoramica delle attività del flusso di lavoro](../assets/workflow-activities.png)

## Attività di targeting {#targeting}

Queste attività sono specifiche per il targeting. Consentono di creare uno o più tipi di pubblico di destinazione definendo un pubblico e suddividendo o combinando tali tipi di pubblico tramite operazioni di intersezione, unione o esclusione.

* [Genera pubblico](build-audience.md): definisci la popolazione target. Seleziona un pubblico esistente o utilizza il modellatore di query per definire una query personalizzata.
* [Modifica origine dati](change-data-source.md): modifica l&#39;origine dati per la tabella di lavoro del flusso di lavoro.
* [Modifica dimensione](change-dimension.md): modifica la dimensione di targeting durante la creazione del flusso di lavoro.
* [Combina](combine.md): esegui la segmentazione del gruppo in entrata. Utilizza un’unione, un’intersezione o un’esclusione.
* [Deduplicazione](deduplication.md): rimuovi i duplicati nei risultati delle attività in entrata.
* [Arricchimento](enrichment.md): definisci i dati aggiuntivi da elaborare nel flusso di lavoro. Configura l’attività per completare la transizione di output con dati aggiuntivi.
* [Query incrementale](incremental-query.md): esegui una query sul database su base pianificata. Ogni volta che questa attività viene eseguita, esclude i risultati dalle esecuzioni precedenti, eseguendo il targeting solo di nuovi elementi.
* [Riconciliazione](reconciliation.md): definire il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro, ad esempio i dati caricati da un file esterno.
* [Salva pubblico](save-audience.md): aggiorna un pubblico esistente o crea un nuovo pubblico dalla popolazione calcolata a monte in un flusso di lavoro.
* [Dividi](split.md): segmenta la popolazione in ingresso in diversi sottoinsiemi.

## Attività di gestione dati {#data}

Queste attività sono specifiche per la manipolazione e l’arricchimento dei dati sulla popolazione.

* [Estrai file](extract-file.md): esporta dati da Adobe Campaign in un altro sistema come file esterno.
* [Carica file](load-file.md): utilizzare profili e dati archiviati in un file esterno.
* [Trasferisci file](transfer-file.md): riceve o invia file, verifica la presenza di file o elenca file su un server. Il protocollo utilizzato può essere un protocollo da server a server o HTTP.
* [Codice JavaScript](javascript-code.md): esegui uno snippet di codice JavaScript nel contesto di un flusso di lavoro.
* [Servizi di abbonamento](subscription-services.md): consente di abbonare o annullare l&#39;abbonamento di più profili a o da un servizio in un&#39;unica azione.
* [Aggiorna dati](update-data.md): esegui aggiornamenti di massa sui campi del database. Diverse opzioni consentono di personalizzare l’aggiornamento dei dati.

## Attività di canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali. Combina le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che attivano azioni in base al comportamento del cliente. Sono disponibili le seguenti attività di **Canale**: e-mail, SMS, Android e notifiche push di iOS. [Scopri come impostare una consegna nel contesto di un flusso di lavoro](channels.md).

## Attività di controllo del flusso {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Attività Fine"
>abstract="L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa."

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

* [And-join](and-join.md): sincronizza più rami di esecuzione di un flusso di lavoro.
* **Fine**: contrassegna graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa.
* [Segnale esterno](external-signal.md): attiva l&#39;esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API.
* [Fork](fork.md): crea transizioni in uscita per avviare più attività contemporaneamente.
* [Modulo di pianificazione](scheduler.md): pianificazione all&#39;avvio del flusso di lavoro.
* [Test](test.md): abilita le transizioni in base alle condizioni specificate.
* [Attendi](wait.md): sospende temporaneamente l&#39;esecuzione di una parte di un flusso di lavoro.