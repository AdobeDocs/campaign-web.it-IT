---
audience: end-user
title: Utilizzare le attività dei flussi di lavoro
description: Scopri come utilizzare le attività dei flussi di lavoro
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 100%

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

* L’attività [Creazione del pubblico](build-audience.md) consente di definire la popolazione target. Puoi selezionare un pubblico esistente o utilizzare il generatore di regole per definire una query personalizzata.
* L’attività [Combina](combine.md) consente di eseguire la segmentazione sulla popolazione in entrata. Puoi utilizzare un’unione, un’intersezione o un’esclusione.
* L’attività [Arricchimento](enrichment.md) consente di definire i dati aggiuntivi da elaborare nel flusso di lavoro. Questa attività consente di sfruttare la transizione in entrata e può essere configurata in modo da completare la transizione in uscita con dati aggiuntivi.
* L’attività [Dividi](split.md) ti consente di segmentare la popolazione in ingresso in diversi sottoinsiemi.

## Attività di canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali, come e-mail, SMS o push. Puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento dei clienti.

Sono disponibili le seguenti attività **Canale**:

* E-mail
* Push
* SMS

Consulta questa [sezione](enrichment.md).

## Attività di controllo del flusso {#flow-control}

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

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

