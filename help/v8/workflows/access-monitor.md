---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: be7cdfbffbe5c3b1a7ec58e5c60856a6bdc56200
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 10%

---

# Accedere e gestire i flussi di lavoro {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flussi di lavoro"
>abstract="In questa schermata, puoi accedere all’elenco completo dei flussi di lavoro autonomi e dei flussi di lavoro delle campagne, verificarne lo stato corrente, le date dell’ultima/successiva esecuzione e creare un nuovo flusso di lavoro. Passa alla scheda “Modello” per accedere ai modelli di flusso di lavoro disponibili."

Il **[!UICONTROL Flussi di lavoro]** consente di accedere all’elenco completo dei flussi di lavoro. Questo elenco include entrambi **flussi di lavoro autonomi** che sono state create da questa schermata e **flussi di lavoro per campagne**, che sono state create all&#39;interno di una campagna.

![](assets/workflow-list.png)

Ogni flusso di lavoro dell&#39;elenco visualizza informazioni sul relativo [stato](#status), l’ultima volta che è stata eseguita o modificata e la successiva data e ora di esecuzione pianificata.

Puoi personalizzare le colonne visualizzate facendo clic sul pulsante **[!UICONTROL Configurare una colonna per un layout personalizzato]** nell&#39;angolo superiore destro dell&#39;elenco. Ciò ti consente di aggiungere ulteriori informazioni all’elenco, ad esempio l’ultima attività in errore per ogni flusso di lavoro o la dimensione di targeting applicata.

Inoltre, sono disponibili una barra di ricerca e dei filtri per facilitare la ricerca all’interno dell’elenco. Ad esempio, puoi filtrare i flussi di lavoro per visualizzare solo quelli appartenenti a una campagna o quelli elaborati durante un intervallo di date specifico.

Per duplicare o eliminare un flusso di lavoro, fai clic sul pulsante con i puntini di sospensione, quindi seleziona **[!UICONTROL Duplica]** o **[!UICONTROL Elimina]**.

>[!NOTE]
>
>È possibile duplicare un flusso di lavoro in corso, ma non eliminarlo.

## Stati dei flussi di lavoro {#status}

I flussi di lavoro possono avere più stati:

* **[!UICONTROL Bozza]**: il flusso di lavoro è stato creato e salvato.
* **[!UICONTROL In corso]**: il flusso di lavoro è attualmente in esecuzione.
* **[!UICONTROL Completato]**: esecuzione del flusso di lavoro completata.
* **[!UICONTROL In pausa]**: il flusso di lavoro è stato sospeso.
* **[!UICONTROL Errato]**: il flusso di lavoro ha rilevato un errore. Apri il flusso di lavoro e accedi ai registri e alle attività per identificare l’errore e risolverlo. [Scopri come monitorare registri e attività](start-monitor-workflows.md#logs-tasks)

Informazioni dettagliate su come avviare e monitorare l’esecuzione di un flusso di lavoro sono disponibili in [questa pagina](start-monitor-workflows.md).

## Modelli di flusso di lavoro {#templates}

Il **[!UICONTROL Modelli]** Questa scheda elenca tutti i modelli di workflow disponibili.

I modelli di flusso di lavoro contengono attività preconfigurate e configurazioni di proprietà generali che possono essere riutilizzate per creare nuovi flussi di lavoro. Vengono creati dalla console client. [Scopri come utilizzare i modelli](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
