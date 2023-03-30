---
audience: end-user
title: Aggiungere un collegamento alla pagina speculare
description: Scopri come aggiungere e gestire il collegamento alla pagina speculare
source-git-commit: b85bf75da466502e4579a061c02a2c4ce4361cd5
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 37%

---


# Aggiungere un collegamento alla pagina speculare{#mirror-page}

## Informazioni sulla pagina speculare{#about-mirror-page}

La pagina speculare è una versione online della tua e-mail.

Mentre la maggior parte dei client e-mail esegue il rendering delle immagini senza alcun problema, alcuni predefiniti possono evitare la visualizzazione delle immagini per motivi di sicurezza. Gli utenti possono passare alla pagina speculare di un’e-mail, ad esempio se riscontrano problemi di rendering o immagini interrotte quando tentano di visualizzarla nella casella in entrata. Si consiglia inoltre di fornire una versione online per motivi di accessibilità o di incoraggiare la condivisione social network.

La pagina speculare generata da Adobe Campaign contiene tutti i dati di personalizzazione.

![campione di collegamento a specchio](assets/mirror-page-link.png){width="600" align="left"}

## Aggiungere un collegamento alla pagina speculare{#link-to-mirror-page}

È buona prassi inserire un collegamento alla pagina speculare. Questo link può essere ad esempio &#39;Visualizza questa e-mail nel tuo browser&#39; o &#39;Leggi questo online&#39;. Spesso si trova nell’intestazione o nel piè di pagina dell’e-mail.

In Adobe Campaign, puoi inserire un collegamento alla pagina speculare nel contenuto dell’e-mail utilizzando l’ **blocco di personalizzazione**. Incorporato **Collegamento a una pagina speculare** nel contenuto dell’e-mail viene inserito il seguente codice: `<%@ include view='MirrorPage' %>`.


Per aggiungere un collegamento a una pagina mirror nel messaggio e-mail:

1. Seleziona un elemento e fai clic su **[!UICONTROL Inserisci collegamento]** nella barra degli strumenti contestuale.

   ![](assets/message-tracking-mirror-page.png)

1. Seleziona l’icona **[!UICONTROL Inserisci collegamento]** per accedere al menu di personalizzazione.

   ![](assets/message-tracking-mirror-page_2.png)

1. Dal menu **[!UICONTROL Blocco di contenuto]**, seleziona **[!UICONTROL URL pagina mirror]** e fai clic su **[!UICONTROL Aggiungi]**.

   ![](assets/message-tracking-mirror-page_3.png)

   Per ulteriori informazioni sull’inserimento di blocchi di contenuto personalizzati, consulta [questa sezione](../personalization/personalize.md#personalize-emails).

La pagina mirror viene creata automaticamente.

>[!IMPORTANT]
>
>I collegamenti alle pagine mirror vengono generati automaticamente e non possono essere modificati. Contengono tutti i dati personalizzati crittografati necessari per eseguire il rendering dell’e-mail originale. Di conseguenza, l’utilizzo di attributi personalizzati con valori di grandi dimensioni può generare URL molto lunghi per le pagine mirror, che potrebbero non funzionare nei browser web in cui la lunghezza dell’URL è soggetta a un limite massimo.

Una volta inviata l’e-mail, quando i destinatari fanno clic sul collegamento della pagina mirror, il contenuto dell’e-mail viene visualizzato nel browser web predefinito.

>[!NOTE]
>
>Nell’e-mail di test inviata ai profili di test, il collegamento alla pagina mirror non è attivo. Viene attivato solo nei messaggi finali.

Per impostazione predefinita, il periodo di conservazione per una pagina speculare è di 60 giorni. Trascorso tale periodo, la pagina mirror non è più disponibile.


## Generazione di pagine mirror{#mirror-page-generation}

Per impostazione predefinita, la pagina speculare viene generata automaticamente da Adobe Campaign se il contenuto dell’e-mail non è vuoto e se contiene un collegamento alla pagina speculare (aka Mirror link).

Puoi controllare la modalità di generazione della pagina speculare e-mail. Le opzioni sono disponibili nelle proprietà di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#mirror)
