---
audience: end-user
title: Utilizzare l’attività Combina flusso di lavoro
description: Scopri come utilizzare l’attività Combina flusso di lavoro
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 14%

---


# Combina {#combine}

Questa attività ti consente di eseguire la segmentazione sulla popolazione in entrata. Puoi quindi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più destinazioni. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Il **Union** consente di raggruppare il risultato di più attività in un unico target.
* Il **Intersezione** consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata nell’attività.
* Il **Esclusione** consente di escludere elementi da una popolazione in base a determinati criteri.

## Configurazione generale {#general}

Per iniziare a configurare il **Combina** attività:

1. Aggiungi più attività come **Creare un pubblico** attività per formare almeno due rami di esecuzione diversi.
1. Aggiungi un **Combina** ad uno dei rami precedenti.
1. Seleziona il tipo di segmentazione: [unione](#union), [intersezione](#intersection) o [esclusione](#exclusion).
1. Clic **Continua**.
1. In **Set da unire** , controlla tutte le attività precedenti a cui desideri partecipare.

## Unione {#union}

Per **Union**, è necessario selezionare **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati:

* **Solo chiavi**: è la modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
* **Selezione di colonne**: seleziona questa opzione per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati. Devi innanzitutto selezionare il set principale (quello contenente i dati di origine), quindi le colonne da utilizzare per il join.

## Intersezione {#intersection}

Per **Intersezione**, è necessario seguire questi passaggi aggiuntivi:

1. Seleziona la **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati. Consulta la [Union](#union) sezione.
1. Puoi controllare la **Genera completamento** se desideri elaborare la popolazione rimanente. Il complemento conterrà l’unione dei risultati di tutte le attività in entrata meno l’intersezione. Verrà quindi aggiunta all’attività un’ulteriore transizione in uscita.

## Esclusione {#exclusion}

Per **Esclusione**, è necessario seguire questi passaggi aggiuntivi:

1. In **Set da unire** , seleziona la sezione **Set primario** dalle transizioni in entrata. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.
1. Se necessario, è possibile modificare le tabelle in entrata. In effetti, per escludere un target da un’altra dimensione, tale target deve essere riportato alla stessa dimensione di targeting del target principale. A questo scopo, fai clic su **Aggiungi una regola** nel **Regole di esclusione** e specificare le condizioni per la modifica delle quote. La riconciliazione dei dati viene eseguita tramite un attributo o un join.
1. Puoi controllare la **Genera completamento** se desideri elaborare la popolazione rimanente. Consulta la [Intersezione](#intersection) sezione.

## Esempi

Nell’esempio seguente è stata aggiunta una **unione** che recupera tutti i profili delle due query: persone di età compresa tra 18 e 27 anni e persone di età compresa tra 34 e 40 anni.

![](../assets/workflow-union-example.png)

L&#39;esempio seguente mostra **intersezione** tra due attività di query. Viene utilizzato qui per recuperare profili che hanno tra i 18 e i 27 anni e il cui indirizzo e-mail è stato fornito.

![](../assets/workflow-intersection-example.png)

I seguenti elementi **esclusione** Questo esempio mostra due query configurate per filtrare profili di età compresa tra i 18 e i 27 anni con un dominio e-mail di Adobe. I profili con un dominio e-mail di Adobe vengono quindi esclusi dal primo set.

![](../assets/workflow-exclusion-example.png)


