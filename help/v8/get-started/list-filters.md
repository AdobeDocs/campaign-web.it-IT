---
audience: end-user
title: Sfogliare, cercare e filtrare gli elenchi
description: Scopri come sfogliare e filtrare gli elenchi di Campaign Web v8
badge: label="Disponibilità limitata"
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 564524185c6bea11d8159d57ee9c28b47df86f74
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 89%

---

# Sfogliare, cercare e filtrare gli elenchi {#list-screens}

La maggior parte dei collegamenti del menu di navigazione a sinistra mostra elenchi di oggetti, ad esempio l’elenco di **Consegne** o **Campagne**. Alcune di queste schermate di elenco sono di sola lettura. È possibile personalizzare la visualizzazione degli elenchi e filtrarli, nel modo descritto di seguito.

Per rimuovere un filtro, fai clic sul pulsante **Cancella tutto**.

## Personalizzare le schermate di elenco {#custom-lists}

Gli elenchi vengono visualizzati in colonne. Per visualizzare ulteriori informazioni puoi modificare la configurazione delle colonne. A questo scopo, fai clic su **Configura le colonne per un layout personalizzato** nell’angolo in alto a destra dell’elenco.

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

Nella schermata **Configura le colonne**, aggiungi o rimuovi le colonne e modificane l’ordine di visualizzazione.

Ad esempio, per queste impostazioni:

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

L’elenco mostra le colonne seguenti:

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

## Ordinare i dati {#sort-lists}

Per ordinare gli elementi dell’elenco, fai clic sulla relativa intestazione di colonna. Viene visualizzata una freccia (su o giù) che indica che l’elenco è ordinato per quella colonna.

Per le colonne numeriche o di data, la freccia **su** indica che l’elenco è ordinato in ordine crescente, mentre la freccia **giù** indica un ordine decrescente. Per le colonne con valori stringa o alfanumerici, i valori sono elencati in ordine alfabetico.

## Filtri incorporati {#list-built-in-filters}

Per trovare gli elementi più rapidamente, puoi utilizzare la barra di ricerca o filtrare l’elenco in base a criteri contestuali.

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

Ad esempio, puoi filtrare le consegne in base al loro stato, canale, data di contatto o cartella. È inoltre possibile nascondere i test.

## Filtri personalizzati{#list-custom-filters}

Per creare filtri personalizzati sui dati, passa alla parte inferiore dei filtri e fai clic sul pulsante **Aggiungi regole**, per accedere al generatore di regole.

Definire e combinare i criteri di filtro in **Filtri avanzati** schermo.

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

I filtri personalizzati sono progettati con Campaign Query Modeler. Informazioni dettagliate su come utilizzarlo sono disponibili in [questa sezione](../query/query-modeler-overview.md).

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."


Only most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes which were set as `advanced` attributes in the data schema are hidden from the configuration screens. 

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list is updated instantly.


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
-->