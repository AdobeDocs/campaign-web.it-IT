---
audience: end-user
title: Gestire gli abbonati
description: Scopri come gestire e consegnare alle persone iscritte a un servizio in Adobe Campaign Web
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 66%

---

# Gestire gli abbonati {#manage-subscribers}

Dopo aver [creato un servizio](manage-services.md#create-service), puoi aggiungere utenti iscritti, annullare l’iscrizione dei destinatari e inviare messaggi agli iscritti al servizio.

La gestione degli utenti iscritti è descritta in questa pagina. Per informazioni su come inviare messaggi alle persone iscritte, consulta [questa sezione](../msg/send-to-subscribers.md).

## Aggiungere iscritti al servizio {#add-subscribers}

Per aggiungere manualmente degli utenti iscritti, segui i passaggi seguenti.

1. Seleziona un servizio esistente dall’elenco **[!UICONTROL Servizi di iscrizione]**.

1. Vai a **[!UICONTROL Abbonati]** e fai clic su **[!UICONTROL Aggiungi abbonati]**.

   ![](assets/service-subscribers-tab.png){zoomable=&quot;yes&quot;}

1. Seleziona nell’elenco i profili da aggiungere e fai clic su **[!UICONTROL Conferma]**.

   ![](assets/service-subscribers-select-profiles.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Invia]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> per fare in modo che i destinatari selezionati ricevano l’abbonamento [messaggio di conferma](manage-services.md#create-confirmation-message) definito quando [creazione del servizio](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Se si seleziona **[!UICONTROL Annulla]**, ai profili selezionati non viene inviato alcun messaggio di conferma, ma sono abbonati.

I profili aggiunti vengono visualizzati nel **[!UICONTROL Abbonati]** scheda. Questi sono ora iscritti al servizio.

## Rimuovere degli iscritti dal servizio {#remove-subscribers}

### Annullare manualmente l’iscrizione dei destinatari {#manual-unsubscription}

Dopo aver [aggiunto iscritti](#add-subscribers) al servizio, puoi annullare manualmente l’iscrizione di ciascuno di essi. Segui i passaggi seguenti.

1. Seleziona un servizio esistente dall’elenco **[!UICONTROL Servizi di iscrizione]**.

1. Fai clic sull’icona con i tre punti accanto al nome del destinatario desiderato e seleziona **[!UICONTROL Elimina]**.

   ![](assets/service-subscribers-delete.png){zoomable=&quot;yes&quot;}

1. Conferma l’eliminazione.

1. Clic **[!UICONTROL Invia]** affinché il destinatario selezionato riceva l’annullamento dell’abbonamento [messaggio di conferma](manage-services.md#create-confirmation-message) definito quando [creazione del servizio](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png){zoomable=&quot;yes&quot;}

Il destinatario viene rimosso dal **[!UICONTROL Abbonati]** e non è più abbonato al servizio.

### Annullare automaticamente l’iscrizione dei destinatari {#automatic-unsubscription}

Un servizio di iscrizione può avere una durata limitata. L’iscrizione dei destinatari viene automaticamente annullata alla scadenza di tale periodo di validità.

Questo periodo viene specificato durante la [creazione del servizio](manage-services.md#create-service). Dalle **[!UICONTROL Opzioni aggiuntive]**, disabilita l’opzione **[!UICONTROL Periodo di validità illimitato]** e definisci un periodo di validità per il servizio.

![](assets/service-create-validity-period.png){zoomable=&quot;yes&quot;}

Alla scadenza della durata specificata, per tutti gli iscritti verrà automaticamente annullata l’iscrizione a tale servizio.
