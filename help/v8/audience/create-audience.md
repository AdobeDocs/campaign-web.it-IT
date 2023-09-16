---
audience: end-user
title: Creare tipi di pubblico
description: Scopri come creare tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
source-git-commit: a61eb527f22346c51b935e4170e1a56bed428f78
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 2%

---


# Creare tipi di pubblico {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Da questa schermata, puoi creare e combinare i tipi di pubblico in un’area di lavoro visiva. Aggiungi varie attività del flusso di lavoro, ad esempio **Dividi** o **Escludi** per generare un pubblico nuovo e perfezionato."


>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Impostazioni pubblico"
>abstract="Immetti il nome del pubblico e altre opzioni, quindi fai clic sul pulsante **Crea pubblico** pulsante."

Campaign Web consente di creare flussi di lavoro in cui combinare i tipi di pubblico esistenti in un’area di lavoro visiva. incorporando varie attività del flusso di lavoro, ad esempio **Dividi** o **Escludi**, puoi generare un pubblico nuovo e perfezionato.

Dopo aver creato il flusso di lavoro, i tipi di pubblico risultanti vengono memorizzati automaticamente all’interno di Campaign Web insieme a quelli esistenti. Questi tipi di pubblico possono quindi essere oggetto di targeting in campagne o consegne autonome.

Per creare un pubblico, segui questi passaggi:

1. Accedi a **[!UICONTROL Tipi di pubblico]** e fai clic sul pulsante **[!UICONTROL Crea pubblico]** nell&#39;angolo superiore destro.
1. Fornisci un’etichetta per il pubblico.
1. Espandi **[!UICONTROL Opzioni aggiuntive]** per configurare parametri di pubblico avanzati.

   Per impostazione predefinita, i tipi di pubblico vengono creati in **[!UICONTROL Profili e destinazioni]** / **[!UICONTROL Elenchi]** menu di esplora risorse. È possibile modificare il percorso di archiviazione predefinito utilizzando **[!UICONTROL Cartella]** campo.

   ![](assets/audiences-settings.png)

1. Dopo aver configurato le impostazioni per il pubblico, fai clic su **[!UICONTROL Crea pubblico]** pulsante.

1. Viene visualizzata un’area di lavoro del flusso di lavoro con due attività predefinite:

   * **[!UICONTROL Creare un pubblico]**: questo è il punto di partenza del flusso di lavoro, che consente di creare un pubblico e utilizzarlo come base per il flusso di lavoro.
   * **[!UICONTROL Salva pubblico]**: questo rappresenta il passaggio finale nel flusso di lavoro, che consente di salvare i risultati come un nuovo pubblico.

1. Personalizza il flusso di lavoro aggiungendo tutte le attività necessarie. Per ulteriori informazioni su come configurare le attività del flusso di lavoro, consulta [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro del pubblico.

   ![](assets/audience-creation-canvas.png)

1. Quando il workflow è pronto, fai clic su **[!UICONTROL Inizio]** per eseguirlo.

1. Il flusso di lavoro viene salvato in **[!UICONTROL Flussi di lavoro]** , mentre i tipi di pubblico risultanti sono accessibili nel **[!UICONTROL Tipi di pubblico]** elenco. [Scopri come monitorare e gestire i tipi di pubblico](access-audiences.md)
