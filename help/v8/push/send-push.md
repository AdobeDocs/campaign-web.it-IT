---
audience: end-user
title: Inviare una consegna di notifica push
description: Scopri come inviare una notifica push con Adobe Campaign Web
badge: label="Alpha"
source-git-commit: c24b53ee17e81805f0717682202d2d4154c96c1e
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Anteprima e invio di una consegna di notifica push {#send-push-delivery}

## Anteprima della consegna delle notifiche push {#preview-push}

Dopo aver definito il contenuto del messaggio, puoi utilizzare gli abbonati di prova per visualizzare in anteprima e verificare il messaggio. Se hai incluso contenuti personalizzati, puoi esaminare come questi contenuti vengono visualizzati nel messaggio utilizzando i dati del profilo di test. Ciò ti consente di garantire che il messaggio venga renderizzato correttamente e che gli elementi personalizzati vengano incorporati in modo appropriato.

I passaggi principali per visualizzare in anteprima la consegna SMS sono i seguenti. Ulteriori dettagli su come visualizzare in anteprima le consegne sono disponibili in [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, utilizza **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/push_send_1.png)

1. Clic **[!UICONTROL Aggiungi abbonati]** per selezionare uno o più profili per visualizzare in anteprima i loro dati nel contenuto della notifica push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. Nel riquadro a destra è disponibile un’anteprima della notifica push, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/push_send_7.png)

Ora puoi rivedere e inviare la notifica push al pubblico.

## Test della consegna delle notifiche push {#test-push}

Utilizzo di **Adobe Campaign**, puoi testare le notifiche push prima di inviarle al pubblico principale. Questo passaggio è importante per convalidare la consegna e identificare eventuali problemi.
I destinatari del test possono rivedere elementi quali collegamenti, immagini e impostazioni di personalizzazione, garantendo prestazioni ottimali e rilevando eventuali errori. Questo processo ti aiuta a perfezionare e ottimizzare le notifiche push prima di raggiungere il pubblico principale.

![](../assets/do-not-localize/book.png) Scopri come inviare notifiche push di prova in [questa sezione](../preview-test/proofs.md#subscribers).

![](assets/push_send_6.png)

## Inviare la consegna delle notifiche push {#send-push}

1. Dopo aver personalizzato il contenuto della notifica push, fai clic su **[!UICONTROL Rivedi e invia]** dal tuo **[!UICONTROL Consegna]** pagina.

   ![](assets/push_send_2.png)

1. Fai clic su **[!UICONTROL Prepara]**e monitorare i progressi e le statistiche fornite.

   Se si verificano errori, fare riferimento al menu Registri per informazioni dettagliate sull&#39;errore.

   ![](assets/push_send_3.png)

1. Inviare i messaggi facendo clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

1. Conferma l’azione di invio facendo clic sul pulsante **[!UICONTROL Invia]** o **[!UICONTROL Invia come pianificato]** pulsante.

   ![](assets/push_send_4.png)

Una volta inviata la consegna, puoi tracciare i dati KPI (Key Performance Indicator, indicatore di prestazioni chiave) dalla pagina di consegna e i dati da **[!UICONTROL Registri]** menu.

Ora puoi iniziare a misurare l’impatto del messaggio con i rapporti incorporati. [Ulteriori informazioni](../reporting/push-report.md)
