---
audience: end-user
title: Monitorare e gestire i tipi di pubblico
description: Scopri come monitorare e gestire i tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 14%

---


# Monitorare e gestire i tipi di pubblico {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Errore di pubblico"
>abstract="I dati sul pubblico non sono disponibili. Attendi la fine dell&#39;esecuzione del flusso di lavoro."

L’elenco dei tipi di pubblico disponibili per l’utilizzo in Campaign Web è accessibile dalla pagina **[!UICONTROL Tipi di pubblico]** menu.

![](assets/audiences-list.png)

I tipi di pubblico possono provenire da più sorgenti. Il **[!UICONTROL Origine]** Le colonne indicano dove è stato creato un determinato pubblico:

* **[!UICONTROL Adobe Campaign]**: questi tipi di pubblico vengono creati nella console di Adobe Campaign V8. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=it){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Questi tipi di pubblico vengono creati all’interno di Adobe Experience Platform e sono integrati in Campaign Web utilizzando l’integrazione Adobe Sources and Destinations. Scopri come impostare questa integrazione in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

>[!NOTE]
>
>Per utilizzare i tipi di pubblico di Adobe Experience Platform in Campaign, devi configurare l’integrazione con origini e destinazioni di Adobe. Consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Interfaccia web di Adobe Campaign]**: questi tipi di pubblico vengono creati utilizzando i flussi di lavoro Pubblico web di Campaign. [Scopri come creare tipi di pubblico](create-audience.md)

Per ottenere ulteriori informazioni su un pubblico, aprilo dall’elenco. Vengono visualizzate le proprietà del pubblico e il numero di profili inclusi nel pubblico. Puoi aggiornare il conteggio del pubblico in qualsiasi momento utilizzando **[!UICONTROL Calcola]** pulsante.

Il **[!UICONTROL Dati]** Questa scheda ti consente di visualizzare i profili che fanno parte del pubblico. Puoi personalizzare questa visualizzazione aggiungendo più colonne o sfruttando filtri avanzati per perfezionare i dati visualizzati.

![](assets/audiences-details.png)

Per duplicare o eliminare un pubblico, fai clic su **[!UICONTROL Altre azioni]** disponibile nell’elenco dei tipi di pubblico accanto al nome del pubblico o all’interno della schermata dei dettagli del pubblico.