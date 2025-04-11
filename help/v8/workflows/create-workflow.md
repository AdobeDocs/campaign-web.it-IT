---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare un flusso di lavoro con Adobe Campaign Web
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 70%

---

# Creare il flusso di lavoro {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Elenco dei flussi di lavoro nella campagna"
>abstract="Nella scheda **Flussi di lavoro** sono elencati tutti i flussi di lavoro collegati alla campagna. Fai clic sul nome di un flusso di lavoro per modificarlo. Utilizza il pulsante **Crea flusso di lavoro** per aggiungere un nuovo flusso di lavoro per questa campagna."

Puoi creare flussi di lavoro autonomi o flussi di lavoro all’interno di una campagna. Il primo passaggio consiste nel selezionare un modello e definirne le proprietà generali. Puoi quindi configurare altre impostazioni in base alle esigenze.

Per farlo, segui questi passaggi:

1. Per creare un **flusso di lavoro autonomo**, passare al menu **Flussi di lavoro**. Per creare un **Flusso di lavoro della campagna**, passa al menu **Campagne** e apri la campagna per la quale desideri creare un nuovo flusso di lavoro.

1. Fai clic sul pulsante **[!UICONTROL Crea flusso di lavoro]** nell’angolo in alto a destra della schermata.

   ![Schermata che mostra il pulsante Crea flusso di lavoro nell&#39;angolo superiore destro dello schermo.](assets/workflow-create.png){zoomable="yes"}

1. Nella finestra di dialogo **Proprietà** del flusso di lavoro, seleziona il modello da utilizzare per creare il flusso di lavoro (puoi anche utilizzare il modello predefinito). [Ulteriori informazioni sui modelli di workflow](#workflow-templates).

1. Immetti un’etichetta per il flusso di lavoro. Aggiungi inoltre una descrizione al flusso di lavoro nel campo dedicato della sezione **[!UICONTROL Opzioni aggiuntive]** della schermata.

1. Espandi la sezione **[!UICONTROL Opzioni aggiuntive]** per configurare altre impostazioni per il flusso di lavoro. Scopri come configurare le proprietà del flusso di lavoro in [questa pagina](workflow-settings.md#properties).

   ![Schermata che mostra la sezione Opzioni aggiuntive per la configurazione delle impostazioni del flusso di lavoro.](assets/workflow-additional-options.png){zoomable="yes"}

1. Fai clic sul pulsante **[!UICONTROL Crea flusso di lavoro]** per confermare la creazione del flusso di lavoro.

Il flusso di lavoro viene ora creato e disponibile nell’elenco dei flussi di lavoro. Puoi accedere alla relativa area di lavoro visiva e iniziare ad aggiungere, configurare e orchestrare le attività che eseguirà. [Scopri come orchestrare le attività del flusso di lavoro](orchestrate-activities.md).

## Utilizzare i modelli di flusso di lavoro {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Modelli di flusso di lavoro"
>abstract="I modelli di flusso di lavoro contengono impostazioni e attività preconfigurate che possono essere riutilizzate per creare nuovi flussi di lavoro."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Proprietà del flusso di lavoro"
>abstract="I modelli di flusso di lavoro contengono impostazioni e attività preconfigurate che possono essere riutilizzate per creare nuovi flussi di lavoro. In questa schermata, immetti l’etichetta del modello di flusso di lavoro e configurane le impostazioni, ad esempio il nome interno, la cartella e le cartelle di esecuzione, il fuso orario e il gruppo di supervisione."

I modelli di flusso di lavoro contengono impostazioni e attività preconfigurate che possono essere riutilizzate per creare nuovi flussi di lavoro. Seleziona il modello del flusso di lavoro dalle proprietà del flusso di lavoro al momento della creazione. Per impostazione predefinita, viene fornito un modello vuoto.

Puoi creare un modello da un flusso di lavoro esistente o crearne uno nuovo da zero. Entrambi i metodi sono descritti di seguito.

>[!BEGINTABS]

>[!TAB Creare un modello da un flusso di lavoro esistente]

Per creare un modello da un flusso di lavoro esistente, segui questi passaggi:

1. Apri il menu **Flussi di lavoro** e passa al flusso di lavoro per salvarlo come modello.
1. Fai clic sui tre punti a destra del nome del flusso di lavoro e scegli **Copia come modello**.

   ![Schermata che mostra l&#39;opzione Copia come modello nel menu del flusso di lavoro.](assets/wf-copy-as-template.png){zoomable="yes"}

1. Conferma la creazione del modello nella finestra a comparsa.
1. Nell’area di lavoro del modello del flusso di lavoro, seleziona, aggiungi e configura le attività in base alle esigenze.
1. Accedi alle impostazioni dal pulsante **Impostazioni** per modificare il nome del modello del flusso di lavoro e immettere una descrizione.
1. Seleziona la **cartella** e la **cartella di esecuzione** del modello. La cartella è la posizione in cui viene salvato il modello del flusso di lavoro. La cartella di esecuzione è la cartella in cui vengono salvati i flussi di lavoro creati in base a questo modello.

   ![Schermata che mostra le impostazioni per la cartella e la cartella di esecuzione nel modello di flusso di lavoro.](assets/wf-settings-template.png){zoomable="yes"}

   Le altre proprietà sono comuni ai flussi di lavoro. Per ulteriori informazioni, consulta [questa pagina](workflow-settings.md#properties).

1. Salva le modifiche.

Il modello del flusso di lavoro è ora disponibile nell’elenco dei modelli. Puoi creare un flusso di lavoro basato su questo modello. Questo flusso di lavoro sarà preconfigurato con le impostazioni e le attività definite nel modello.

>[!TAB Creare un modello da zero]

Per creare un modello di flusso di lavoro da zero, segui questi passaggi:

1. Apri il menu **Flussi di lavoro** e passa alla scheda **Modelli**. Puoi visualizzare l’elenco dei modelli di flusso di lavoro disponibili.
1. Fai clic sul pulsante **[!UICONTROL Crea modello]** nell’angolo in altro a destra della schermata.
1. Immetti l’etichetta e apri le opzioni aggiuntive per immettere una descrizione del modello del flusso di lavoro.
1. Seleziona la cartella e la cartella di esecuzione del modello. La cartella è la posizione in cui viene salvato il modello del flusso di lavoro. La cartella di esecuzione è la cartella in cui vengono salvati i flussi di lavoro creati in base a questo modello.

   ![Schermata che mostra la creazione di un nuovo modello di flusso di lavoro con le impostazioni della cartella e della cartella di esecuzione.](assets/new-wf-template.png){zoomable="yes"}

   Le altre proprietà sono comuni ai flussi di lavoro. Per ulteriori informazioni, consulta [questa pagina](workflow-settings.md#properties).

1. Fai clic sul pulsante **Crea** per confermare le impostazioni.
1. Nell’area di lavoro del modello di flusso di lavoro, aggiungi e configura le attività in base alle esigenze.

   ![Schermata che mostra l&#39;area di lavoro del modello di flusso di lavoro per l&#39;aggiunta e la configurazione delle attività.](assets/wf-template-activities.png){zoomable="yes"}

1. Salva le modifiche.

Il modello del flusso di lavoro è ora disponibile nell’elenco dei modelli. Puoi creare un flusso di lavoro basato su questo modello. Questo flusso di lavoro sarà preconfigurato con le impostazioni e le attività definite nel modello.

>[!ENDTABS]