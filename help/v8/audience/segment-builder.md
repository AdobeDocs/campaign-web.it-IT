---
audience: end-user
title: Definire un pubblico con il generatore di regole
description: Scopri come lavorare con Segment Builder
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: a59c133254632c49618fae6ad3d61a2f6e0a1eea
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Definire un pubblico con il generatore di regole {#segment-builder}

![](../assets/do-not-localize/badge.png)

Questa sezione descrive come creare un pubblico durante la progettazione di un nuovo messaggio e-mail. Il pubblico creato può essere utilizzato solo in questo messaggio e-mail.

Il generatore di regole ti consente di definire la popolazione target del messaggio filtrando i dati contenuti nel database. Per selezionare un pubblico esistente, consulta [sezione](add-audience.md).

Per ulteriori informazioni sul generatore di regole, consulta la [Documentazione del servizio di segmentazione](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

Per creare un nuovo pubblico durante la progettazione di un’e-mail, effettua le seguenti operazioni:

1. Da **Pubblico** nell’assistente per la creazione della consegna, fai clic sul pulsante **[!UICONTROL Selezionare il pubblico]** pulsante .

   ![](assets/segment-builder0.png)

1. Seleziona **Crea il tuo**. Viene visualizzato il generatore di regole.

   ![](assets/segment-builder.png)

## La palette

La palette, situata a sinistra, contiene tutti gli elementi che è possibile filtrare per creare un pubblico. Per poter essere configurati e presi in considerazione, i riquadri contenuti nella palette devono essere spostati nell’area di lavoro centrale. La palette è divisa in due schede:

* **Attributi**: questa scheda ti consente di accedere a tutti i campi disponibili dallo schema. L’elenco dei campi dipende dallo schema di targeting definito nel modello e-mail.

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **Tipi di pubblico**: questa scheda ti consente di filtrare utilizzando uno dei tipi di pubblico esistenti definiti nella console Campaign Classic o da Adobe Experience Platform.

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >Per sfruttare i tipi di pubblico di Adobe Experience Platform, devi configurare l’integrazione con le destinazioni. Fai riferimento a [Documentazione sulle destinazioni](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=it){target="_blank"}.

Puoi usare la barra di ricerca per trovare rapidamente gli elementi.

## Il quadro

L’area di lavoro è la zona centrale in cui è possibile configurare e combinare le regole in base agli elementi aggiunti dalla palette. Per aggiungere una nuova regola, trascina un riquadro dalla palette e rilascialo nell’area di lavoro. Verranno quindi presentate opzioni specifiche per il contesto in base al tipo di dati aggiunti.

![](assets/segment-builder4.png){width="70%" align="left"}

## Riquadro delle proprietà della regola

Sul lato destro, il **Proprietà delle regole** Il riquadro ti consente di eseguire le azioni seguenti:

![](assets/segment-builder5.png){width="70%" align="left"}

* **Visualizza risultati:** visualizza l’elenco dei destinatari interessati dal pubblico.
* **Vista Codice**: visualizza una versione del pubblico basata su codice in SQL.
* **Visualizzare gli attributi avanzati**: seleziona questa opzione se desideri visualizzare l’elenco completo degli attributi nella palette a sinistra: nodi, raggruppamenti, collegamenti 1-1, collegamenti 1-N.
* **Attributi**: visualizza una descrizione del pubblico creato.

## Esempio

In questo esempio, creeremo un pubblico per tutti i clienti che vivono ad Atlanta o a Seattle e sono nati dopo il 1980.

1. In **Attributi** scheda della palette, cerca il **Data di nascita** campo . Trascina la tessera e rilasciala sull’area di lavoro.

   ![](assets/segment-builder6.png)

1. Nell’area di lavoro, scegli la **Dopo** e immetti la data desiderata.

   ![](assets/segment-builder7.png)

1. Nella palette, cerca il **Città** e aggiungilo all&#39;area di lavoro sotto la prima regola.

   ![](assets/segment-builder8.png)

1. Nel campo di testo, immettere il nome della prima città, quindi premere invio.

   ![](assets/segment-builder9.png)

1. Ripetere questa azione per il nome della seconda città.

   ![](assets/segment-builder10.png)

1. Fai clic su **Visualizza risultati** per visualizzare l’elenco e il numero di destinatari corrispondenti alla query. Puoi anche aggiungere colonne per visualizzare e controllare i dati. Nel nostro esempio, aggiungi la **Città** dovrebbe vedere Atlanta e Seattle.

   ![](assets/segment-builder11.png)

1. Fai clic su **Conferma**.

Il pubblico è definito e pronto per essere utilizzato nell’e-mail.