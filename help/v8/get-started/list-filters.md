---
audience: end-user
title: Sfogliare, cercare e filtrare gli elenchi
description: Scopri come sfogliare e filtrare gli elenchi di Campaign Web v8
badge: label="Alpha" type="Positive"
source-git-commit: 9f9cb4423d098ae57f429fb2a49e335d413399c1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 13%

---


# Sfogliare, cercare e filtrare gli elenchi {#list-screens}

La maggior parte dei collegamenti del menu di navigazione a sinistra visualizza elenchi di oggetti, ad esempio l&#39;elenco di **Consegne** o **Campagne**. Alcune di queste schermate di elenco sono di sola lettura. È possibile personalizzare la visualizzazione degli elenchi e filtrarli, come descritto di seguito.

Per rimuovere un filtro, fare clic su **Cancella tutto** pulsante.

## Personalizzare le schermate dell’elenco {#custom-lists}

Gli elenchi vengono visualizzati in colonne. Per visualizzare ulteriori informazioni puoi modificare la configurazione delle colonne. A questo scopo, fai clic su **Configurare una colonna per un layout personalizzato** nell’angolo in alto a destra dell’elenco.

![](assets/config-columns.png){width="70%" align="left"}

In **Configurare le colonne** , aggiungere o rimuovere colonne e modificare l&#39;ordine di visualizzazione.

Ad esempio, per queste impostazioni:

![](assets/columns.png){width="70%" align="left"}

L’elenco mostra le colonne seguenti:

![](assets/column-sample.png){width="70%" align="left"}

Utilizza il **Visualizzare attributi avanzati** per visualizzare tutti gli attributi dell&#39;elenco corrente. [Ulteriori informazioni](#adv-attributes)

## Ordinare i dati {#sort-lists}

Puoi anche ordinare gli elementi nell’elenco facendo clic su un’intestazione di colonna qualsiasi. Viene visualizzata una freccia (su o giù) che indica che l’elenco è ordinato per quella colonna.

Per le colonne numeriche o di data, **Su** freccia indica che l&#39;elenco è ordinato in ordine crescente mentre **Giù** freccia indica un ordine decrescente. Per le colonne con valori stringa o alfanumerici, i valori sono elencati in ordine alfabetico.

## Filtri integrati {#list-built-in-filters}

Per trovare gli elementi più rapidamente, puoi utilizzare la barra di ricerca o filtrare l’elenco in base a criteri contestuali.

![](assets/filter.png){width="70%" align="left"}

Ad esempio, puoi filtrare le consegne in base al loro stato, canale, data di contatto o cartella. È inoltre possibile nascondere i test.

## Filtri personalizzati{#list-custom-filters}

Per creare filtri personalizzati sui dati, passa alla parte inferiore dei filtri e fai clic sul pulsante **Aggiungi regole** pulsante.

Trascina e rilascia gli attributi per creare i criteri di filtro nel **Filtri avanzati** schermo.

![](assets/custom-filter.png){width="70%" align="left"}

Utilizza il **Visualizzare attributi avanzati** per visualizzare tutti gli attributi dell&#39;elenco corrente. [Ulteriori informazioni](#adv-attributes)

## Usa attributi avanzati {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Visualizza gli attributi avanzati"
>abstract="Per impostazione predefinita, nell&#39;elenco degli attributi vengono visualizzati solo gli attributi più comuni. Utilizza questo interruttore per creare un filtro con attributi avanzati."

Solo gli attributi più comuni vengono visualizzati per impostazione predefinita nelle schermate elenco attributi e configurazione filtro. Attributi impostati come `advanced` Gli attributi nello schema dati sono nascosti dalle schermate di configurazione.

Utilizza il **Visualizzare attributi avanzati** attiva per visualizzare tutti gli attributi disponibili per l&#39;elenco corrente.
