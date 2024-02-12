---
audience: end-user
title: Aggiungere offerte ai messaggi
description: Scopri come aggiungere e inviare offerte
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 66%

---


# Aggiungere offerte ai messaggi {#offers-content}

Puoi aggiungere offerte alle consegne nell’interfaccia utente web di Adobe Campaign. Queste offerte sono disponibili nella **Offerte** menu a sinistra che consente di accedere all’elenco delle offerte. Tutte queste offerte sono di sola lettura e devono essere state create nella console client di Campaign utilizzando **[!UICONTROL Interazione]** modulo. Per ulteriori informazioni su Interazione e su come gestire un catalogo di offerte nella console, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=it){target="_blank"}.


I passaggi per inviare offerte con una consegna sono i seguenti:

1. [Configurare le offerte da proporre](#configure)
1. [Inserire le offerte nella consegna](#insert)

## Configurare le offerte da proporre {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Definire i parametri delle offerte"
>abstract="Configura le offerte da proporre ai destinatari definendo uno spazio delle offerte, facoltativamente una categoria e un tema, e specifica il numero di offerte da inserire nella consegna."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Impostare le impostazioni avanzate delle offerte"
>abstract="Puoi abilitare l’esclusione dei destinatari per i quali non vi sono sufficienti offerte idonee e scegliere come verrà elaborato il messaggio nel caso in cui una delle proposte non esista."

Adobe Campaign ti consente di rispondere in tempo reale durante un’interazione con un determinato contatto proponendo loro una o più offerte specifiche. Queste offerte possono essere semplici messaggi di comunicazione, offerte speciali su uno o più prodotti o un servizio.

Per selezionare le offerte da aggiungere alla consegna, segui i passaggi indicati di seguito.

1. Fai clic su **[!UICONTROL Configura le offerte]** dalla schermata di modifica del contenuto della consegna.

   ![](assets/offer-setup.png){zoomable=&quot;yes&quot;}

1. Configura le offerte da proporre ai destinatari.

   Seleziona prima lo **[!UICONTROL Spazio dell’offerta]** che corrisponde all’ambiente dell’offerta. Scopri come creare uno spazio delle offerte nel [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html?lang=it){target="_blank"}.

   ![](assets/offer-create-content.png){zoomable=&quot;yes&quot;}

1. Per perfezionare le offerte scelte dal motore, seleziona la **[!UICONTROL Categoria offerta]** in base alla quale ordinare le offerte.

   Quando si seleziona una cartella, tutte le sottocartelle vengono incluse automaticamente e non possono essere rimosse. Tieni presente che l’interfaccia di [!DNL Campaign] non riflette questo comportamento.

   >[!NOTE]
   >
   >Se non viene specificata alcuna categoria, il motore di offerte prenderà in considerazione tutte le offerte contenute nell’ambiente, a meno che non venga selezionato un **[!UICONTROL Tema offerta]**.

1. (Facoltativo) Specifica un tema in base al quale filtrare le categorie. I temi sono parole chiave definite a monte nelle categorie. Fungono da filtro e consentono di perfezionare il numero di offerte da presentare selezionandole in un set di categorie.

1. Utilizza il campo **[!UICONTROL Proposte]** per specificare il numero di offerte da inserire nella consegna.

1. Se necessario, seleziona l’opzione **[!UICONTROL Escludi destinatari non idonei]**.

   Questa opzione consente di attivare o disattivare l’esclusione dei destinatari per i quali non vi sono sufficienti offerte idonee:

   * Se l’opzione è abilitata, i destinatari che non hanno abbastanza proposte vengono esclusi dalla consegna.
   * Se l’opzione è disabilitata, questi destinatari non vengono esclusi ma non possono disporre del numero di proposte richiesto.

1. Se necessario, seleziona l’opzione **[!UICONTROL Nascondi tutto se non è selezionata alcuna offerta]**.

   Questa opzione consente di scegliere la modalità di elaborazione del messaggio nel caso in cui una delle proposte non esista:

   * Se l’opzione è abilitata, la rappresentazione della proposta mancante non viene visualizzata e nel messaggio per la proposta non viene visualizzato alcun contenuto.
   * Se l’opzione è disabilitata, il messaggio stesso viene annullato durante l’invio e i destinatari non possono più ricevere messaggi.

Dopo aver configurato le offerte da proporre nella consegna, puoi inserirle nel contenuto della consegna.

## Inserire offerte nella consegna {#insert}

Le offerte possono essere aggiunte alla consegna utilizzando [editor di espressioni](../personalization/gs-personalization.md#access). Possono essere inserite nella riga dell’oggetto o nel corpo della consegna.

>[!CAUTION]
>
>Prima di inserire un’offerta in una consegna, assicurati di aver [configurato quale offerta proporre con tale consegna](#configure).

Per inserire un’offerta tramite l’editor di espressioni, segui la procedura riportata di seguito.

1. Accedi all’oggetto o al contenuto di una consegna.

1. Posiziona il cursore del mouse nel punto in cui desideri inserire l’offerta e apri l’editor di espressioni utilizzando l’icona di personalizzazione.

   ![](assets/offer-insert-perso-icon.png){zoomable=&quot;yes&quot;}

1. Seleziona il menu **[!UICONTROL Proposte]**. Le proposte disponibili vengono visualizzate nell’elenco.

   >[!NOTE]
   >
   >Il numero di proposte viene definito quando si [configurano le offerte](#configure) per la consegna corrente.

1. Definisci ogni proposta utilizzando i campi di personalizzazione, le funzioni di rendering o gli attributi di offerta disponibili.

   ![](assets/offer-inserted.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Il numero di proposte disponibili dipende dal modo in cui viene configurata la chiamata del motore e il loro ordine dipende dalla priorità delle offerte. Per ulteriori informazioni, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=it){target="_blank"}.

1. Salva le modifiche.

1. Completa il contenuto, verifica e invia la consegna. [Ulteriori informazioni](gs-messages.md)

Ora, quando un destinatario riceve la consegna, viene visualizzata l’offerta giusta per quel profilo specifico.
