---
audience: end-user
title: Utilizzare i servizi di abbonamento
description: Scopri come creare e gestire i servizi in Adobe Campaign Web
badge: label="Beta"
source-git-commit: 307d1e65850fcbdb51ca0016e4f3f30ca74997be
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Utilizzare i servizi di abbonamento {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Creare e gestire i servizi"
>abstract="Utilizza Adobe Campaign per creare e monitorare servizi come le newsletter e per verificare gli abbonamenti/annullamenti degli abbonamenti a tali servizi. Gli abbonamenti si applicano solo alla consegna di e-mail e SMS."

Utilizza il Web di Adobe Campaign per gestire e creare servizi come le newsletter e per verificare gli abbonamenti o i loro annullamenti.

>[!NOTE]
>
>Gli abbonamenti si applicano solo alla consegna di e-mail e SMS.

Diversi servizi possono essere definiti in parallelo, ad esempio: newsletter per specifiche categorie di prodotti, temi o aree di un sito web, abbonamenti a vari tipi di messaggi di avviso e notifiche in tempo reale.

Per ulteriori informazioni sulla gestione degli abbonamenti e sul loro annullamento, consulta [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Accedere ai servizi di abbonamento {#access-services}

Per accedere ai servizi di abbonamento disponibili per la tua piattaforma, passa a **[!UICONTROL Servizi di abbonamento]** menu nella barra di navigazione a sinistra.

![](assets/service-list.png)

Viene visualizzato l’elenco di tutti i servizi di abbonamento esistenti. Puoi cercare i servizi e filtrare in base al canale, alla cartella o utilizzare filtri avanzati.

![](assets/service-filters.png)

Per modificare un servizio esistente, fare clic sul relativo nome.

## Creare il primo servizio di abbonamento {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definire le proprietà del servizio"
>abstract="Inserisci l’etichetta del servizio di abbonamento e definisci le opzioni aggiuntive, ad esempio un periodo di validità per il servizio."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Seleziona un messaggio di conferma"
>abstract="Quando un utente si abbona o annulla l’abbonamento a un servizio, puoi inviare un messaggio di conferma. Seleziona i modelli da utilizzare per il messaggio."

Per creare un servizio di abbonamento, effettua le seguenti operazioni:

1. Seleziona la **[!UICONTROL Crea servizio di abbonamento]** pulsante.

   ![](assets/service-create-button.png)

1. Seleziona un canale: **[!UICONTROL E-mail]** o **[!UICONTROL SMS]**.

1. Nelle proprietà del servizio, immetti un’etichetta e definisci le opzioni aggiuntive in base alle tue esigenze.

   ![](assets/service-create-properties.png)

1. Per impostazione predefinita, gli abbonamenti sono illimitati. È possibile disattivare la **[!UICONTROL Periodo di validità illimitato]** per definire una durata di validità per il servizio. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. Quando un utente si abbona o annulla l’abbonamento a un servizio, puoi inviare un messaggio di conferma. Seleziona i modelli da utilizzare per quel messaggio in base al tuo caso d’uso.

   ![](assets/service-create-confirmation-msg.png)

1. Fai clic su **[!UICONTROL Salva]**. Il nuovo servizio viene aggiunto al **[!UICONTROL Servizi di abbonamento]** elenco.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


