---
audience: end-user
title: Inviare messaggi agli abbonati di un servizio
description: Scopri come inviare messaggi agli abbonati di un servizio
badge: label="Beta"
source-git-commit: e5ef71de970468fce418cc06cb9d2c25c0c40306
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 3%

---


# Inviare messaggi agli abbonati di un servizio

Puoi creare servizi di abbonamento in Adobe Campaign e inviare messaggi ai tuoi abbonati. Scopri come creare servizi di abbonamento in [questa pagina](../audience//manage-services.md#create-service).

Per inviare messaggi agli abbonati, crea un pubblico specifico per identificare gli abbonati, quindi crea la consegna come descritto di seguito.

1. Creazione di un pubblico. Ulteriori informazioni sui tipi di pubblico in [questa pagina](../audience/create-audience.md).

1. In **[!UICONTROL Creare un pubblico]** attività, visualizza gli attributi avanzati e seleziona **[!UICONTROL Destinatario]** > **[!UICONTROL Iscrizioni]** > **[!UICONTROL Servizio]**.

   In questo esempio, seleziona gli utenti abbonati al servizio che dispone di **Newsletter Luma** etichetta.

   ![](assets/service-audience-subscribers.png)

1. Salva il pubblico.
1. Creare una consegna. I passaggi per creare una consegna sono descritti in [questa pagina](../msg/gs-messages.md#create-delivery).
1. Individua le impostazioni di consegna e modifica la mappatura di destinazione predefinita in **Sottoscrizioni (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Nella sezione di destinazione principale della consegna, seleziona il pubblico creato in precedenza.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Crea il contenuto del messaggio, verifica e invia la consegna, come descritto in [questa sezione](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

La consegna viene inviata solo agli abbonati di tale servizio.
