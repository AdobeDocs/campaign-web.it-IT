---
audience: end-user
title: Inviare una consegna di notifica push
description: Scopri come inviare una consegna di tipo notifica push con Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 31%

---

# Anteprima e invio di una consegna push {#send-push-delivery}

## Anteprima della consegna di notifiche push {#preview-push}

Una volta definito il contenuto del messaggio, utilizza i sottoscrittori di test per visualizzarlo in anteprima e testarlo. Se è incluso un contenuto personalizzato, esamina come questo contenuto viene visualizzato nel messaggio utilizzando i dati del profilo di test. In questo modo il messaggio viene renderizzato correttamente e gli elementi personalizzati vengono incorporati in modo appropriato.

I passaggi principali per visualizzare in anteprima la notifica push sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![Anteprima del contenuto personalizzato nella pagina del contenuto della consegna](assets/push_send_1.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi iscritti]** per selezionare uno o più profili in modo da visualizzarne in anteprima i dati nel contenuto della notifica push.

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. Nel riquadro a destra, individua un’anteprima della notifica push, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![Riquadro di anteprima con elementi personalizzati sostituiti con dati del profilo](assets/push_send_7.png){zoomable="yes"}

Rivedi e invia la notifica push al pubblico.

## Test della consegna di notifiche push {#test-push}

Utilizzando **Adobe Campaign**, invia le bozze prima di distribuirle al pubblico principale. Questo passaggio convalida la consegna e identifica eventuali problemi.

I profili di test fungono da destinatari della bozza. Rivedono e convalidano componenti e impostazioni quali collegamenti, immagini e personalizzazione, garantendo prestazioni ottimali e rilevando gli errori. Questo processo perfeziona e ottimizza le notifiche push prima di raggiungere il pubblico principale. [Scopri come inviare bozze](../preview-test/test-deliveries.md#subscribers).

![Verifica della consegna delle notifiche push con destinatari bozza](assets/push_send_6.png){zoomable="yes"}

## Inviare la consegna di notifiche push {#send-push}

1. Dopo aver personalizzato il contenuto della notifica push, fai clic su **[!UICONTROL Rivedi e invia]** nella pagina **[!UICONTROL Consegna]**.

   ![Pulsante Rivedi e invia nella pagina di consegna](assets/push_send_2.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano errori, fare riferimento al menu Registri per informazioni dettagliate sull&#39;errore.

   ![Monitoraggio dell&#39;avanzamento della preparazione e delle statistiche](assets/push_send_3.png){zoomable="yes"}

1. Invia i messaggi facendo clic su **[!UICONTROL Invia]** per continuare con il processo di invio finale.

1. Confermare l&#39;azione di invio facendo clic su **[!UICONTROL Invia]**.

   Se la consegna push è pianificata, fai clic sul pulsante **[!UICONTROL Invia come pianificato]**. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![Pulsante Invia come pianificato per la consegna push pianificata](assets/push_send_4.png){zoomable="yes"}

Una volta inviata la consegna, tieni traccia dei dati dell&#39;indicatore di prestazioni chiave (KPI) dalla pagina di consegna e dei dati dal menu **[!UICONTROL Registri]**.

Inizia a misurare l’impatto del messaggio con i rapporti incorporati. [Ulteriori informazioni](../reporting/push-report.md).