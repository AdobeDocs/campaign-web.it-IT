---
title: Guardrail e limitazioni nei flussi di lavoro dell’interfaccia utente di Campaign Web
description: Guardrail e limitazioni nell’utilizzo dei flussi di lavoro nell’interfaccia utente web di Campaign
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '435'
ht-degree: 100%

---

# Guardrail e limitazioni per i flussi di lavoro {#guardrails-limitations}

Durante l’utilizzo deli flussi di lavoro creati o modificati nella console client di Campaign nell’interfaccia utente di Campaign Web, si applicano i guardrail e le limitazioni elencate di seguito.

Tieni presente che, anche se questa pagina identifica considerazioni chiave quando si lavora con i flussi di lavoro nella console e nell’interfaccia utente web, non include tutte le potenziali incompatibilità tra le due interfacce.

## Attività del flussi di lavoro {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Attività non modificabile"
>abstract="Quando un’attività di **Query** o **Arricchimento** è configurata con dati aggiuntivi nella console; i dati di arricchimento vengono presi in considerazione in Campaign Web e trasmessi nella transizione in uscita, ma non possono essere modificati."

Le attività dei flussi di lavoro non ancora supportate nell’interfaccia utente di Campaign Web sono di sola lettura e vengono visualizzate come attività non compatibili. Puoi eseguire comunque il flusso di lavoro, inviare messaggi, verificare i registri e svolgere altre attività. Le attività del flusso di lavoro che sono disponibili sia nell’interfaccia utente di Campaign Web che nella console client di Campaign sono modificabili.

| Console | Web |
| --- | --- |
| ![Schermata che mostra le limitazioni delle attività nella console](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Schermata che mostra le limitazioni delle attività nell’interfaccia web](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Quando un’attività di **Query** o **Arricchimento** è configurata con dati aggiuntivi nella console; i dati di arricchimento vengono presi in considerazione in Campaign Web e trasmessi nella transizione in uscita, ma non possono essere modificati.

| Console | Web |
| --- | --- |
| ![Schermata che mostra le limitazioni delle opzioni nella console](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Schermata che mostra le limitazioni delle opzioni nell’interfaccia web](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Nella console, l’attività **Arricchimento** può eseguire sia la riconciliazione che l’arricchimento. Se hai definito le impostazioni di riconciliazione nell’attività **Arricchimento** nella console client, questa verrà visualizzata come attività **Riconciliazione** nell’interfaccia utente di Campaign Web.

| Console | Web |
| --- | --- |
| ![Schermata che mostra l’attività Arricchimento nella console](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Schermata che mostra l’attività Arricchimento nell’interfaccia web](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Area di lavoro del flusso di lavoro {#wkf-canvas}

Quando crei un nuovo flusso di lavoro nell’interfaccia utente di Campaign Web, l’area di lavoro supporta un solo punto di ingresso. Tuttavia, se hai creato un flusso di lavoro nella console con più punti di ingresso, puoi aprirlo e modificarlo nell’interfaccia utente di Campaign Web.

| Console | Web |
| --- | --- |
| ![Schermata che mostra più punti di ingresso nella console](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Schermata che mostra più punti di ingresso nell’interfaccia web](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Il posizionamento dei nodi viene aggiornato ogni volta che si aggiunge o si rimuove un’attività. Se crei un flusso di lavoro nella console, lo modifichi utilizzando l’interfaccia utente di Campaign Web e quindi lo riapri nella console, potresti notare alcune lievi imperfezioni di posizionamento. Questo non ha alcun impatto sui processi e sulle attività del flusso di lavoro.

| Flusso di lavoro iniziale | Posizionamento modificato |
| --- | --- |
| ![Schermata che mostra il posizionamento iniziale del flusso di lavoro](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Schermata che mostra il posizionamento dopo le modifiche apportate](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |