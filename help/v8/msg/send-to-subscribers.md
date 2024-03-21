---
audience: end-user
title: Inviare messaggi agli iscritti di un servizio
description: Scopri come inviare messaggi agli iscritti di un servizio
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 63%

---

# Inviare messaggi agli iscritti di un servizio {#send-to-subscribers}

Puoi creare servizi di iscrizione in Adobe Campaign e inviare messaggi agli utenti iscritti. Scopri come creare servizi di abbonamento su [questa pagina](../audience//manage-services.md#create-service).

Per inviare messaggi agli iscritti, crea un pubblico specifico per identificare gli iscritti, quindi crea la consegna come descritto di seguito.

1. Crea un pubblico. Viene creato automaticamente un nuovo flusso di lavoro. [Ulteriori informazioni sui tipi di pubblico](../audience/create-audience.md)

1. Per una migliore leggibilità, modifica il nome del flusso di lavoro nelle impostazioni del flusso di lavoro&quot; **Etichetta** campo. [Scopri come configurare le impostazioni del flusso di lavoro](../workflows/workflow-settings.md)

1. Apri **[!UICONTROL Creare un pubblico]** attività e seleziona **[!UICONTROL Creare un pubblico]**. [Scopri come configurare un’attività Crea pubblico](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png){zoomable=&quot;yes&quot;}

1. Nel flusso di creazione del pubblico, seleziona le seguenti condizioni personalizzate: **[!UICONTROL Sottoscrizioni]** esistono come **[!UICONTROL Servizio]** è uguale al servizio definito. In questo esempio, seleziona il tuo **Newsletter yoga Luma**.

   ![](assets/service-audience-subscribers.png){zoomable=&quot;yes&quot;}

1. Seleziona **[!UICONTROL Conferma]** e fai clic su **[!UICONTROL Inizio]** per eseguire il workflow.

1. Crea una consegna. I passaggi per creare una consegna sono descritti in [questa pagina](../msg/gs-messages.md#create-delivery).
1. Individua le impostazioni di consegna e modifica la mappatura target predefinita in **Abbonamenti (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png){zoomable=&quot;yes&quot;}

1. Nella sezione target principale della consegna, seleziona il pubblico creato in precedenza.

   ![](assets/service-delivery-targeting-subscribers.png){zoomable=&quot;yes&quot;}

1. Crea il contenuto del messaggio, esegui un test e invia la consegna, come descritto in [questa sezione](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png){zoomable=&quot;yes&quot;}

La consegna viene inviata solo agli utenti iscritti per tale servizio.
