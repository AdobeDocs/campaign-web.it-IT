---
audience: end-user
title: Monitorare e gestire i tipi di pubblico
description: Scopri come monitorare e gestire i tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 1f2a6e0944f46c0e37ce9e2b174a08e69981d143
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 100%

---

# Monitorare e gestire i tipi di pubblico {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Errore pubblico"
>abstract="Dati del pubblico non disponibili. Attendi la fine dell’esecuzione del flusso di lavoro."

Il pubblico è il target principale della consegna: i destinatari che ricevono i messaggi. Il tipo di pubblico dipende dalla mappatura target definita nel modello di consegna. Ulteriori informazioni sui modelli di consegna sono disponibili in [questa pagina](../msg/delivery-template.md).

Per definire la popolazione di un pubblico, puoi:

* [Creare nuovi tipi di pubblico](create-audience.md) dal menu **[!UICONTROL Tipi di pubblico]**
* [Selezionare un pubblico esistente](add-audience.md) creato come elenco nella console client o proveniente da Adobe Experience Platform
* [Creare un nuovo pubblico](../query/query-modeler-overview.md) con il generatore di regole definendo e combinando criteri di filtro
* [Utilizzare un pubblico da un file esterno](file-audience.md); questa opzione è disponibile solo per le consegne e-mail autonome e non può essere utilizzata nelle consegne delle campagne.

Nel targeting di un pubblico, puoi definire dei **gruppi di controllo** per evitare di inviare messaggi a una parte del pubblico, in modo da misurare l’impatto delle campagne. [Scopri come impostare un gruppo di controllo](control-group.md)

>[!NOTE]
>
>Quando si inviano messaggi nel contesto del flusso di lavoro di una campagna, il pubblico viene definito in una specifica attività **Crea pubblico** del flusso di lavoro. In questo contesto, non puoi caricare un pubblico da un file per una consegna e-mail e il pubblico è definito solo in questa attività dedicata. Scopri come definire il pubblico della consegna in un flusso di lavoro della campagna in [questa sezione](../workflows/activities/build-audience.md)

L’elenco dei tipi di pubblico disponibili per l’utilizzo in Campaign Web è accessibile dal menu **[!UICONTROL Tipi di pubblico]**.

![](assets/audiences-list.png)

I tipi di pubblico possono provenire da più origini. Le colonne **[!UICONTROL Origine]** indicano dove è stato creato un determinato pubblico:

* **[!UICONTROL Adobe Campaign]**: questi tipi di pubblico vengono creati nella console di Adobe Campaign V8. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=it){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** questi tipi di pubblico vengono creati all’interno di Adobe Experience Platform e sono integrati in Campaign Web utilizzando l’integrazione con origini e destinazioni di Adobe. Per ulteriori informazioni su come impostare questa integrazione, consulta la [Documentazione su Campaign v8 (console del client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.

>[!NOTE]
>
>Per utilizzare i tipi di pubblico di Adobe Experience Platform in Campaign, devi configurare l’integrazione con origini e destinazioni di Adobe. Consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.

* **[!UICONTROL Interfaccia web di Adobe Campaign]**: questi tipi di pubblico vengono creati utilizzando i flussi di lavoro del pubblico di Campaign Web. [Scopri come creare tipi di pubblico](create-audience.md)

Per ottenere ulteriori informazioni su un pubblico, aprilo dall’elenco. Vengono visualizzate le proprietà del pubblico, insieme al numero di profili inclusi nel pubblico. Puoi aggiornare il conteggio del pubblico in qualsiasi momento utilizzando il pulsante **[!UICONTROL Calcola]**.

La scheda **[!UICONTROL Dati]** consente di visualizzare i profili che fanno parte del pubblico. Puoi personalizzare questa vista aggiungendo più colonne o sfruttando filtri avanzati per ottimizzare i dati visualizzati.

![](assets/audiences-details.png)

Per duplicare o eliminare un pubblico, fai clic sul pulsante **[!UICONTROL Altre azioni]** disponibile nell’elenco dei tipi di pubblico accanto al nome del pubblico o all’interno della schermata dei dettagli del pubblico.
