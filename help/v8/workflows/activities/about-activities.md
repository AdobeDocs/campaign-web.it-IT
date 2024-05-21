---
audience: end-user
title: Utilizzare le attività dei flussi di lavoro
description: Scopri come utilizzare le attività dei flussi di lavoro
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 32%

---


# Informazioni sulle attività dei flussi di lavoro {#workflow-activities}

Le attività dei flussi di lavoro sono raggruppate in tre categorie. A seconda del contesto, le attività disponibili possono variare.

Tutte le attività sono descritte nelle sezioni seguenti:

* [Attività di targeting e gestione dei dati](#targeting)
* [Attività di canale](#channel)
* [Attività di controllo del flusso](#flow-control)

![](../assets/workflow-activities.png)

## Attività di targeting {#targeting}

Queste attività sono specifiche per il targeting. Consentono di creare uno o più target definendo un pubblico e suddividendo o combinando i tipi di pubblico mediante le operazioni di intersezione, unione o esclusione.

* [Creare un pubblico](build-audience.md): definisci la popolazione target. Puoi selezionare un pubblico esistente o utilizzare il modellatore di query per definire una query personalizzata.
* [Cambia origine dati](change-data-source.md): modifica l’origine dati per la tabella di lavoro del flusso di lavoro.&quot;
* [Cambia dimensione](change-dimension.md): modifica la dimensione di targeting durante la creazione del flusso di lavoro.
* [Combina](combine.md): esegui la segmentazione sulla popolazione in entrata. Puoi utilizzare un’unione, un’intersezione o un’esclusione.
* [Deduplicazione](deduplication.md): elimina i duplicati nei risultati delle attività in entrata.
* [Arricchimento](enrichment.md): definisci i dati aggiuntivi da elaborare nel flusso di lavoro. Questa attività consente di sfruttare la transizione in entrata e può essere configurata in modo da completare la transizione in uscita con dati aggiuntivi.
* [Query incrementale](incremental-query.md): esegui una query sul database in base a una pianificazione. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi.
* [Reconciliation](reconciliation.md): definisci il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro, ad esempio i dati caricati da un file esterno.
* [Salva pubblico](save-audience.md): aggiorna un pubblico esistente o creane uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro.
* [Dividi](split.md): segmenta la popolazione in ingresso in diversi sottoinsiemi.

## Attività di gestione dati {#data}

Queste attività sono specifiche per la manipolazione e l’arricchimento dei dati sulla popolazione.

* [Extract file](extract-file.md): esporta dati da Adobe Campaign a un altro sistema come file esterno.
* [Carica file](load-file.md): utilizza profili e dati memorizzati in un file esterno.
* [Trasferisci file](transfer-file.md): ricezione o invio di file, verifica della presenza di file o elenco di file su un server. Il protocollo utilizzato può essere un protocollo da server a server o HTTP.
* [Codice JavaScript](javascript-code.md): esegui uno snippet di codice JavaScript nel contesto di un flusso di lavoro.
* [Servizi di abbonamento](subscription-services.md): possibilità di abbonare o annullare l’abbonamento di più profili a/da un servizio in una singola azione.
* [Aggiorna dati](update-data.md): esegui aggiornamenti di massa sui campi del database. Diverse opzioni consentono di personalizzare l’aggiornamento dei dati.

## Attività di canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali. Puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento del cliente. I seguenti elementi **Canale** Le attività sono disponibili: e-mail, SMS, Android e notifiche push iOS. [Scopri come impostare una consegna nel contesto di un flusso di lavoro](channels.md).

## Attività di controllo del flusso {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Attività Fine"
>abstract="L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa."

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

* [And-join](and-join.md): sincronizza più rami di esecuzione di un flusso di lavoro.
* **Fine**: contrassegna graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa
* [Segnale esterno](external-signal.md): attiva l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API.
* [Fork](fork.md): crea transizioni in uscita per avviare più attività in contemporanea.
* [Scheduler](scheduler.md): pianifica l’avvio del flusso di lavoro.
* [Test](test.md): abilita le transizioni in base a condizioni specificate.
* [Wait](wait.md): sospende temporaneamente l’esecuzione di una parte di un flusso di lavoro.
