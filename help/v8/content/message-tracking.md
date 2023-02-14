---
audience: end-user
title: Tracciare i messaggi
description: Scopri come aggiungere collegamenti e tenere traccia dei messaggi inviati
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: ht
source-wordcount: '0'
ht-degree: 100%

---

# Aggiungere collegamenti e tenere traccia dei messaggi {#tracking}

![](../assets/do-not-localize/badge.png)

Utilizza E-mail Designer per aggiungere collegamenti al contenuto, quindi tieni traccia dei messaggi inviati per monitorare il comportamento dei destinatari.

## Inserire i collegamenti {#insert-links}

Durante la progettazione di un messaggio, puoi aggiungere collegamenti al contenuto.

>[!NOTE]
>
>Quando il tracciamento è abilitato, vengono tracciati tutti i collegamenti inclusi nel contenuto del messaggio.

Per inserire collegamenti nel contenuto delle e-mail, segui la procedura seguente:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** nella barra degli strumenti contestuale.

   ![](assets/message-tracking-insert-link.png)

1. Aggiungi un’**[!UICONTROL Etichetta]** e un **[!UICONTROL Collegamento]**.

1. Salva le modifiche.

1. Una volta creato il collegamento, puoi comunque modificarlo dal panello **[!UICONTROL Impostazioni componenti]** a destra.

   * Puoi modificare il collegamento e modificarne la relativa **[!UICONTROL Destinazione]**.
   * Puoi scegliere di sottolineare o meno il collegamento, selezionando l’opzione corrispondente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>I messaggi e-mail di tipo marketing devono includere un collegamento di rinuncia, che non è invece necessario per i messaggi transazionali. La categoria del messaggio (**[!UICONTROL Marketing]** o **[!UICONTROL Transazionale]**) viene definita a livello di superficie di canale (ad esempio, nel predefinito per messaggi) e durante la creazione del messaggio.

## Collegare a una pagina mirror {#mirror-page}

La pagina mirror è una pagina HTML accessibile online tramite un browser web. Il contenuto è identico a quello dell’e-mail.

Per aggiungere un collegamento a una pagina mirror nel messaggio e-mail:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** nella barra degli strumenti contestuale.

   ![](assets/message-tracking-mirror-page.png)

1. Seleziona l’icona **[!UICONTROL Inserisci collegamento]** per accedere al menu di personalizzazione.

   ![](assets/message-tracking-mirror-page_2.png)

1. Dal menu **[!UICONTROL Blocco di contenuto]**, seleziona **[!UICONTROL URL pagina mirror]** e fai clic su **[!UICONTROL Aggiungi]**.

   ![](assets/message-tracking-mirror-page_3.png)

La pagina mirror viene creata automaticamente.

>[!IMPORTANT]
>
>I collegamenti alle pagine mirror vengono generati automaticamente e non possono essere modificati. Contengono tutti i dati personalizzati crittografati necessari per eseguire il rendering dell’e-mail originale. Di conseguenza, l’utilizzo di attributi personalizzati con valori di grandi dimensioni può generare URL molto lunghi per le pagine mirror, che potrebbero non funzionare nei browser web in cui la lunghezza dell’URL è soggetta a un limite massimo.

Una volta inviata l’e-mail, quando i destinatari fanno clic sul collegamento della pagina mirror, il contenuto dell’e-mail viene visualizzato nel browser web predefinito.

>[!NOTE]
>
>Nell’e-mail di test inviata ai profili di test, il collegamento alla pagina mirror non è attivo. Viene attivato solo nei messaggi finali.

Il periodo di conservazione di una pagina mirror è di 60 giorni. Trascorso tale periodo, la pagina mirror non è più disponibile.

## Gestire il tracciamento {#manage-tracking}

[E-mail Designer](create-email-content.md) consente di gestire gli URL tracciati, ad esempio modificando il tipo di tracciamento per ogni collegamento.

1. Fai clic sull’icona **[!UICONTROL Collegamenti]** nel riquadro a sinistra per visualizzare l’elenco di tutti gli URL del contenuto da tracciare.

   Questo elenco consente di avere una visualizzazione centralizzata e di individuare ogni URL nel contenuto dell’e-mail.

1. Per modificare un collegamento, fai clic sull’icona a forma di matita corrispondente.

   ![](assets/message-tracking-edit-links.png)

1. Se necessario, puoi modificare il **[!UICONTROL Tipo di tracciamento]**:

   ![](assets/message-tracking-edit-a-link.png)

   Per ogni URL tracciato, puoi impostare la modalità di tracciamento su uno dei seguenti valori:

   * **[!UICONTROL Tracciato]**: attiva il tracciamento su questo URL.
   * **[!UICONTROL Rinuncia]**: considera questo URL come un URL di rinuncia o di annullamento dell’iscrizione.
   * **[!UICONTROL Pagina mirror]**: considera questo URL come un URL della pagina mirror.
   * **[!UICONTROL Mai]**: non attiva mai il tracciamento di questo URL.<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Aggiungi una **[!UICONTROL Categoria]** al collegamento per raggruppare i collegamenti tracciati e fai clic su **[!UICONTROL Salva]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Dopo aver inviato la consegna, accedi al rapporto di consegna. Nel menu **[!UICONTROL Tracciamento]**, il rapporto di **[!UICONTROL URL e flussi di clic]** mostra gli URL di consegna più visitati. [Ulteriori informazioni](../reporting/reports.md)
