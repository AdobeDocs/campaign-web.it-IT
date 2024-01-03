---
audience: end-user
title: Filtra elenchi
description: Scopri come filtrare gli elenchi web di Adobe Campaign utilizzando filtri incorporati e personalizzati.
source-git-commit: 843f3ad906d81892f45281ef5734d512b4c8f3d6
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 6%

---


# Filtra elenchi {#filter-lists}

Adobe Campaign Web fornisce filtri all’interno di ogni elenco di oggetti, consentendo di filtrare le informazioni in base a criteri contestuali specifici. Ad esempio, puoi filtrare le consegne in base al loro stato, canale, data di contatto o cartella. È inoltre possibile nascondere i test.

## Applicare i filtri{#apply}

Per applicare i filtri a un elenco, fare clic su **[!UICONTROL Mostra filtri]** nell&#39;angolo superiore sinistro dell&#39;elenco, accanto alla barra di ricerca.

Viene visualizzato il riquadro Filtri, in cui sono visualizzati i filtri disponibili per l’elenco selezionato. Ad esempio, puoi filtrare le campagne in base al loro stato, alle date di inizio e fine o alla cartella di archiviazione, mentre l’elenco dei servizi di abbonamento può essere filtrato in base al loro canale e alla loro cartella di archiviazione.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Per filtrare un elenco in base a criteri personalizzati, crea un filtro personalizzato. A questo scopo, passa alla parte inferiore del riquadro dei filtri e fai clic sul pulsante **Aggiungi regole** pulsante. [Scopri come creare filtri personalizzati](#custom)

Una volta applicati a un elenco, i filtri sono visibili sotto la barra di ricerca. Puoi rimuovere un singolo filtro in qualsiasi momento oppure tutti i filtri facendo clic sul pulsante **Cancella tutto** pulsante.

## Creare filtri personalizzati {#custom}

I filtri personalizzati ti consentono di perfezionare gli elenchi in base a criteri specifici. Sono progettate utilizzando il modellatore di query di Campaign. Per creare un filtro personalizzato, effettua le seguenti operazioni:

1. Apri il riquadro dei filtri e fai clic su **Aggiungi regole** nella parte inferiore del riquadro.
1. Viene aperto Query Modeler. Definisci e combina i criteri di filtro in base alle tue esigenze. Informazioni dettagliate sull’utilizzo di Query Modeler sono disponibili in [questa sezione](../query/query-modeler-overview.md).

   L’esempio seguente mostra un filtro personalizzato progettato per visualizzare nell’elenco delle campagne le campagne SMS eseguite dagli operatori dei dipartimenti in esecuzione o Yoga.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. Una volta configurato il filtro personalizzato, fai clic su **[!UICONTROL Conferma]** per applicarlo all&#39;elenco.
