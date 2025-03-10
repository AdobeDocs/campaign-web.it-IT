---
audience: end-user
title: Aggiungere un collegamento alla pagina mirror
description: Scopri come aggiungere e gestire il collegamento alla pagina mirror
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 73%

---

# Pagina mirror {#mirror-page}

La pagina speculare è una versione online dell’e-mail. L’aggiunta di un collegamento alla pagina speculare rappresenta una buona pratica di e-mail marketing. Gli utenti possono passare alla pagina mirror di un’e-mail, ad esempio se riscontrano problemi di rendering o immagini interrotte quando tentano di visualizzarla nella casella in entrata. Si consiglia inoltre di fornire una versione online per motivi di accessibilità o di incoraggiare la condivisione social.

La pagina mirror generata da Adobe Campaign contiene tutti i dati di personalizzazione.

![esempio di collegamento mirror](assets/mirror-page-link.png){width="600" align="left"}

## Aggiungere un collegamento alla pagina mirror{#link-to-mirror-page}

In Adobe Campaign, puoi inserire un collegamento alla pagina mirror nel contenuto dell’e-mail utilizzando il **blocco di personalizzazione** dedicato. Il blocco di personalizzazione incorporato **Collegamento a una pagina mirror** inserisce il seguente codice nel contenuto dell’e-mail: `<%@ include view='MirrorPage' %>`.

Per aggiungere un collegamento a una pagina speculare nell’e-mail, effettua le seguenti operazioni:

1. Selezionare un elemento (testo o immagine) e fare clic su **[!UICONTROL Inserisci collegamento]** nella barra degli strumenti contestuale.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Seleziona l’icona **[!UICONTROL Aggiungi personalizzazione]** per accedere al menu di personalizzazione.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Dal menu **[!UICONTROL Frammenti]**, seleziona **[!UICONTROL URL pagina mirror]** e fai clic su **[!UICONTROL Aggiungi]**. [Scopri come utilizzare i frammenti di espressione](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

La pagina mirror viene creata automaticamente.

Una volta inviata l’e-mail, quando i destinatari fanno clic sul collegamento della pagina mirror, il contenuto dell’e-mail viene visualizzato nel browser web predefinito.

Per impostazione predefinita, il periodo di conservazione per una pagina mirror è di **60 giorni**. Trascorso tale periodo, la pagina mirror non è più disponibile.

>[!CAUTION]
>
>* I collegamenti alle pagine mirror vengono generati automaticamente e non possono essere modificati. Contengono tutti i dati personalizzati crittografati necessari per eseguire il rendering dell’e-mail originale. Di conseguenza, l’utilizzo di attributi personalizzati con valori di grandi dimensioni può generare URL molto lunghi per le pagine mirror, che potrebbero non funzionare nei browser web in cui la lunghezza dell’URL è soggetta a un limite massimo.
>
>* Nella bozza inviata ai profili di test, il collegamento alla pagina speculare non è attivo. È attivo solo nei messaggi finali.


## Generazione di pagine mirror {#mirror-page-generation}

Per impostazione predefinita, la pagina mirror viene generata automaticamente da Adobe Campaign se il contenuto dell’e-mail non è vuoto e se contiene un collegamento alla pagina mirror (detto anche collegamento mirror).

Puoi controllare la modalità di generazione della pagina mirror dell’e-mail. Le opzioni sono disponibili nelle proprietà di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#mirror)
