---
audience: end-user
title: Inviare una consegna di notifica push
description: Scopri come inviare una consegna di tipo notifica push con Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 80%

---

# Anteprima e invio di una consegna push {#send-push-delivery}

## Anteprima della consegna di notifiche push {#preview-push}

Dopo aver definito il contenuto del messaggio, puoi utilizzare iscritti a scopo di test per visualizzarlo in anteprima e testarlo. Se hai incluso contenuti personalizzati, puoi esaminare come questi vengono visualizzati nel messaggio utilizzando i dati del profilo di test. Potrai così assicurarti che il messaggio venga riprodotto correttamente e che gli elementi personalizzati vengano incorporati in modo appropriato.

I passaggi principali per visualizzare in anteprima la notifica push sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/push_send_1.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi iscritti]** per selezionare uno o più profili in modo da visualizzarne in anteprima i dati nel contenuto della notifica push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. Nel riquadro a destra è disponibile un’anteprima della notifica push, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/push_send_7.png){zoomable="yes"}

Ora puoi rivedere e inviare le notifiche push al pubblico.

## Test della consegna di notifiche push {#test-push}

Utilizzando **Adobe Campaign**, puoi inviare bozze prima di inviarle al pubblico principale. Questo passaggio è importante per convalidare la consegna e identificare eventuali problemi.

I profili di test sono i destinatari della bozza. Possono rivedere e convalidare componenti e impostazioni quali collegamenti, immagini e personalizzazione, garantendo prestazioni ottimali e il rilevamento di eventuali errori. Questo processo ti aiuta a perfezionare e ottimizzare le notifiche push prima di raggiungere il pubblico principale. [Scopri come inviare bozze](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable="yes"}

## Inviare la consegna di notifiche push {#send-push}

1. Dopo aver personalizzato il contenuto della notifica push, fai clic su **[!UICONTROL Rivedi e invia]** nella pagina **[!UICONTROL Consegna]**.

   ![](assets/push_send_2.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano degli errori, fai riferimento al menu Registri per informazioni dettagliate sull’errore.

   ![](assets/push_send_3.png){zoomable="yes"}

1. Per inviare i messaggi, fai clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

1. Conferma l’azione di invio facendo clic su **[!UICONTROL Invia]**.

   Se la consegna push è stata pianificata, fai clic sul pulsante **[!UICONTROL Invia come pianificato]**. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable="yes"}

Una volta inviata la consegna, puoi tenere traccia dei tuoi KPI (indicatori chiave di prestazioni) dalla pagina della consegna e dei dati dal menu **[!UICONTROL Registri]**.

Ora puoi iniziare a misurare l’impatto del messaggio utilizzando i rapporti incorporati. [Ulteriori informazioni](../reporting/push-report.md)
