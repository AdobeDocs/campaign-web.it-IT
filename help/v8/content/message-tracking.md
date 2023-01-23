---
audience: end-user
title: Tracciare i messaggi
description: Scopri come aggiungere collegamenti e tenere traccia dei messaggi inviati
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# Aggiungere collegamenti e tenere traccia dei messaggi {#tracking}

![](../assets/do-not-localize/badge.png)

Utilizza E-mail designer per aggiungere collegamenti al contenuto e tenere traccia dei messaggi inviati per monitorare il comportamento dei destinatari.

## Inserisci collegamenti {#insert-links}

Durante la progettazione di un messaggio, puoi aggiungere collegamenti al contenuto.

>[!NOTE]
>
>Quando il tracciamento è abilitato, vengono tracciati tutti i collegamenti inclusi nel contenuto del messaggio.

Per inserire collegamenti nel contenuto delle e-mail, segui la procedura seguente:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** dalla barra degli strumenti contestuale.

   ![](assets/message-tracking-insert-link.png)

1. Aggiungi un **[!UICONTROL Etichetta]** e **[!UICONTROL Collegamento]**.

1. Salva le modifiche.

1. Una volta creato il collegamento, puoi comunque modificarlo dal **[!UICONTROL Impostazioni dei componenti]** a destra.

   * Puoi modificare il collegamento e modificarne le relative **[!UICONTROL Target]**.
   * Puoi scegliere di sottolineare il collegamento o meno selezionando l’opzione corrispondente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>I messaggi e-mail di tipo marketing devono includere un collegamento di rinuncia, che non è necessario per i messaggi transazionali. La categoria del messaggio (**[!UICONTROL Marketing]** o **[!UICONTROL Transazionale]**) viene definita a livello della superficie del canale (ad es. predefinito per messaggi) e durante la creazione del messaggio.

## Collegamento a una pagina speculare {#mirror-page}

La pagina speculare è una pagina HTML accessibile online tramite un browser web. Il contenuto è identico a quello dell’e-mail.

Per aggiungere un collegamento a una pagina speculare nel messaggio e-mail:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** dalla barra degli strumenti contestuale.

   ![](assets/message-tracking-mirror-page.png)

1. Seleziona la **[!UICONTROL Inserisci collegamento]** per accedere al menu di personalizzazione.

   ![](assets/message-tracking-mirror-page_2.png)

1. Da **[!UICONTROL Blocco del contenuto]** menu, seleziona **[!UICONTROL URL pagina speculare]** e fai clic su **[!UICONTROL Aggiungi]**.

   ![](assets/message-tracking-mirror-page_3.png)

La pagina speculare viene creata automaticamente.

>[!IMPORTANT]
>
>I collegamenti alle pagine mirror vengono generati automaticamente e non possono essere modificati. Contengono tutti i dati personalizzati crittografati necessari per eseguire il rendering dell’e-mail originale. Di conseguenza, l’utilizzo di attributi personalizzati con valori di grandi dimensioni può generare URL per pagine mirror lunghe, il che può impedire il funzionamento del collegamento nei browser web con una lunghezza massima di URL.

Una volta inviata l’e-mail, quando i destinatari fanno clic sul collegamento della pagina speculare, il contenuto dell’e-mail viene visualizzato nel browser Web predefinito.

>[!NOTE]
>
>Nell’e-mail di test inviata ai profili di test, il collegamento alla pagina speculare non è attivo. Viene attivato solo nei messaggi finali.

Il periodo di conservazione per una pagina speculare è di 60 giorni. Dopo tale ritardo, la pagina speculare non è più disponibile.

## Gestire il tracciamento {#manage-tracking}

La [E-mail Designer](create-email-content.md) consente di gestire gli URL tracciati, ad esempio modificando il tipo di tracciamento per ogni collegamento.

1. Fai clic sul pulsante **[!UICONTROL Collegamenti]** per visualizzare l’elenco di tutti gli URL del contenuto da tracciare.

   Questo elenco consente di avere una visualizzazione centralizzata e di individuare ogni URL nel contenuto dell’e-mail.

1. Per modificare un collegamento, fai clic sull’icona a forma di matita corrispondente.

   ![](assets/message-tracking-edit-links.png)

1. Puoi modificare la **[!UICONTROL Tipo di tracciamento]** se necessario:

   ![](assets/message-tracking-edit-a-link.png)

   Per ogni URL tracciato, puoi impostare la modalità di tracciamento su uno dei seguenti valori:

   * **[!UICONTROL Tracciato]**: Attiva il tracciamento su questo URL.
   * **[!UICONTROL Rinuncia]**: Considera questo URL come un URL di rinuncia o di annullamento dell’abbonamento.
   * **[!UICONTROL Pagina speculare]**: Considera questo URL come un URL della pagina speculare.
   * **[!UICONTROL Mai]**: Non attiva mai il tracciamento di questo URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Aggiungi un **[!UICONTROL Categoria]** al collegamento per raggruppare i collegamenti tracciati e fai clic su **[!UICONTROL Salva]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Dopo aver inviato la consegna, accedi al rapporto di consegna. Sotto la **[!UICONTROL Tracking]** il menu **[!UICONTROL URL e flussi di clic]** nel rapporto vengono visualizzati gli URL della consegna più visitati. [Ulteriori informazioni](../reporting/reports.md)
