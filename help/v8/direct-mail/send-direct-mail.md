---
audience: end-user
title: Anteprima e invio di una consegna direct mailing
description: Scopri come visualizzare in anteprima e inviare una consegna di direct mailing con Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 13%

---

# Anteprima e invio di una consegna direct mailing {#send-direct-mail}

Dopo aver configurato il file di estrazione per la consegna di direct mailing, puoi utilizzare i profili di test per visualizzarlo in anteprima. Se hai incluso contenuti personalizzati, puoi esaminare come questi contenuti vengono visualizzati nelle colonne utilizzando i dati del profilo di test. Ciò ti consente di garantire che il contenuto del file venga riprodotto correttamente e che gli elementi personalizzati vengano incorporati in modo appropriato.

Quando il file di estrazione è pronto, puoi inviare la consegna di direct mailing per generare il file e condividerlo con il provider di direct mailing. [Scopri come inviare la consegna direct mailing](#dm-send)

## Anteprima del file di estrazione {#preview-dm}

I passaggi principali per visualizzare in anteprima il file di estrazione sono i seguenti. Per ulteriori dettagli su come visualizzare in anteprima le consegne, consulta [questa sezione](../preview-test/preview-content.md).

1. Dalla pagina dei contenuti della consegna, puoi utilizzare **[!UICONTROL Simula contenuto]** per visualizzare in anteprima i contenuti personalizzati.

   ![](assets/dm-simulate.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi profili di test]** per selezionare uno o più profili con cui visualizzare l&#39;anteprima dei dati nel contenuto del file di estrazione.

1. Nel riquadro a destra trovi un’anteprima del file di estrazione, in cui gli elementi personalizzati vengono sostituiti dinamicamente con i dati del profilo selezionato.

   ![](assets/dm-preview-right.png){zoomable="yes"}

## Inviare bozze {#test-dm}

Utilizzando **Adobe Campaign**, puoi inviare bozze prima di inviarle al pubblico principale. Questo passaggio è importante per convalidare la consegna e identificare eventuali problemi. I destinatari del test possono esaminare elementi quali le impostazioni di personalizzazione, garantendo prestazioni ottimali e rilevando eventuali errori. Questo processo ti aiuta a perfezionare e ottimizzare il file di estrazione prima di raggiungere il pubblico principale.

Per le consegne di direct mailing, l’invio di bozze genera un campione del file di estrazione utilizzando i dati dei profili di test selezionati. Per accedervi, effettua le seguenti operazioni:

1. Dalla schermata Simula contenuto, fai clic sul pulsante **[!UICONTROL Invia bozza]** e segui gli stessi passaggi di qualsiasi tipo di consegna per inviare una bozza. [Scopri come inviare bozze](../preview-test/test-deliveries.md)

1. Una volta inviata la bozza, puoi accedervi dal pulsante **[!UICONTROL Visualizza bozze]** o dall&#39;elenco delle consegne. [Scopri come accedere alle bozze inviate](../preview-test/test-deliveries.md#access-test-deliveries)

1. Nel dashboard di consegna delle bozze, fai clic sul pulsante **[!UICONTROL Anteprima file]** per accedere all&#39;anteprima del file di estrazione.

   ![](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >Nel file di anteprima vengono visualizzate solo le prime 100 righe.

## Inviare la consegna direct mail {#send-dm}

Una volta che la direct mailing è pronta per essere inviata ai clienti, puoi inviare la consegna per avviare l’estrazione dei dati nel file di estrazione specificato. Per farlo, segui questi passaggi:

1. Dopo aver progettato il contenuto del file di estrazione, fai clic su **[!UICONTROL Rivedi e invia]** dalla pagina **[!UICONTROL Consegna]**.

   ![](assets/dm-review-send.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Prepara]** e monitora l’avanzamento e le statistiche fornite.

   Se si verificano errori, fare riferimento al menu **[!UICONTROL Registri]** per informazioni dettagliate sull&#39;errore.

   ![](assets/dm-prepare.png){zoomable="yes"}

1. Per inviare i messaggi, fai clic su **[!UICONTROL Invia]** per procedere con il processo di invio finale.

1. Conferma l’azione di invio facendo clic su **[!UICONTROL Invia]**.

   Se la consegna direct mailing è stata pianificata, fare clic sul pulsante **[!UICONTROL Invia come pianificato]**. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#schedule-the-delivery-sending).

Una volta inviata la consegna, il file di estrazione viene generato ed esportato automaticamente nella posizione specificata nell&#39;account esterno **[!UICONTROL Routing]** selezionato nelle [impostazioni avanzate](../advanced-settings/delivery-settings.md) del modello di consegna.

Puoi tenere traccia dei dati KPI (Key Performance Indicator) dalla pagina di consegna e dei dati dal menu **[!UICONTROL Registri]**.

Puoi anche iniziare a misurare l’impatto del messaggio con i rapporti incorporati. [Ulteriori informazioni](../reporting/direct-mail.md)
