---
audience: end-user
title: Inviare una consegna SMS
description: Scopri come inviare SMS con Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 36%

---

# Anteprima e invio di una consegna SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Metrica di nuove quarantene"
>abstract="Numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare."

## Anteprima della consegna SMS {#preview-sms}

Una volta definito il contenuto del messaggio, utilizza i profili di test per visualizzarlo in anteprima e testarlo. Se è incluso un contenuto personalizzato, esamina come questo contenuto viene visualizzato nel messaggio utilizzando i dati del profilo di test. In questo modo il messaggio viene visualizzato come previsto e le informazioni personalizzate vengono presentate correttamente.

I passaggi principali per visualizzare in anteprima la consegna di SMS sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![Anteprima del contenuto SMS personalizzato](assets/sms_send_1.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi profili di test]** per selezionare uno o più profili di test o profili.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Nel riquadro a destra, visualizza un’anteprima della consegna SMS, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![Riquadro di anteprima con consegna SMS personalizzata](assets/sms_send_3.png){zoomable="yes"}

Rivedi e invia il messaggio SMS al tuo pubblico.

## Testare la consegna SMS {#test-sms}

Con **Adobe Campaign**, verifica un messaggio prima di inviarlo al pubblico principale. Questo passaggio convalida la tua campagna e-mail e identifica potenziali problemi.

L’invio di bozze è fondamentale per garantire la qualità e l’efficacia della consegna. I destinatari della bozza esaminano vari elementi come collegamenti, collegamenti di rinuncia e immagini e identificano eventuali errori nel rendering, nel contenuto, nelle impostazioni di personalizzazione e nella configurazione degli SMS. Questo processo valuta e ottimizza accuratamente gli SMS prima di raggiungere il pubblico principale.

![Icona libro per l&#39;invio di bozze](../assets/do-not-localize/book.png) Scopri come inviare bozze in [questa sezione](../preview-test/test-deliveries.md).

![Verifica della consegna SMS](assets/sms_send_6.png){zoomable="yes"}

## Inviare la consegna SMS {#send-sms}

1. Dopo aver personalizzato il contenuto SMS, fai clic su **[!UICONTROL Rivedi e invia]** dalla pagina **[!UICONTROL Consegna]**.

   ![Rivedi e invia SMS](assets/sms_send_4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano errori, fare riferimento al menu Registri per informazioni dettagliate sull&#39;errore.

1. Invia i messaggi facendo clic su **[!UICONTROL Invia]** per continuare con il processo di invio finale.

   ![Invio della consegna SMS](assets/sms_send_5.png){zoomable="yes"}

   Se la consegna SMS è pianificata, fai clic sul pulsante **[!UICONTROL Invia come pianificato]**. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Conferma l’azione di invio facendo clic sul pulsante **[!UICONTROL Invia]**.

Una volta inviata la consegna, tieni traccia dei dati KPI (Key Performance Indicator) dalla pagina di consegna e dei dati dal menu **[!UICONTROL Registri]**.

Inizia a misurare l’impatto del messaggio con i rapporti incorporati. [Ulteriori informazioni](../reporting/sms-report.md)