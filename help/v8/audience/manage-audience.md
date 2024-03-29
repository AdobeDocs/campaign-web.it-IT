---
audience: end-user
title: Monitorare e gestire tipi di pubblico
description: Scopri come monitorare e gestire i tipi di pubblico in Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 86%

---

# Monitorare e gestire tipi di pubblico {#monitor-manage}

## Cos’è un pubblico? {#what}

Il pubblico è il target principale della consegna: i profili che ricevono i messaggi. Il tipo di pubblico dipende dalla mappatura target definita nel modello di consegna. Ulteriori informazioni sui modelli di consegna sono disponibili in [questa pagina](../msg/delivery-template.md).

Per definire la popolazione di un pubblico, puoi:

* [Creare nuovi tipi di pubblico](create-audience.md) dal menu **[!UICONTROL Tipi di pubblico]**
* [Selezionare un pubblico esistente](add-audience.md) creato come elenco nella console client o proveniente da Adobe Experience Platform
* [Creare un nuovo pubblico](../query/query-modeler-overview.md) con Query Modeler definendo e combinando criteri di filtraggio,
* [Utilizzare un pubblico da un file esterno](file-audience.md); questa opzione è disponibile solo per le consegne e-mail autonome e non può essere utilizzata nelle consegne delle campagne.

Nel targeting di un pubblico, puoi definire dei **gruppi di controllo** per evitare di inviare messaggi a una parte del pubblico, in modo da misurare l’impatto delle campagne. [Scopri come impostare un gruppo di controllo](control-group.md)

>[!NOTE]
>
>Quando si inviano messaggi nel contesto del flusso di lavoro di una campagna, il pubblico viene definito in una specifica attività **Crea pubblico** del flusso di lavoro. In questo contesto, non puoi caricare un pubblico da un file per una consegna e-mail e il pubblico è definito solo in questa attività dedicata. Scopri come definire il pubblico della consegna in un flusso di lavoro della campagna in [questa sezione](../workflows/activities/build-audience.md)

## Monitora i tipi di pubblico {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Properties"
>abstract="Qui è disponibile un riepilogo delle proprietà del pubblico, come l’origine, la cartella di archiviazione o il relativo stato. Fai clic sul collegamento nella sezione **Ultimo flusso di lavoro** per aprire il flusso di lavoro utilizzato per creare il pubblico."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Dimensione del pubblico"
>abstract="Qui è disponibile il numero totale di profili all’interno del pubblico. Fai clic sul pulsante Calcola per aggiornare e ricalcolare i risultati del pubblico."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Errore pubblico"
>abstract="Dati del pubblico non disponibili. Attendi la fine dell’esecuzione del flusso di lavoro."

L’elenco dei tipi di pubblico disponibili per l’utilizzo in Campaign Web è accessibile dal menu **[!UICONTROL Tipi di pubblico]**.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

I tipi di pubblico possono provenire da più origini. Le colonne **[!UICONTROL Origine]** indicano dove è stato creato un determinato pubblico:

* **[!UICONTROL Adobe Campaign]**: questi tipi di pubblico vengono creati nella console di Adobe Campaign V8. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=it){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** questi tipi di pubblico vengono creati all’interno di Adobe Experience Platform e sono integrati in Campaign Web utilizzando l’integrazione con origini e destinazioni di Adobe. Per ulteriori informazioni su come impostare questa integrazione, consulta la [Documentazione su Campaign v8 (console del client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.

  ➡️ [Scopri questa funzione nel video](#video)

* **[!UICONTROL Interfaccia web di Adobe Campaign]**: questi tipi di pubblico vengono creati utilizzando i flussi di lavoro del pubblico di Campaign Web. [Scopri come creare tipi di pubblico](create-audience.md)

Per ottenere ulteriori informazioni su un pubblico, aprilo dall’elenco. Vengono visualizzate le proprietà del pubblico, insieme al numero di profili inclusi nel pubblico. Puoi aggiornare il conteggio del pubblico in qualsiasi momento utilizzando il pulsante **[!UICONTROL Calcola]**.

La scheda **[!UICONTROL Dati]** consente di visualizzare i profili che fanno parte del pubblico. Puoi personalizzare questa vista aggiungendo più colonne o sfruttando filtri avanzati per ottimizzare i dati visualizzati.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

Per duplicare o eliminare un pubblico, fai clic sul pulsante **[!UICONTROL Altre azioni]** disponibile nell’elenco dei tipi di pubblico accanto al nome del pubblico o all’interno della schermata dei dettagli del pubblico.

## Video dimostrativo {#video}

Scopri come creare una destinazione per utilizzare un pubblico di Experienci Platform nell’interfaccia utente web di Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Informazioni dettagliate su come impostare l’integrazione Adobe Sources and Destinations sono disponibili in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.
