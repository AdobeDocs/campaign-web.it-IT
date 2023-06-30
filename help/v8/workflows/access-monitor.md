---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '364'
ht-degree: 100%

---

# Accedere e gestire i flussi di lavoro {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flussi di lavoro"
>abstract="In questa schermata, puoi accedere all’elenco completo dei flussi di lavoro autonomi e della campagna, controllarne lo stato, le date dell’ultima/successiva esecuzione e creare un nuovo flusso di lavoro. Passa alla scheda “Modello” per accedere ai modelli di flusso di lavoro disponibili."

Il menu **[!UICONTROL Flussi di lavoro]** consente di accedere all’elenco completo dei flussi di lavoro. Questo elenco include sia i **flussi di lavoro autonomi** che sono stati creati da questa schermata sia i **flussi di lavoro della campagna**, che sono stati creati all’interno di una campagna.

![](assets/workflow-list.png)

Ogni flusso di lavoro dell’elenco mostra informazioni sul relativo [stato](#status), l’ultima volta che è stato eseguito o modificato e la data e ora di esecuzione successiva pianificata.

Puoi personalizzare le colonne visualizzate facendo clic sull’icona **[!UICONTROL Configura una colonna per un layout personalizzato]** nell’angolo superiore a destra dell&#39;elenco. Ciò ti consente di aggiungere ulteriori informazioni all’elenco, ad esempio l’ultima attività in errore per ogni flusso di lavoro o la dimensione di targeting applicata.

Inoltre, sono disponibili una barra di ricerca e dei filtri per facilitare la ricerca all’interno dell’elenco. Ad esempio, puoi filtrare i flussi di lavoro per visualizzare solo quelli appartenenti a una campagna o quelli elaborati durante un intervallo di date specifico.

Per duplicare o eliminare un flusso di lavoro, fai clic sul pulsante con i puntini di sospensione, quindi seleziona **[!UICONTROL Duplica]** o **[!UICONTROL Elimina]**.

>[!NOTE]
>
>È possibile duplicare un flusso di lavoro in corso, ma non eliminarlo.

## Stati dei flussi di lavoro {#status}

I flussi di lavoro possono avere più stati:

* **[!UICONTROL Bozza]**: il flusso di lavoro è stato creato e salvato.
* **[!UICONTROL In corso]**: il flusso di lavoro è attualmente in esecuzione.
* **[!UICONTROL Completato]**: l’esecuzione del flusso di lavoro è stata completata.
* **[!UICONTROL In pausa]**: il flusso di lavoro è stato messo in pausa.
* **[!UICONTROL Errato]**: il flusso di lavoro ha riscontrato un errore. Apri il flusso di lavoro e accedi ai registri e alle attività per identificare l’errore e risolverlo. [Scopri come monitorare i registri e le attività](start-monitor-workflows.md#logs-tasks)

Informazioni dettagliate su come avviare e monitorare l’esecuzione di un flusso di lavoro sono disponibili in [questa pagina](start-monitor-workflows.md).

## Modelli di flusso di lavoro {#templates}

Nella scheda **[!UICONTROL Modelli]** sono elencati tutti i modelli di flusso di lavoro disponibili.

I modelli di flusso di lavoro contengono attività preconfigurate e configurazioni di proprietà generali che possono essere riutilizzate per creare nuovi flussi di lavoro. Vengono creati dalla console client. [Scopri come utilizzare i modelli](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html?lang=it#workflow-templates)
