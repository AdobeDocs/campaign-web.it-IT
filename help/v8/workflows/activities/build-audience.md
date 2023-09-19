---
audience: end-user
title: Utilizzare l’attività Crea pubblico nei flussi di lavoro
description: Scopri come utilizzare l’attività Crea pubblico nei flussi di lavoro
badge: label="Beta"
source-git-commit: 4028fabf0aca85ace97316b4e072c2b1dfa5dc5f
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 62%

---


# Crea pubblico {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Creare un’attività di pubblico"
>abstract="Il **Creare un pubblico** attività ti consente di definire il pubblico che entrerà nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro, il pubblico del messaggio non è definito nell’attività del canale, ma nel **Creare un pubblico** attività."


L’attività **Crea pubblico** è un’attività di **targeting**. Questa attività consente di definire il pubblico che sarà inserito nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro, il pubblico del messaggio non è definito nell’attività del canale, ma nel **Creare un pubblico** attività.

Per definire la popolazione del pubblico, puoi eseguire le seguenti operazioni:

* Seleziona un pubblico esistente, creato come elenco nella console client.
* Seleziona un pubblico di Adobe Experience Platform.
* Crea un nuovo pubblico con il generatore di regole definendo e combinando criteri di filtro.

>[!NOTE]
>
>In questo contesto, non è possibile caricare un pubblico da un file. A questo scopo, devi creare una consegna e-mail autonoma. [Ulteriori informazioni](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurare l’attività Genera pubblico

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Seleziona la dimensione di targeting"
>abstract="La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, iscritti, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari."


Per configurare l’attività **Crea pubblico**, segui questi passaggi:

1. Aggiungi un’attività **Crea pubblico**.
1. Definisci un’etichetta.
1. Definisci il tipo di pubblico: **Crea una query personalizzata** o **Leggi pubblico**.

Per creare una query personalizzata, segui questi passaggi aggiuntivi:

1. Seleziona **Crea una query personalizzata**.
1. Scegli la **Dimensione targeting**. La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, iscritti, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. Consulta la [documentazione di v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=it#targeting-and-filtering-dimensions){target="_blank"}.
1. Fai clic su **Continua**.
1. Utilizza il generatore di regole per definire la query, seguendo la stessa procedura con cu si crea un pubblico durante la progettazione di una nuova e-mail. Consulta questa [sezione](../../audience/segment-builder.md).

Per selezionare un pubblico esistente, segui questi passaggi:

1. Seleziona **Leggi pubblico**.
1. Fai clic su **Continua**.
1. Seleziona il pubblico seguendo la stessa procedura utilizzata per selezionare un pubblico durante la progettazione di una nuova e-mail. Consulta questa [sezione](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Se si desidera utilizzare una **[!UICONTROL Creare un pubblico]** attività che ha come target un pubblico di Experienci Platform, è necessario aggiungere una **[!UICONTROL Cambia dimensione]** per garantire che la dimensione di targeting del pubblico sia impostata su &quot;Destinatario&quot;. Nella parte inferiore di questa pagina è disponibile un esempio di flusso di lavoro.

## Esempi

Di seguito è riportato un esempio di un flusso di lavoro con due attività **Crea pubblico**. Il primo esegue il targeting di un pubblico di giocatori di poker, seguito da una consegna e-mail. Il secondo quello di un pubblico di clienti VIP, seguito da una consegna SMS.

![](../assets/workflow-audience-example.png)

Ecco un altro esempio di flusso di lavoro in cui un pubblico di Adobe Experience Platform viene combinato con un pubblico di Adobe Campaign. Per consentire la combinazione di questi tipi di pubblico, è necessario **[!UICONTROL Cambia dimensione]** L’attività con la dimensione di targeting &quot;Destinatario&quot; viene aggiunta dopo il pubblico di Adobe Experience Platform. [Scopri come configurare un’attività di modifica della dimensione](change-dimension.md)

![](../assets/workflow-audience-aep.png)
