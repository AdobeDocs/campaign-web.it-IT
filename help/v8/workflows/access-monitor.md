---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 46%

---

# Accedere e gestire i flussi di lavoro {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flussi di lavoro"
>abstract="In questa schermata, puoi accedere all’elenco completo dei flussi di lavoro autonomi e della campagna, controllarne lo stato, le date dell’ultima/successiva esecuzione e creare un nuovo flusso di lavoro. Passa alla scheda “Modelli” per accedere ai modelli di flusso di lavoro disponibili."

Il menu **[!UICONTROL Flussi di lavoro]** consente di accedere all&#39;elenco completo dei flussi di lavoro. Questo elenco include sia **flussi di lavoro autonomi**, creati da questa schermata, sia **flussi di lavoro campagne**, creati all&#39;interno di una campagna.

![Schermata dell&#39;elenco dei flussi di lavoro che mostra i flussi di lavoro autonomi e delle campagne](assets/workflow-list.png){zoomable="yes"}

Ogni flusso di lavoro dell’elenco mostra informazioni sul relativo [stato](#status), l’ultima volta che è stato eseguito o modificato e la data e ora di esecuzione successiva pianificata.

Personalizzare le colonne visualizzate facendo clic sulla colonna **[!UICONTROL Configura per un layout personalizzato]** nell&#39;angolo superiore destro dell&#39;elenco. Ciò ti consente di aggiungere ulteriori informazioni all’elenco, ad esempio l’ultima attività in errore per ogni flusso di lavoro o la dimensione di targeting applicata.

Inoltre, sono disponibili una barra di ricerca e dei filtri per semplificare la ricerca all’interno dell’elenco. Ad esempio, filtra i flussi di lavoro per visualizzare solo quelli appartenenti a una campagna o quelli elaborati durante un intervallo di date specifico.

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

Informazioni dettagliate su come avviare e monitorare l&#39;esecuzione di un flusso di lavoro sono disponibili in [questa pagina](start-monitor-workflows.md).

## Modelli di flusso di lavoro {#templates}

Nella scheda **[!UICONTROL Modelli]** sono elencati tutti i modelli di flusso di lavoro disponibili.

I modelli di flusso di lavoro contengono attività preconfigurate e configurazioni di proprietà generali che possono essere riutilizzate per creare nuovi flussi di lavoro.

Crea modelli di flusso di lavoro da un flusso di lavoro esistente o da zero. [Scopri come creare modelli di flusso di lavoro](create-workflow.md#workflow-templates)