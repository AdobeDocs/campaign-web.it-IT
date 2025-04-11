---
audience: end-user
title: Inviare messaggi agli iscritti di un servizio
description: Scopri come inviare messaggi agli iscritti di un servizio
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 28%

---

# Inviare messaggi agli iscritti di un servizio {#send-to-subscribers}

Puoi creare servizi di abbonamento in Adobe Campaign e inviare messaggi ai tuoi abbonati. Scopri come creare servizi di abbonamento in [questa pagina](../audience//manage-services.md#create-service).

Per inviare messaggi agli iscritti, crea un pubblico specifico per identificare gli iscritti, quindi crea la consegna come descritto di seguito.

1. Crea un pubblico. Viene creato automaticamente un nuovo flusso di lavoro. [Ulteriori informazioni sui tipi di pubblico](../audience/create-audience.md)

1. Per una migliore leggibilità, modifica il nome del flusso di lavoro nel campo **Etichetta** delle impostazioni del flusso di lavoro. [Scopri come configurare le impostazioni del flusso di lavoro](../workflows/workflow-settings.md).

1. Apri l&#39;attività **[!UICONTROL Genera pubblico]** e seleziona **[!UICONTROL Crea pubblico]**. [Scopri come configurare un&#39;attività Genera pubblico](../workflows/activities/build-audience.md).

   ![Schermata che mostra la configurazione dell&#39;attività Genera pubblico in Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. Nel flusso di creazione del pubblico, seleziona le seguenti condizioni personalizzate: **[!UICONTROL Esistono abbonamenti]**, ad esempio **[!UICONTROL Il servizio]** è uguale al servizio definito. In questo esempio, seleziona la tua **newsletter yoga Luma**.

   ![Schermata che mostra il flusso di creazione del pubblico con condizioni personalizzate per gli abbonamenti in Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Seleziona **[!UICONTROL Conferma]** e fai clic su **[!UICONTROL Avvia]** per eseguire il flusso di lavoro.

1. Crea una consegna. I passaggi per creare una consegna sono descritti in [questa pagina](../msg/gs-messages.md#create-delivery).

1. Individua le impostazioni di consegna e modifica il mapping di destinazione predefinito in **Sottoscrizioni (nms:subscriptions)**.

   ![Schermata che mostra le impostazioni di consegna con la mappatura di destinazione modificata in Abbonamenti in Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Nella sezione target principale della consegna, seleziona il pubblico creato in precedenza.

   ![Schermata che mostra la sezione di destinazione principale della consegna con il pubblico selezionato in Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Crea il contenuto del messaggio, verificalo e invia la consegna, come descritto in [questa sezione](../preview-test/preview-test.md).

   ![Schermata che mostra la consegna pronta per essere inviata in Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

La consegna viene inviata solo agli utenti iscritti per tale servizio.