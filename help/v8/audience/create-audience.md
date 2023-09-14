---
audience: end-user
title: Creare tipi di pubblico
description: Scopri come creare tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 1%

---


# Creare tipi di pubblico {#create-audiences}

Campaign Web consente di creare flussi di lavoro in cui combinare i tipi di pubblico esistenti in un’area di lavoro visiva e sfruttare varie attività (suddivisione, esclusione...) per creare nuovi tipi di pubblico.

Al termine, i tipi di pubblico risultanti vengono salvati e inseriti nel backup in Campaign Web insieme ai tipi di pubblico esistenti e possono essere utilizzati in consegne o campagne autonome per il targeting di singoli utenti.

## Creare il primo pubblico {#create}

Per creare un pubblico, segui questi passaggi:

1. Accedi a **[!UICONTROL Tipi di pubblico]** e fai clic su **[!UICONTROL Crea pubblico]** nell&#39;angolo in alto a destra.
1. Fornisci un’etichetta per il pubblico.
1. Espandi la sezione Opzioni aggiuntive per configurare i parametri avanzati per il pubblico.

   >[!NOTE]
   >
   >Per impostazione predefinita, i tipi di pubblico vengono creati nel menu Esplora profili e destinazioni/elenchi. È possibile modificare il percorso di archiviazione predefinito in **[!UICONTROL Cartella]** campo.

1. Una volta configurate le impostazioni del pubblico, fai clic su **[!UICONTROL Crea pubblico]** pulsante.

1. Viene visualizzata un’area di lavoro del flusso di lavoro con due attività predefinite:

   * **[!UICONTROL Creare un pubblico]**: punto iniziale del flusso di lavoro. Questa attività ti consente di selezionare uno o più tipi di pubblico come base per il flusso di lavoro,
   * **[!UICONTROL Salva pubblico]**: ultimo passaggio del flusso di lavoro. Questa attività ti consente di salvare il risultato del flusso di lavoro in un nuovo pubblico.

1. Configura il flusso di lavoro aggiungendo tutte le attività necessarie. Per ulteriori informazioni su come configurare le varie attività, consulta [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro del pubblico.

   ![](assets/audience-creation-canvas.png)

1. Quando il workflow è pronto, fai clic su **[!UICONTROL Inizio]** per eseguirlo.

1. Il flusso di lavoro viene salvato in **[!UICONTROL Flussi di lavoro]** e i tipi di pubblico risultanti nel **[!UICONTROL Tipi di pubblico]** elenco. [Scopri come monitorare e gestire i tipi di pubblico](access-audiences.md)
