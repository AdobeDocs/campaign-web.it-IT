---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 422f2d2cbef424a95540f359c4a5e978eace6c9f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 7%

---


# Orchestrare le attività {#orchestrate}

Una volta che hai [ha creato un flusso di lavoro](create-workflow.md), dal menu del flusso di lavoro o all’interno di una campagna, puoi iniziare a orchestrare le diverse attività che eseguirà. A questo scopo, viene fornita un’area di lavoro visiva che consente di creare un diagramma di flusso di lavoro. All’interno di questo diagramma, puoi aggiungere varie attività e collegarle in ordine sequenziale.

In questa fase della configurazione, il diagramma viene visualizzato con un’icona iniziale che rappresenta l’inizio del flusso di lavoro. Per aggiungere la prima attività, fai clic sul pulsante + collegato all’icona Start.

Viene visualizzato un elenco di attività che possono essere aggiunte al diagramma. Le attività disponibili dipendono dalla posizione all’interno del diagramma del flusso di lavoro. Ad esempio, quando aggiungi la prima attività, puoi avviare il flusso di lavoro eseguendo il targeting di un pubblico, suddividendo il percorso del flusso di lavoro o impostando un’attività Attendi per ritardare l’esecuzione del flusso di lavoro. D’altra parte, dopo un’attività Genera pubblico, puoi perfezionare il target con le attività di targeting, inviare una consegna al pubblico con le attività del canale o organizzare il processo di flusso di lavoro con le attività di controllo del flusso.

![](assets/workflow-start.png)

Una volta aggiunta un’attività al diagramma, viene visualizzato un riquadro a destra che consente di configurare l’attività appena aggiunta con impostazioni specifiche. Informazioni dettagliate su come configurare ogni attività sono disponibili in [questa sezione](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Ripeti questo processo aggiungendo tutte le attività desiderate in base alle attività che desideri che il flusso di lavoro esegua. Puoi anche inserire una nuova attività tra due attività. A questo scopo, fai clic sul pulsante + sulla transizione tra le attività, seleziona l’attività desiderata e configurala nel riquadro a destra.

Per rimuovere un’attività, selezionala nell’area di lavoro e fai clic sull’icona Elimina nelle proprietà dell’attività.

>[!TIP]
>
>Hai la possibilità di personalizzare il nome delle transizioni tra ciascuna attività. A questo scopo, seleziona la transizione e modifica la relativa etichetta nel riquadro a destra.

Dopo aver completato il flusso di lavoro, aggiungi un’attività Fine alla fine del diagramma. Questa attività ti consente di contrassegnare visivamente la fine di un flusso di lavoro e non ha alcun impatto funzionale.

Dopo aver progettato correttamente il diagramma del flusso di lavoro, è possibile eseguirlo e tenere traccia dell&#39;avanzamento delle varie attività. [Scopri come avviare un flusso di lavoro e monitorarne l’esecuzione](start-monitor-workflows.md)