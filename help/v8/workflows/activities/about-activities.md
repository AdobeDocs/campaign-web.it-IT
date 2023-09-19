---
audience: end-user
title: Utilizzare le attività dei flussi di lavoro
description: Scopri come utilizzare le attività dei flussi di lavoro
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: a8b73ba5664eedf473f09050602a61895993663e
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 83%

---


# Informazioni sulle attività dei flussi di lavoro {#workflow-activities}

Le attività dei flussi di lavoro sono raggruppate in tre categorie. A seconda del contesto, le attività disponibili possono variare.

Tutte le attività sono descritte nelle sezioni seguenti:

* [Attività di targeting](#targeting)
* [Attività di canale](#channel)
* [Attività di controllo del flusso](#flow-control)

![](../assets/workflow-activities.png)

## Attività di targeting {#targeting}

Queste attività sono specifiche per il targeting, la gestione e l’arricchimento dei dati sulla popolazione. Consentono di creare uno o più target definendo un pubblico e suddividendo o combinando i tipi di pubblico mediante le operazioni di intersezione, unione o esclusione.

* Il [Salva pubblico](save-audience.md) attività ti consente di aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro.
* L’attività [Creazione del pubblico](build-audience.md) consente di definire la popolazione target. Puoi selezionare un pubblico esistente o utilizzare il generatore di regole per definire una query personalizzata.
* L’attività [Combina](combine.md) consente di eseguire la segmentazione sulla popolazione in entrata. Puoi utilizzare un’unione, un’intersezione o un’esclusione.
* L’attività [Dividi](split.md) ti consente di segmentare la popolazione in ingresso in diversi sottoinsiemi.
* L’attività [Arricchimento](enrichment.md) consente di definire i dati aggiuntivi da elaborare nel flusso di lavoro. Questa attività consente di sfruttare la transizione in entrata e può essere configurata in modo da completare la transizione in uscita con dati aggiuntivi.
* Il [Deduplicazione](deduplication.md) attività ti consente di eliminare i duplicati nei risultati delle attività in entrata.
* Il [Cambia dimensione](change-dimension.md) attività ti consente di modificare la dimensione di targeting durante la creazione del flusso di lavoro.

## Attività di canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali, come e-mail, SMS o push. Puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento dei clienti.

Sono disponibili le seguenti attività **Canale**:

* E-mail
* Push
* SMS

Consulta questa [sezione](channels.md).

## Attività di controllo del flusso {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Attività fine"
>abstract="L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa."

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

* Il [Scheduler](scheduler.md) attività ti consente di pianificare quando viene avviato il flusso di lavoro.
* L’attività [Unione AND](and-join.md) consente di sincronizzare più rami di esecuzione di un flusso di lavoro.
* L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa.
* L’attività [Fork](fork.md) consente di creare transizioni in uscita per avviare più attività contemporaneamente.
* L’attività [Attendi](wait.md) sospende momentaneamente l’esecuzione di una parte di un flusso di lavoro.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

