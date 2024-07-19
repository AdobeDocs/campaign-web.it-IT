---
audience: end-user
title: Inviare una consegna SMS
description: Scopri come inviare SMS con Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 88%

---

# Anteprima e invio di una consegna SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Metrica di nuove quarantene"
>abstract="Numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare."

## Anteprima della consegna SMS{#preview-sms}

Dopo aver definito il contenuto del messaggio, puoi utilizzare i profili di test per visualizzarlo in anteprima e testarlo. Se hai incluso contenuti personalizzati, puoi esaminare come questi vengono visualizzati nel messaggio utilizzando i dati del profilo di test. Potrai così assicurarti che il messaggio venga visualizzato come previsto e che tutte le informazioni personalizzate vengano presentate correttamente.

I passaggi principali per visualizzare in anteprima la consegna di SMS sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/sms_send_1.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi profili di test]** per selezionare uno o più profili di test o profili.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Nel riquadro a destra è disponibile un’anteprima della consegna SMS in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/sms_send_3.png){zoomable="yes"}

Ora puoi esaminare e inviare il messaggio SMS al pubblico.

## Testare la consegna SMS {#test-sms}

Con **Adobe Campaign**, puoi testare un messaggio prima di inviarlo al pubblico principale, cioè utilizzando un passaggio essenziale per convalidare la campagna e-mail e identificare potenziali problemi.

L’invio di bozze è un passaggio importante per garantire la qualità e l’efficacia della consegna. I destinatari della bozza possono esaminare vari elementi come collegamenti, collegamenti di rinuncia e immagini, nonché identificare eventuali errori nel rendering, nel contenuto, nelle impostazioni di personalizzazione e nella configurazione degli SMS. Questo processo ti aiuta a valutare e ottimizzare accuratamente gli SMS prima di raggiungere il pubblico principale.

![](../assets/do-not-localize/book.png) Scopri come inviare bozze in [questa sezione](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png){zoomable="yes"}

## Inviare la consegna SMS {#send-sms}

1. Dopo aver personalizzato il contenuto SMS, fai clic su **[!UICONTROL Rivedi e invia]** dalla pagina **[!UICONTROL Consegna]**.

   ![](assets/sms_send_4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano degli errori, fai riferimento al menu Registri per informazioni dettagliate sull’errore.

1. Per inviare i messaggi, fai clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

   ![](assets/sms_send_5.png){zoomable="yes"}

   Se la consegna SMS è stata pianificata, fai clic sul pulsante **[!UICONTROL Invia come pianificato]**. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Conferma l’azione di invio facendo clic sul pulsante **[!UICONTROL Invia]**.

Una volta inviata la consegna, puoi tenere traccia dei tuoi KPI (indicatori chiave di prestazioni) dalla pagina della consegna e dei dati dal menu **[!UICONTROL Registri]**.

Ora puoi iniziare a misurare l’impatto del messaggio utilizzando i rapporti incorporati. [Ulteriori informazioni](../reporting/sms-report.md)
