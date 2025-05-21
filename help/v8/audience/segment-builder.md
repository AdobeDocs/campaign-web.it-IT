---
audience: end-user
title: Creare un pubblico con il generatore di regole di Campaign
description: Scopri come utilizzare il generatore di regole
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 28%

---

# Utilizzare il generatore di regole {#segment-builder}

Il generatore di regole ti consente di definire la popolazione target della consegna filtrando i dati contenuti nel database. Puoi utilizzarlo per creare un pubblico da un flusso di lavoro utilizzando un&#39;attività **[!UICONTROL Genera pubblico]** oppure direttamente durante la creazione di una consegna per creare un pubblico una tantum.

* [Scopri come creare e salvare un pubblico](create-audience.md)
* [Scopri come creare un pubblico una tantum per una consegna](one-time-audience.md)

## La palette

La palette, che si trova sul lato sinistro, contiene tutti gli elementi su cui puoi filtrare per creare il pubblico. Utilizza la barra di ricerca per trovare rapidamente gli elementi. Sposta le tessere contenute nella palette nell’area di lavoro centrale per configurarle e tenerne conto.

![Interfaccia della tavolozza con opzioni e schede di filtro](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

La palette è divisa in due schede:

* **Attributi**: questa scheda consente di accedere a tutti i campi disponibili dello schema. L’elenco dei campi dipende dallo schema di targeting definito nel modello e-mail.

* **Tipi di pubblico**: questa scheda ti consente di filtrare utilizzando uno dei tipi di pubblico esistenti definiti nella console Campaign Classic o da Adobe Experience Platform. Scopri come monitorare e gestire il pubblico in [questa sezione](manage-audience.md).

  >[!NOTE]
  >
  >Per utilizzare i tipi di pubblico di Adobe Experience Platform, configura l’integrazione con Destinazioni. Consulta la [documentazione sulle destinazioni Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=it){target="_blank"}.

## L’area di lavoro

L’area di lavoro è l’area centrale in cui puoi configurare e combinare le regole in base agli elementi aggiunti dalla palette. Per aggiungere una nuova regola, trascina una sezione dalla palette e rilasciala nell’area di lavoro. Le opzioni specifiche del contesto vengono presentate in base al tipo di dati aggiunti.

![L&#39;interfaccia dell&#39;area di lavoro mostra le opzioni di configurazione delle regole](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## Il riquadro delle proprietà delle regole

Sul lato destro, il riquadro **Proprietà regola** consente di eseguire le azioni elencate di seguito.

![Il riquadro delle proprietà delle regole mostra le azioni disponibili](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Visualizza risultati:** Visualizza l&#39;elenco dei profili target del pubblico.
* **Vista codice**: mostra una versione basata su codice del pubblico in SQL.
* **Visualizza attributi avanzati**: selezionare questa opzione per visualizzare l&#39;elenco completo degli attributi nella tavolozza a sinistra, inclusi nodi, raggruppamenti, collegamenti 1-1 e collegamenti 1-N.
* **Calcola**: aggiorna e visualizza il numero di profili interessati dalla query.
* **Seleziona o salva il filtro**: utilizza un filtro predefinito per filtrare la query oppure salva la query come nuovo filtro per riutilizzarla in futuro. [Scopri come utilizzare i filtri predefiniti](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >In questa versione del prodotto, alcuni filtri predefiniti non sono disponibili nell’interfaccia utente di. Tuttavia, puoi ancora usarli. [Ulteriori informazioni](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Attributi**: visualizza una descrizione del pubblico creato.

## Esempio

In questo esempio, viene creato un pubblico per rivolgersi a tutti i clienti che vivono ad Atlanta o Seattle e sono nati dopo il 1980.

1. Nella scheda **Attributi** della palette, cerca il campo **Data di nascita**. Trascina la sezione e rilasciala sull’area di lavoro.

   ![Aggiunta del campo Data di nascita all&#39;area di lavoro](assets/segment-builder6.png){zoomable="yes"}

1. Nell’area di lavoro, scegli l’operatore **Dopo** e immetti la data desiderata.

   ![Configurazione dell&#39;operatore After per il campo Data di nascita](assets/segment-builder7.png){zoomable="yes"}

1. Nella palette, cerca il campo **Città** e aggiungilo all’area di lavoro sotto la prima regola.

   ![Aggiunta del campo Città all&#39;area di lavoro](assets/segment-builder8.png){zoomable="yes"}

1. Nel campo di testo, immetti il nome della prima città, quindi premi Invio.

   ![Immissione del nome della città nel campo Città](assets/segment-builder9.png){zoomable="yes"}

1. Ripeti questa azione per il nome della seconda città.

   ![Inserimento del secondo nome della città nel campo Città](assets/segment-builder10.png){zoomable="yes"}

1. Fai clic su **Visualizza i risultati** per visualizzare l’elenco e il numero di destinatari corrispondenti alla query. Aggiungi colonne per visualizzare e controllare i dati. In questo esempio, aggiungi la colonna **Città** per visualizzare Atlanta e Seattle.

   ![Visualizzazione dei risultati con la colonna Città aggiunta](assets/segment-builder11.png){zoomable="yes"}

1. Fai clic su **Conferma**.