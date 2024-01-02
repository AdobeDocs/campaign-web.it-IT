---
audience: end-user
title: Utilizzare le attività dei flussi di lavoro
description: Scopri come utilizzare le attività dei flussi di lavoro
badge: label="Disponibilità limitata"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 1336690b8abe4c3697341ee1d1d704f21f7ece20
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 39%

---


# Informazioni sulle attività dei flussi di lavoro {#workflow-activities}

Le attività dei flussi di lavoro sono raggruppate in tre categorie. A seconda del contesto, le attività disponibili possono variare.

Tutte le attività sono descritte nelle sezioni seguenti:

* [Attività di targeting e gestione dei dati](#targeting)
* [Attività di canale](#channel)
* [Attività di controllo del flusso](#flow-control)

![](../assets/workflow-activities.png)

## Attività di targeting e gestione dei dati {#targeting}

Queste attività sono specifiche per il targeting, la gestione e l’arricchimento dei dati sulla popolazione. Consentono di creare uno o più target definendo un pubblico e suddividendo o combinando i tipi di pubblico mediante le operazioni di intersezione, unione o esclusione.

* Utilizza il [Salva pubblico](save-audience.md) attività per aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro.
* Utilizza il [Creare un pubblico](build-audience.md) per definire la popolazione target. Puoi selezionare un pubblico esistente o utilizzare il generatore di regole per definire una query personalizzata.
* Utilizza il [Combina](combine.md) attività per eseguire la segmentazione sulla popolazione in entrata. Puoi utilizzare un’unione, un’intersezione o un’esclusione.
* Utilizza il [Dividi](split.md) attività per segmentare la popolazione in ingresso in diversi sottoinsiemi.
* Utilizza il [Reconciliation](reconciliation.md) attività per definire il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro, ad esempio i dati caricati da un file esterno.
* Utilizza il [Arricchimento](enrichment.md) per definire i dati aggiuntivi da elaborare nel flusso di lavoro. Questa attività consente di sfruttare la transizione in entrata e può essere configurata in modo da completare la transizione in uscita con dati aggiuntivi.
* Utilizza il [Deduplicazione](deduplication.md) attività per eliminare i duplicati nei risultati delle attività in entrata.
* Utilizza il [Cambia dimensione](change-dimension.md) attività per modificare la dimensione di targeting durante la creazione del flusso di lavoro.
* Utilizza il [Carica file](load-file.md) per lavorare con profili e dati memorizzati in un file esterno.


## Attività di canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali. Puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento del cliente. I seguenti elementi **Canale** Le attività sono disponibili: e-mail, SMS, Android e notifiche push iOS.

Scopri come impostare una consegna nel contesto di un flusso di lavoro in questo [sezione](channels.md).

## Attività di controllo del flusso {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Attività Fine"
>abstract="L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa."

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

* Utilizza il [Scheduler](scheduler.md) attività da pianificare all’avvio del flusso di lavoro.
* Utilizza il [And-join](and-join.md) attività per sincronizzare più rami di esecuzione di un flusso di lavoro.
* Aggiungi un **Fine** per contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa.
* Utilizza il [Fork](fork.md) attività per creare transizioni in uscita e avviare più attività contemporaneamente.
* Aggiungi un [Wait](wait.md) attività per mettere momentaneamente in pausa l’esecuzione di una parte di un flusso di lavoro.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

