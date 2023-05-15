---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: ht
source-wordcount: '286'
ht-degree: 100%

---


# Principi chiave per la creazione di flussi di lavoro {#gs-workflow-creation}

Con Campaign v8 Web, puoi creare flussi di lavoro in un’area di lavoro visiva per progettare processi cross-channel come la segmentazione, l’esecuzione di campagne e l’elaborazione di file.

I flussi di lavoro possono essere creati come flussi di lavoro autonomi, dal menu Flussi di lavoro o dall’interno di una campagna, dal menu Campagne.

TBD: specificità dei flussi di lavoro autonomi e di campagna.

## Cosa c’è all’nterno di un flusso di lavoro?

Il diagramma del flusso di lavoro è una rappresentazione di ciò che dovrebbe accadere. Descrive le varie attività da eseguire e il modo in cui vengono collegate tra loro.

Ogni flusso di lavoro contiene:

* **Attività**: un’attività è un’attività da eseguire. Le varie attività disponibili sono rappresentate nel diagramma tramite icone. Ogni attività presenta proprietà specifiche e altre proprietà comuni a tutte le attività.

   In un diagramma del flusso di lavoro, una determinata attività può produrre più attività, in particolare in presenza di un ciclo o di azioni ricorrenti.

* **Transizioni**: le transizioni collegano un’attività di origine a un’attività di destinazione e ne definiscono la sequenza.

* **Tabelle di lavoro**: la tabella di lavoro contiene tutte le informazioni riportate dalla transizione. Ogni flusso di lavoro utilizza diverse tabelle di lavoro. I dati trasmessi in queste tabelle possono essere accelerati e utilizzati per l’intero ciclo di vita del flusso di lavoro, purché non vengano eliminati. In effetti, le tabelle non necessarie vengono eliminate ogni volta che il flusso di lavoro viene passivato e possibilmente durante l’esecuzione dei flussi di lavoro più grandi per evitare di sovraccaricare il server.

## Passaggi principali per creare un flusso di lavoro

I passaggi principali per creare i flussi di lavoro sono i seguenti:

TBD: grafico che mostra l’intero processo con spiegazione e riferimento alle pagine della documentazione

Creare e definire le proprietà > Orchestrare le attività nell’area di lavoro > Configurare le impostazioni se necessario > Avviare l’esecuzione e monitorare