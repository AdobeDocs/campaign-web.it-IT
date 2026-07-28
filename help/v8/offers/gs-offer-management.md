---
audience: end-user
title: Introduzione alla gestione delle offerte
description: Scopri come gestire le offerte in Adobe Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 763
ht-degree: 4%

---

# Introduzione alla gestione delle offerte {#gs-offer-management}

Questa funzionalità ti consente di aggiungere offerte personalizzate alle consegne e di presentare quella più pertinente per ciascun profilo in un determinato contesto. Le offerte possono essere un semplice messaggio di comunicazione o promozioni su uno o più prodotti. In base alle regole di idoneità e ai pesi di priorità, il motore di offerta seleziona la proposta migliore da presentare.

L’interfaccia utente di Campaign Web consente di gestire le offerte in modalità end-to-end. Puoi creare e configurare ambienti di offerta, progettare spazi di offerta, creare il catalogo delle offerte, impostare le regole di idoneità, modificare il contenuto delle offerte e pubblicare le offerte.

Le offerte vengono quindi presentate ai destinatari tramite consegne basate su **regole di idoneità** e **pesi di priorità**, in modo che venga selezionata l&#39;offerta migliore per ogni profilo in un determinato contesto.

>[!NOTE]
>
>L’interfaccia utente di Campaign Web si concentra sull’utilizzo più comune di gestione delle offerte. Le configurazioni avanzate rimangono disponibili nella console client di Campaign. Consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=it){target="_blank"}

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## Concetti chiave {#concepts}

Prima di iniziare a lavorare con le offerte, acquisisci familiarità con gli oggetti principali coinvolti.

* **Ambiente offerte**: contenitore che contiene un catalogo delle offerte e i relativi spazi delle offerte. Esistono due tipi, l&#39;ambiente **Design**, in cui si creano e configurano le offerte, e quello di sola lettura **[!UICONTROL Live]**, che contiene gli oggetti approvati e distribuiti disponibili per la consegna. [Ulteriori informazioni](offer-environment.md)

* **Spazio dell&#39;offerta**: definisce dove e come viene esposta un&#39;offerta (e-mail, direct mailing, SMS, web in entrata, ecc.). Lo spazio elenca i campi di contenuto che possono essere utilizzati nell’offerta, la funzione di rendering che crea la rappresentazione dell’offerta e le impostazioni di archiviazione che determinano lo stato della proposta. [Ulteriori informazioni](offer-space.md)

* **Catalogo offerte e categorie** — Le offerte sono organizzate in un catalogo gerarchico di **categorie** e sottocategorie. Ogni categoria può condividere regole di idoneità, date di validità e **temi applicazione**. Nell&#39;ambiente di progettazione viene fornita una categoria predefinita per la ricezione di tutte le offerte.

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **Offerta**: una singola offerta con il proprio periodo di idoneità, filtro di destinazione, peso e contenuto. Le offerte vengono approvate e distribuite prima di poter essere presentate ai destinatari. [Ulteriori informazioni](create-offer.md)

* **Proposta di offerta**: risultato della presentazione di un&#39;offerta a un contatto in un determinato spazio (un banner in un sito Web, un&#39;e-mail, un SMS, ecc.). Il numero di proposte per consegna è configurato quando [si impostano le offerte in una consegna](../msg/offers.md).

* **Arbitraggio** — Principio in base al quale il motore di offerta classifica le offerte idonee in base alla priorità per selezionare quelle da presentare. L&#39;arbitraggio utilizza i criteri definiti sulle categorie, le offerte e le offerte contestuali.

## Flusso di gestione delle offerte {#workflow}

Il flusso end-to-end tipico nell’interfaccia utente di Campaign Web è il seguente:

1. **Verifica le impostazioni dell&#39;ambiente dell&#39;offerta** — Controlla le impostazioni di progettazione/mappatura live, idoneità e gestione del peso. [Ulteriori informazioni](offer-environment.md)

1. **Crea uno spazio dell&#39;offerta**: definisci i campi di contenuto, la funzione di rendering e i parametri avanzati che corrispondono al tuo canale. [Ulteriori informazioni](offer-space.md)

1. **Crea offerte nel catalogo**: imposta il periodo di idoneità, il filtro di destinazione, il peso e il contenuto di ogni offerta. [Ulteriori informazioni](create-offer.md)

1. **Approva e distribuisci**: invia l&#39;offerta per l&#39;approvazione, approvane il contenuto e l&#39;idoneità, quindi consenti al processo di distribuzione di pubblicarla nell&#39;ambiente live. [Ulteriori informazioni](create-offer.md#approve-deploy)

1. **Aggiungi l&#39;offerta a una consegna**. Fai riferimento allo spazio dell&#39;offerta e alle proposte nella consegna tramite e-mail, SMS, push o direct mailing. [Ulteriori informazioni](../msg/offers.md)

## Accedere alle offerte nell’interfaccia web {#access}

Le offerte sono disponibili dal menu a sinistra **[!UICONTROL Offerte]**. Da qui puoi sfogliare il catalogo, aprire un’offerta per l’edizione e monitorarne lo stato di approvazione e distribuzione.

![Schermata che mostra il menu Offerta.](assets/offers-gs.png){zoomable="yes"}

Gli ambienti delle offerte e gli spazi delle offerte sono accessibili tramite **[!UICONTROL Explorer]**, passando alla cartella corrispondente.


## Complementi solo console {#console-complements}

Alcune funzionalità di offerta non sono ancora esposte nell’interfaccia utente web e devono ancora essere configurate dalla console client:

* **Simulazione offerte**: il modulo **Simulazione** che consente di verificare la distribuzione delle offerte prima dell&#39;invio. Vedi [Simulazione offerte](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html#offer-simulation){target="_blank"}.

* Gestione di **Filtri predefiniti**: regole di filtro riutilizzabili a cui è possibile fare riferimento da qualsiasi offerta. Vedere [Gestire i filtri predefiniti](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}.

* **Tracciamento delle offerte**: configurazione del tracciamento per le proposte di offerta per alimentare la cronologia delle proposte. Consulta [Tracciare le proposte di offerta](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html){target="_blank"}.

* **Ruoli di operatore** — Assegnazione dei diritti di Gestione offerte/Responsabile della consegna. Consulta [Operatori del modulo di interazione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **Best practice di interazione e regole di arbitraggio**. Consulta [Best practice per l&#39;interazione con Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=it){target="_blank"}.

* **Generazione rapporti** — I rapporti di offerte e proposte dedicati non sono ancora disponibili nell&#39;interfaccia utente Web.