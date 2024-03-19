---
audience: end-user
title: Anteprima e invio di una consegna direct mailing
description: Scopri come visualizzare in anteprima e inviare una consegna di direct mailing con Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 14%

---


# Anteprima e invio di una consegna direct mailing {#send-direct-mail}

Dopo aver configurato il file di estrazione per la consegna di direct mailing, puoi utilizzare i profili di test per visualizzarlo in anteprima. Se hai incluso contenuti personalizzati, puoi esaminare come questi contenuti vengono visualizzati nelle colonne utilizzando i dati del profilo di test. Ciò ti consente di garantire che il contenuto del file venga riprodotto correttamente e che gli elementi personalizzati vengano incorporati in modo appropriato.

Quando il file di estrazione è pronto, puoi inviare la consegna di direct mailing per generare il file e condividerlo con il provider di direct mailing. [Scopri come inviare la consegna di direct mailing](#dm-send)

## Anteprima del file di estrazione {#preview-dm}

I passaggi principali per visualizzare in anteprima il file di estrazione sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Aggiungi profili di test]** per selezionare uno o più profili per visualizzare in anteprima i relativi dati nel contenuto del file di estrazione.

1. Nel riquadro a destra trovi un’anteprima del file di estrazione, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Inviare bozze {#test-dm}

Utilizzo di **Adobe Campaign**, puoi inviare le bozze prima di inviarle al pubblico principale. Questo passaggio è importante per convalidare la consegna e identificare eventuali problemi. I destinatari del test possono esaminare elementi quali le impostazioni di personalizzazione, garantendo prestazioni ottimali e rilevando eventuali errori. Questo processo ti aiuta a perfezionare e ottimizzare il file di estrazione prima di raggiungere il pubblico principale.

Per le consegne di direct mailing, l’invio di bozze genera un campione del file di estrazione utilizzando i dati dei profili di test selezionati. Per accedervi, effettua le seguenti operazioni:

1. Dalla schermata Simula contenuto, fai clic su **[!UICONTROL Invia bozza]** e segui gli stessi passaggi di qualsiasi tipo di consegna per inviare una bozza. [Scopri come inviare bozze](../preview-test/test-deliveries.md)

1. Una volta inviata la bozza, puoi accedervi dal **[!UICONTROL Visualizza bozze]** o dall’elenco delle consegne. [Scopri come accedere alle bozze inviate](../preview-test/test-deliveries.md#access-test-deliveries)

1. Nel dashboard della consegna delle bozze, fai clic su **[!UICONTROL Anteprima file]** per accedere a un’anteprima del file di estrazione.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Nel file di anteprima vengono visualizzate solo le prime 100 righe.

## Inviare la consegna direct mail {#send-dm}

Una volta che la direct mailing è pronta per essere inviata ai clienti, puoi inviare la consegna per avviare l’estrazione dei dati nel file di estrazione specificato. Per farlo, segui questi passaggi:

1. Dopo aver progettato il contenuto del file di estrazione, fai clic su **[!UICONTROL Rivedi e invia]** dal tuo **[!UICONTROL Consegna]** pagina.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano errori, fare riferimento a **[!UICONTROL Registri]** per informazioni dettagliate sull&#39;errore.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Per inviare i messaggi, fai clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

1. Conferma l’azione di invio facendo clic su **[!UICONTROL Invia]**.

   Se la consegna di direct mailing è stata pianificata, fai clic sul pulsante **[!UICONTROL Invia come pianificato]** pulsante. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).

Una volta inviata la consegna, il file di estrazione viene generato ed esportato automaticamente nella posizione specificata in **[!UICONTROL Indirizzamento]** account esterno selezionato nel modello di consegna [impostazioni avanzate](../advanced-settings/delivery-settings.md).

Puoi tenere traccia dei dati KPI (Key Performance Indicator) dalla pagina di consegna e dei dati da **[!UICONTROL Registri]** menu.

Puoi anche iniziare a misurare l’impatto del messaggio con i rapporti incorporati. [Ulteriori informazioni](../reporting/direct-mail.md)