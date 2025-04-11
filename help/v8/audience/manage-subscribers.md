---
audience: end-user
title: Gestire gli abbonati
description: Scopri come gestire e consegnare alle persone iscritte a un servizio in Adobe Campaign Web
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 40%

---

# Gestire gli abbonati {#manage-subscribers}

Dopo aver [creato un servizio](manage-services.md#create-service), puoi aggiungere utenti iscritti, annullare l’iscrizione dei destinatari e inviare messaggi agli iscritti al servizio.

La gestione degli abbonati è descritta in questa pagina. Per informazioni su come inviare messaggi alle persone iscritte, consulta [questa sezione](../msg/send-to-subscribers.md).

## Aggiungere iscritti al servizio {#add-subscribers}

Per aggiungere manualmente degli utenti iscritti, segui i passaggi seguenti.

1. Seleziona un servizio esistente dall’elenco **[!UICONTROL Servizi di iscrizione]**.

1. Passare alla scheda **[!UICONTROL Sottoscrittori]** e fare clic su **[!UICONTROL Aggiungi sottoscrittori]**.

   ![Schermata che mostra la scheda Sottoscrittori nell&#39;interfaccia dei servizi di abbonamento.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Selezionare i profili da aggiungere dall&#39;elenco e fare clic su **[!UICONTROL Conferma]**.

   ![Schermata che mostra l&#39;interfaccia di selezione del profilo per l&#39;aggiunta dei sottoscrittori.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Invia]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> per fare in modo che i destinatari selezionati ricevano il [messaggio di conferma](manage-services.md#create-confirmation-message) della sottoscrizione definito durante la [creazione del servizio](manage-services.md#create-service).

   ![Schermata che mostra l&#39;interfaccia del messaggio di conferma per l&#39;aggiunta dei sottoscrittori.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se si seleziona **[!UICONTROL Annulla]**, ai profili selezionati non viene inviato alcun messaggio di conferma, ma sono sottoscritti.

I profili aggiunti vengono visualizzati nella scheda **[!UICONTROL Abbonati]**. Questi sono ora iscritti al servizio.

## Rimuovere degli iscritti dal servizio {#remove-subscribers}

### Annullare manualmente l’abbonamento dei profili {#manual-unsubscription}

Dopo aver [aggiunto iscritti](#add-subscribers) al servizio, puoi annullare manualmente l’iscrizione di ciascuno di essi. Segui i passaggi seguenti.

1. Seleziona un servizio esistente dall’elenco **[!UICONTROL Servizi di iscrizione]**.

1. Fai clic sull&#39;icona dei tre punti accanto al nome del destinatario desiderato e seleziona **[!UICONTROL Elimina]**.

   ![Schermata che mostra l&#39;opzione Elimina per annullare l&#39;abbonamento dei profili.](assets/service-subscribers-delete.png){zoomable="yes"}

1. Conferma l’eliminazione.

1. Fai clic su **[!UICONTROL Invia]** per fare in modo che il destinatario selezionato riceva il [messaggio di conferma](manage-services.md#create-confirmation-message) dell&#39;annullamento dell&#39;abbonamento definito durante la [creazione del servizio](manage-services.md#create-service).

   ![Schermata che mostra l&#39;interfaccia del messaggio di conferma per l&#39;annullamento dell&#39;abbonamento dei profili.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

Il destinatario viene rimosso dalla scheda **[!UICONTROL Abbonati]** e non è più abbonato al servizio.

### Annullare automaticamente l’iscrizione dei destinatari {#automatic-unsubscription}

Un servizio di iscrizione può avere una durata limitata. L’abbonamento ai profili viene annullato automaticamente alla scadenza del periodo di validità.

Questo periodo viene specificato durante la [creazione del servizio](manage-services.md#create-service). Da **[!UICONTROL Opzioni aggiuntive]**, disabilita l&#39;opzione **[!UICONTROL Periodo di validità illimitato]** e definisci un periodo di validità per il servizio.

![Schermata che mostra la configurazione del periodo di validità per un servizio di abbonamento.](assets/service-create-validity-period.png){zoomable="yes"}

Alla scadenza della durata specificata, per tutti gli iscritti verrà automaticamente annullata l’iscrizione a tale servizio.