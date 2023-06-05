---
audience: end-user
title: Utilizzare le attività di dei flussi di lavoro
description: Scopri come eseguire le attività del flusso di lavoro
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 07da5f804e25382c6202b7438e15dafaee413f27
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 8%

---


# Informazioni sulle attività del flusso di lavoro {#workflow-activities}

Le attività del flusso di lavoro sono raggruppate in tre categorie. A seconda del contesto, le attività disponibili possono variare.

Tutte le attività sono descritte nelle sezioni seguenti:

* [Attività di targeting](#targeting)
* [Attività del canale](#channel)
* [Attività di controllo del flusso](#flow-control)

![](../assets/workflow-activities.png)

## Attività di targeting {#targeting}

Queste attività sono specifiche per il targeting, la manipolazione e l’arricchimento dei dati sulla popolazione. Consentono di creare uno o più target definendo un pubblico e suddividendo o combinando questi tipi di pubblico tramite operazioni di intersezione, unione o esclusione.

* Il [Creare un pubblico](build-audience.md) attività ti consente di definire la popolazione target. Puoi selezionare un pubblico esistente o utilizzare il generatore di regole per definire una query personalizzata.
* Il [Combina](combine.md) l’attività ti consente di eseguire la segmentazione sulla popolazione in entrata. Puoi utilizzare un’unione, un’intersezione o un’esclusione.
* Il [Arricchimento](enrichment.md) attività ti consente di definire i dati aggiuntivi da elaborare nel flusso di lavoro. Con questa attività, puoi sfruttare la transizione in entrata e configurare l’attività in modo da completare la transizione in uscita con l’inserimento di dati aggiuntivi.

## Attività del canale {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su più canali, ad esempio e-mail, SMS o push. Puoi combinare le attività dei canali nell’area di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento del cliente.

I seguenti elementi **Canale** Le attività sono disponibili:

* [E-mail](email.md)
* [Push](push.md)
* [SMS](sms.md)

## Attività di controllo del flusso {#flow-control}

Le seguenti attività sono specifiche per l’organizzazione e l’esecuzione dei flussi di lavoro. Il loro compito principale è quello di coordinare le altre attività:

* Il [And-join](and-join.md) attività consente di sincronizzare più rami di esecuzione di un flusso di lavoro.
* Il [Fine](end.md) attività consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività non ha alcun impatto funzionale ed è pertanto facoltativa.
* Il [Fork](fork.md) attività consente di creare transizioni in uscita per avviare più attività in contemporanea.
* Il [Wait](wait.md) l’attività sospende momentaneamente l’esecuzione di una parte di un flusso di lavoro.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

