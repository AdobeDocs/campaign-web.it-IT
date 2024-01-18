---
audience: end-user
title: Inviare messaggi agli iscritti di un servizio
description: Scopri come inviare messaggi agli iscritti di un servizio
badge: label="Disponibilità limitata"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 100%

---

# Inviare messaggi agli iscritti di un servizio {#send-to-subscribers}

Puoi creare servizi di iscrizione in Adobe Campaign e inviare messaggi agli utenti iscritti. Per sccoprire come creare servizi di iscrizione, consulta [questa pagina](../audience//manage-services.md#create-service).

Per inviare messaggi agli iscritti, crea un pubblico specifico per identificare gli iscritti, quindi crea la consegna come descritto di seguito.

1. Crea un pubblico. Per ulteriori informazioni sui tipi di pubblico, consulta [questa pagina](../audience/create-audience.md).

1. Nell’attività **[!UICONTROL Crea pubblico]**, visualizza gli attributi avanzati e seleziona **[!UICONTROL Destinatario]** > **[!UICONTROL Iscrizioni]** > **[!UICONTROL Servizio]**.

   In questo esempio, seleziona gli utenti iscritti per il servizio con etichetta **Newsletter Luma**.

   ![](assets/service-audience-subscribers.png)

1. Salva il pubblico.
1. Crea una consegna. I passaggi per creare una consegna sono descritti in [questa pagina](../msg/gs-messages.md#create-delivery).
1. Individua le impostazioni di consegna e modifica la mappatura target predefinita in **Abbonamenti (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Nella sezione target principale della consegna, seleziona il pubblico creato in precedenza.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Crea il contenuto del messaggio, esegui un test e invia la consegna, come descritto in [questa sezione](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

La consegna viene inviata solo agli utenti iscritti per tale servizio.
