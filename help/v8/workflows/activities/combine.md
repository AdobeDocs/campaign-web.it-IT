---
audience: end-user
title: Utilizzare l’attività Combina nei flussi di lavoro
description: Scopri come utilizzare l’attività Combina nei flussi di lavoro
badge: label="Beta"
source-git-commit: d5b0777ba51f595733c6b7e366d0a9a21a13d84a
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 85%

---


# Combina {#combine}

Il **Combina** l&#39;attività è un **Targeting** attività. Questa attività consente di eseguire la segmentazione sulla popolazione in entrata. Puoi quindi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più target. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* L’attività **Unione** consente di raggruppare il risultato di più attività in un unico target.
* L’attività **Intersezione** consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata all’interno dell’attività.
* L’attività **Esclusione** consente di escludere elementi da una popolazione in base a determinati criteri.

## Configurazione generale {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opzioni di unione per Intersezione"
>abstract="L’attività Intersezione consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata all’interno dell’attività. Nella sezione Set da unire, seleziona tutte le attività precedenti che desideri unire."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opzioni di unione per Esclusione"
>abstract="L’attività Esclusione consente di escludere elementi da una popolazione in base a determinati criteri. Nella sezione Set da unire, seleziona tutte le attività precedenti che desideri unire."

Per iniziare a configurare l’attività **Combina**, segui questi passaggi comuni:

1. Aggiungi più attività, come le attività **Crea pubblico**, per formare almeno due rami di esecuzione diversi.
1. Aggiungi un’attività **Combina** ad uno dei rami precedenti.
1. Seleziona il tipo di segmentazione: [Unione](#union), [Intersezione](#intersection) o [Esclusione](#exclusion).
1. Fai clic su **Continua**.
1. Nella sezione **Set da unire**, seleziona tutte le attività precedenti che desideri unire.

## Unione {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Intersezione  Opzioni di riconciliazione"
>abstract="Seleziona il tipo di riconciliazione per definire la modalità di gestione dei duplicati."

In **Combina** attività, puoi configurare un **Union**. A questo scopo, seleziona la **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati:

* **Solo chiavi**: è la modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
* **Una seleziona di colonne**: seleziona questa opzione per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati. Innanzitutto è necessario selezionare il set primario (quello contenente i dati di origine), quindi le colonne da utilizzare per l’unione.

## Intersezione {#intersection}

In **Combina** attività, puoi configurare un’ **Intersezione**. A questo scopo, segui i passaggi aggiuntivi riportati di seguito:

1. Seleziona il **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati. Consulta la sezione [Unione](#union).
1. Puoi selezionare l’opzione **Genera complemento** se desideri elaborare la popolazione rimanente. Il complemento conterrà l’unione dei risultati di tutte le attività in entrata senza l’intersezione. Verrà quindi aggiunta all’attività un’ulteriore transizione in uscita.

## Esclusione {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Regole di esclusione"
>abstract="Se necessario, è possibile elaborare le tabelle in entrata. In effetti, per escludere un target da un’altra dimensione, tale target deve essere restituito nella stessa dimensione targeting del target principale. A questo scopo, nella sezione Regole di esclusione, fai clic su Aggiungi una regola e specifica le condizioni di modifica della dimensione. La riconciliazione dei dati viene eseguita tramite un attributo o un’unione."

In **Combina** attività, puoi configurare un’ **Esclusione**. A questo scopo, segui i passaggi aggiuntivi riportati di seguito:

1. Nella sezione **Set da unire**, dalle transizioni in entrata, seleziona **Set primario**. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.
1. Se necessario, è possibile elaborare le tabelle in entrata. In effetti, per escludere un target da un’altra dimensione, tale target deve essere restituito nella stessa dimensione targeting del target principale. A questo scopo, nella sezione **Regole di esclusione**, fai clic su **Aggiungi una regola** e specifica le condizioni per la modifica delle dimensioni. La riconciliazione dei dati viene eseguita tramite un attributo o un’unione.
1. Puoi selezionare l’opzione **Genera complemento** se desideri elaborare la popolazione rimanente. Consulta la sezione [Intersezione](#intersection).

## Esempi

Nell’esempio seguente viene utilizzato un **Combina** e viene aggiunta una **unione** per recuperare tutti i profili delle due query: persone di età compresa tra 18 e 27 anni e persone di età compresa tra 34 e 40 anni.

![](../assets/workflow-union-example.png)

L’esempio seguente mostra l’**intersezione** tra due attività di query. In questo caso, viene utilizzata per recuperare i profili che hanno tra i 18 e i 27 anni e il cui indirizzo e-mail è stato fornito.

![](../assets/workflow-intersection-example.png)

Il seguente esempio di attività di **Esclusione** mostra due query configurate per filtrare i profili di età compresa tra i 18 e i 27 anni con un dominio e-mail di Adobe. I profili con un dominio e-mail di Adobe sono quindi esclusi dal primo set.

![](../assets/workflow-exclusion-example.png)


