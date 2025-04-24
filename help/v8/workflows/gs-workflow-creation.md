---
audience: end-user
title: Principi chiave per la creazione di flussi di lavoro
description: Scopri i principi chiave dei flussi di lavoro con Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# Principi chiave per la creazione di flussi di lavoro {#gs-workflow-creation}

Con Adobe Campaign Web, è possibile creare flussi di lavoro in un’area di lavoro visiva per progettare processi cross-channel come la segmentazione, l’esecuzione di campagne e l’elaborazione di file.

## Che cosa c’è all’interno di un flusso di lavoro? {#gs-workflow-inside}

Il diagramma del flusso di lavoro rappresenta il processo pianificato. Descrive le varie attività da eseguire e il modo in cui vengono collegate tra loro.

![Diagramma di esempio del flusso di lavoro che mostra le attività e le relative connessioni](assets/workflow-example.png){zoomable="yes"}

Ogni flusso di lavoro contiene:

* **Attività**: un’attività è un’attività da eseguire. Le icone nel diagramma rappresentano le varie attività. Ogni attività presenta proprietà specifiche e altre proprietà comuni a tutte le attività.

  In un diagramma del flusso di lavoro, una determinata attività può produrre più attività, in particolare in presenza di un ciclo o di azioni ricorrenti.

* **Transizioni**: le transizioni collegano un’attività di origine a un’attività di destinazione e ne definiscono la sequenza.

* **Tabelle di lavoro**: la tabella di lavoro contiene tutte le informazioni riportate dalla transizione. Ogni flusso di lavoro utilizza diverse tabelle di lavoro. I dati presenti in queste tabelle possono essere utilizzati in tutto il ciclo di vita del flusso di lavoro.

## Passaggi chiave per creare un flusso di lavoro {#gs-workflow-steps}

Campaign offre due modi per creare un flusso di lavoro:

1. I flussi di lavoro possono essere creati come flussi di lavoro autonomi dal menu **Flussi di lavoro**.

   ![Schermata dell’interfaccia per la creazione di un flusso di lavoro autonomo](assets/create-a-standalone-wf.png){zoomable="yes"}

1. I flussi di lavoro possono essere creati direttamente all’interno di una campagna, dalla scheda **Flusso di lavoro** della campagna. Quando è incluso in una campagna, il flusso di lavoro viene eseguito insieme a tutti gli altri flussi di lavoro della campagna e le metriche di reporting sono raggruppate a livello di campagna.

   ![Schermata dell’interfaccia per la creazione di un flusso di lavoro all’interno di una campagna](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

I passaggi chiave per creare i flussi di lavoro sono i seguenti:

![Diagramma che mostra il processo di creazione del flusso di lavoro](assets/workflow-creation-process.png){zoomable="yes"}

Questi passaggi sono descritti nelle sezioni seguente:

1. [Creare il flusso di lavoro e definirne le proprietà](create-workflow.md)
1. [Orchestrare e configurare le attività](orchestrate-activities.md)
1. [Configurare le impostazioni avanzate del flusso di lavoro](workflow-settings.md)
1. [Avviare il flusso di lavoro e monitorarne l’esecuzione](start-monitor-workflows.md)