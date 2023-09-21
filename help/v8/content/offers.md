---
audience: end-user
title: Aggiungere offerte ai messaggi
description: Scopri come aggiungere e inviare offerte
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 71%

---


# Aggiungere offerte ai messaggi {#offers-content}

Adobe Campaign Web v8 consente di inviare delle offerte di consegne create nella console mediante il modulo **[!UICONTROL Interazione]**. Per ulteriori informazioni sull’interazione e su come gestire un catalogo di offerte nella console, consulta [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=it){target="_blank"}.

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
>abstract="Puoi abilitare l’esclusione dei destinatari per i quali non vi sono sufficienti offerte idonee e scegliere la modalità di elaborazione del messaggio nel caso in cui una delle proposte non esista."

Adobe Campaign ti consente di proporre una o più offerte specifiche a un determinato contatto. Modulo di interazione che consente di rispondere in tempo reale durante un’interazione con un determinato contatto proponendo loro una o più offerte specifiche. Queste offerte possono essere semplici messaggi di comunicazione, offerte speciali su uno o più prodotti o un servizio.

Per selezionare le offerte da aggiungere alla consegna, segui i passaggi indicati di seguito.

1. Fai clic su **[!UICONTROL Configurare le offerte]** dalla schermata delivery content edition.

   ![](assets/setup-offers.png)

1. Configura le offerte da proporre ai destinatari.

   Seleziona prima lo **[!UICONTROL Spazio dell’offerta]** che corrisponde all’ambiente dell’offerta. Scopri come creare uno spazio delle offerte nel [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html?lang=it){target="_blank"}

   ![](assets/create-content-offers.png)

1. Per perfezionare le offerte scelte dal motore, seleziona la **[!UICONTROL Categoria offerta]** in base alla quale ordinare le offerte.

   Quando si seleziona una cartella, tutte le sottocartelle vengono incluse automaticamente e non possono essere rimosse. Tieni presente che l’interfaccia di [!DNL Campaign] non riflette questo comportamento.

   >[!NOTE]
   >
   >Se non viene specificata alcuna categoria, il motore di offerte prenderà in considerazione tutte le offerte contenute nell’ambiente, a meno che non venga selezionato un **[!UICONTROL Tema offerta]**.

1. (Facoltativo) Specifica un tema in base al quale filtrare le categorie. I temi sono parole chiave definite a monte nelle categorie. Fungono da filtro e consentono di perfezionare il numero di offerte da presentare selezionandole in un set di categorie.

1. Utilizza il campo **[!UICONTROL Proposte]** per specificare il numero di offerte da inserire nella consegna.

1. Se necessario, seleziona l’opzione **[!UICONTROL Escludi destinatari non idonei]**.

   Questa opzione consente di attivare o disattivare l’esclusione dei destinatari per i quali non sono disponibili sufficienti offerte idonee.

   * Se l’opzione è abilitata, i destinatari che non hanno abbastanza proposte vengono esclusi dalla consegna.
   * Se l’opzione è disabilitata, questi destinatari non vengono esclusi ma non possono disporre del numero di proposte richiesto.

1. Se necessario, seleziona l’opzione **[!UICONTROL Nascondi tutto se non è selezionata alcuna offerta]**.

   Questa opzione consente di scegliere come viene elaborato il messaggio nel caso in cui una delle proposte non esista.

   * Se l’opzione è abilitata, la rappresentazione della proposta mancante non viene visualizzata e nel messaggio per la proposta non viene visualizzato alcun contenuto.
   * Se l’opzione è disabilitata, il messaggio stesso viene annullato durante l’invio e i destinatari non possono più ricevere messaggi.

Dopo aver configurato le offerte da proporre nella consegna, puoi inserirle nel contenuto della consegna utilizzando l’editor espressioni.

## Inserire offerte nella consegna {#insert}

Le offerte possono essere aggiunte alla consegna utilizzando l’[Editor espressioni](../personalization/gs-personalization.md#access). Possono essere inserite nella riga dell’oggetto o nel corpo della consegna.

>[!CAUTION]
>
>Prima di inserire un’offerta in una consegna, assicurati di aver [configurato quale offerta proporre con tale consegna](#configure).

Per inserire un’offerta utilizzando l’editor di espressioni, effettua le seguenti operazioni.

1. Accedi all’oggetto o al contenuto di una consegna.

1. Posiziona il cursore nel punto in cui desideri inserire l’offerta e apri l’editor espressioni utilizzando l’icona di personalizzazione.

1. Seleziona il menu **[!UICONTROL Proposte]**. Le proposte disponibili vengono visualizzate nell’elenco.

   >[!NOTE]
   >
   >Il numero di proposte viene definito quando si [configurano le offerte](#configure) per la consegna corrente.

   ![](assets/offer-insertion.png)

1. Aggiungi le proposte all’oggetto o al corpo della consegna utilizzando i campi di personalizzazione, le funzioni di rendering o gli attributi dell’offerta disponibili per ogni proposta.

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >Il numero di proposte disponibili dipende dal modo in cui viene configurata la chiamata del motore e il loro ordine dipende dalla priorità delle offerte. Per ulteriori informazioni, consulta [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. Salva le modifiche.

1. Completa il contenuto, esegui un test e invia la consegna.

Ora, quando un destinatario riceve la consegna, viene visualizzata l’offerta giusta per quel profilo specifico.
