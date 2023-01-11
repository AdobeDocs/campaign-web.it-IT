---
audience: end-user
title: Inviare offerte
description: Inviare offerte
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Inviare offerte {#offers-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Impostazioni delle offerte"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Offre impostazioni avanzate"
>abstract="TBC"

Adobe Campaign v8 Web consente di inviare con le offerte e-mail create nella console utilizzando **[!UICONTROL Interazione]** modulo . Per ulteriori informazioni sull’interazione e su come gestire un catalogo di offerte nella console, consulta [Documentazione di Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html)

I passaggi per inviare offerte con un’e-mail sono i seguenti:

1. [Configurare le offerte da proporre](#configure),
1. [Inserisci le offerte nell’e-mail](#insert).

## Configurare le offerte da proporre {#configure}

Per selezionare le offerte da proporre nel messaggio e-mail, fai clic sul pulsante **[!UICONTROL Offerte]** dalla schermata dell’edizione del contenuto dell’e-mail, quindi configura le offerte da proporre.

![](assets/create-content-offers.png)

1. Seleziona la **[!UICONTROL Spazio offerta]** che corrisponde all’ambiente dell’offerta.

1. Per perfezionare la scelta delle offerte del motore, seleziona una **[!UICONTROL Categoria di offerta]** in cui vengono ordinate le offerte.

   Se non viene specificata alcuna categoria, tutte le offerte contenute nell’ambiente verranno prese in considerazione dal motore di offerta, a meno che un **[!UICONTROL Tema offerta]** è selezionato.

   >[!NOTE]
   >
   >I temi sono parole chiave definite a monte nelle categorie. Fungono da filtro e consentono di perfezionare il numero di offerte da presentare selezionandole in un set di categorie.

1. Utilizza la **[!UICONTROL Proposte]** per specificare il numero di offerte da inserire nell’e-mail.

1. Seleziona la **[!UICONTROL Escludere i destinatari non idonei]** se necessario.

   Questa opzione ti consente di attivare o disattivare l’esclusione dei destinatari per i quali non sono disponibili sufficienti offerte idonee.

   * Se l’opzione è abilitata, i destinatari che non hanno abbastanza proposte verranno esclusi dalla consegna.
   * Se l’opzione è disabilitata, questi destinatari non verranno esclusi ma non avranno il numero di proposte richiesto.

1. Se necessario, seleziona la **[!UICONTROL Nascondi tutto se non è selezionata alcuna offerta]** opzione .

   Questa opzione ti consente di scegliere come verrà elaborato il messaggio nel caso in cui una delle proposte non esista.

   * Se l’opzione è abilitata, la rappresentazione della proposta mancante non viene visualizzata e nel messaggio per la proposta non verrà visualizzato alcun contenuto.
   * Se l’opzione è disabilitata, il messaggio stesso viene annullato durante l’invio e i destinatari non riceveranno più alcun messaggio.

Dopo aver configurato le offerte da proporre nell’e-mail, puoi inserirle nell’e-mail utilizzando l’editor espressioni. [Scopri come inserire offerte nell’e-mail](#insert)

## Inserire offerte nell’e-mail {#insert}

Le offerte vengono aggiunte a un’e-mail tramite l’editor espressioni. Possono essere inseriti:

* nella riga dell’oggetto dell’e-mail,
* nel corpo dell’e-mail consentendo la personalizzazione in qualsiasi componente di contenuto. [Scopri come aggiungere componenti di contenuto](content-components.md)

>[!NOTE]
>
>Prima di inserire un’offerta, assicurati di [configurato quali offerte proporre con l’e-mail](#configure).

Per inserire un’offerta utilizzando l’editor espressioni, effettua le seguenti operazioni:

1. Apri l’Editor espressioni, quindi seleziona la **[!UICONTROL Proposte]** menu.

   Le proposte disponibili vengono visualizzate nell’elenco. Il numero di proposte viene definito durante la configurazione delle offerte da proporre.

   ![](assets/offer-insertion.png)

1. Aggiungi le proposte all’oggetto o al corpo dell’e-mail utilizzando i campi di personalizzazione, le funzioni di rendering o gli attributi dell’offerta disponibili per ogni proposta.

   ![](assets/offer-inserted.png)
