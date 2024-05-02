---
audience: end-user
title: Tracciare i messaggi
description: Scopri come aggiungere collegamenti e tenere traccia dei messaggi inviati
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 66%

---

# Aggiungere collegamenti e tenere traccia dei messaggi {#tracking}

Utilizza E-mail Designer per aggiungere collegamenti al contenuto, quindi tieni traccia dei messaggi inviati per monitorare il comportamento dei destinatari.

## Inserire i collegamenti {#insert-links}

Durante la progettazione di un messaggio, puoi aggiungere collegamenti al contenuto.

>[!NOTE]
>
>Quando il tracciamento è abilitato, vengono tracciati tutti i collegamenti inclusi nel contenuto del messaggio.

Per inserire collegamenti nel contenuto delle e-mail, segui la procedura seguente:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** nella barra degli strumenti contestuale.

1. Scegli il tipo di collegamento da creare:

   ![](assets/message-tracking-insert-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Collegamento esterno]**: inserisci un collegamento a un URL esterno.

     >[!AVAILABILITY]
     >
     >Le seguenti funzionalità (collegamento a **[!UICONTROL Pagina di destinazione]**, **[!UICONTROL Collegamento di abbonamento]** e **[!UICONTROL Collegamento per annullare l’iscrizione]**) sono in Disponibilità limitata (LA). Sono limitati ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

   * **[!UICONTROL Pagina di destinazione]**: inserisci un collegamento a una pagina di destinazione. Se selezioni una pagina di destinazione dinamica (con **[!UICONTROL Servizio da URL]** selezionato), è possibile selezionare qualsiasi servizio dall’elenco. [Ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Collegamento di abbonamento]**: inserisci un collegamento a un servizio di abbonamento. Quando gli utenti fanno clic sul collegamento, verranno indirizzati alla pagina di destinazione dell’abbonamento a cui si fa riferimento nel servizio selezionato. [Ulteriori informazioni](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Collegamento per annullare l’iscrizione]**: inserisci un collegamento a un servizio di annullamento dell’abbonamento. Quando gli abbonati fanno clic sul collegamento, verranno indirizzati alla pagina di destinazione per l’annullamento dell’abbonamento a cui si fa riferimento nel servizio selezionato. [Ulteriori informazioni](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Inserisci l’URL desiderato nel campo corrispondente, oppure seleziona una pagina di destinazione o un servizio, e definisci le impostazioni e gli stili del collegamento.

1. Aggiungi un’**[!UICONTROL Etichetta]** e un **[!UICONTROL Collegamento]**.

1. Salva le modifiche.

1. Una volta creato il collegamento, puoi comunque modificarlo dalla scheda **[!UICONTROL Impostazioni]**.

   * Puoi modificare il collegamento e modificarne la relativa **[!UICONTROL Destinazione]**.
   * Puoi scegliere di sottolineare o meno il collegamento, selezionando l’opzione corrispondente.

   ![](assets/message-tracking-link-settings.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>I messaggi e-mail di tipo marketing devono includere un collegamento di rinuncia, che non è invece necessario per i messaggi transazionali. La categoria del messaggio (**[!UICONTROL Marketing]** o **[!UICONTROL Transazionale]**) viene definito a livello della superficie di canale e durante la creazione del messaggio.

In tutti i messaggi e-mail deve essere aggiunto un collegamento specifico alla pagina mirror. Ulteriori informazioni sulla pagina mirror in [questa sezione](mirror-page.md).

## Gestire il tracciamento {#manage-tracking}

[E-mail Designer](create-email-content.md) consente di gestire gli URL tracciati, ad esempio modificando il tipo di tracciamento per ogni collegamento.

1. Fai clic sull’icona **[!UICONTROL Collegamenti]** nel riquadro a sinistra per visualizzare l’elenco di tutti gli URL del contenuto da tracciare.

   Questo elenco consente di avere una visualizzazione centralizzata e di individuare ogni URL nel contenuto dell’e-mail.

1. Per modificare un collegamento, fai clic sull’icona a forma di matita corrispondente.

   ![](assets/message-tracking-edit-links.png){zoomable=&quot;yes&quot;}

1. Se necessario, puoi modificare il **[!UICONTROL Tipo di tracciamento]**:

   ![](assets/message-tracking-edit-a-link.png){zoomable=&quot;yes&quot;}

   Per ogni URL tracciato, puoi impostare la modalità di tracciamento su uno dei seguenti valori:

   * **[!UICONTROL Tracciato]**: attiva il tracciamento su questo URL.
   * **[!UICONTROL Rinuncia]**: considera questo URL come un URL di rinuncia o di annullamento dell’iscrizione.
   * **[!UICONTROL Pagina mirror]**: considera questo URL come un URL della pagina mirror.
   * **[!UICONTROL Mai]**: non attiva mai il tracciamento di questo URL.<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Aggiungi una **[!UICONTROL Categoria]** al collegamento per raggruppare i collegamenti tracciati e fai clic su **[!UICONTROL Salva]**.

   ![](assets/message-tracking-edit-a-link_2.png){zoomable=&quot;yes&quot;}

1. Dopo aver inviato la consegna, accedi al rapporto di consegna. Nel menu **[!UICONTROL Tracciamento]**, il rapporto di **[!UICONTROL URL e flussi di clic]** mostra gli URL di consegna più visitati. [Ulteriori informazioni](../reporting/gs-reports.md)
