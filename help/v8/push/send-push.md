---
audience: end-user
title: Inviare una consegna di notifica push
description: Scopri come inviare una consegna di tipo notifica push con Adobe Campaign Web
badge: label="Alpha"
source-git-commit: 4a439abca9c7b1f2cc5d82214efb0aae033a996c
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 57%

---

# Anteprima e invio di una consegna di notifica push {#send-push-delivery}

## Anteprima della consegna di notifiche push {#preview-push}

Dopo aver definito il contenuto del messaggio, puoi utilizzare gli abbonati di prova per visualizzare in anteprima e verificare il messaggio. Se hai incluso contenuti personalizzati, puoi esaminare come questi contenuti vengono visualizzati nel messaggio utilizzando i dati del profilo di test. Potrai così assicurarti che il messaggio venga riprodotto correttamente e che gli elementi personalizzati vengano incorporati in modo appropriato.

I passaggi principali per visualizzare in anteprima la consegna SMS sono i seguenti. Ulteriori dettagli su come visualizzare in anteprima le consegne sono disponibili in [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, utilizza **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/push_send_1.png)

1. Clic **[!UICONTROL Aggiungi abbonati]** per selezionare uno o più profili per visualizzare in anteprima i loro dati nel contenuto della notifica push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. Nel riquadro a destra è disponibile un’anteprima della notifica push, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/push_send_7.png)

Ora puoi rivedere e inviare le notifiche push al pubblico.

## Test della consegna di notifiche push {#test-push}

In **Adobe Campaign** puoi testare le notifiche push prima di inviarle al pubblico principale. Questo passaggio è importante per convalidare la consegna e individuare eventuali problemi.
I destinatari del test possono rivedere elementi quali collegamenti, immagini e impostazioni di personalizzazione, al fine di garantire prestazioni ottimali e rilevare eventuali errori. Questo processo è utile per perfezionare e ottimizzare le notifiche push prima di inviarle al pubblico principale.

![](../assets/do-not-localize/book.png) Scopri come inviare notifiche push di prova in [questa sezione](../preview-test/test-deliveries.md#subscribers).

![](assets/push_send_6.png)

## Inviare la consegna di notifiche push {#send-push}

1. Dopo aver personalizzato il contenuto della notifica push, fai clic su **[!UICONTROL Rivedi e invia]** nella pagina **[!UICONTROL Consegna]**.

   ![](assets/push_send_2.png)

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano degli errori, fai riferimento al menu Registri per informazioni dettagliate sull’errore.

   ![](assets/push_send_3.png)

1. Per inviare i messaggi, fai clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

1. Conferma l’azione di invio facendo clic sul pulsante **[!UICONTROL Invia]** o **[!UICONTROL Invia come pianificato]**.

   ![](assets/push_send_4.png)

Una volta inviata la consegna, puoi tracciare i dati KPI (Key Performance Indicator, indicatore di prestazioni chiave) dalla pagina di consegna e i dati da **[!UICONTROL Registri]** menu.

Ora puoi iniziare a misurare l’impatto del messaggio utilizzando i rapporti incorporati. [Ulteriori informazioni](../reporting/push-report.md)
