---
audience: end-user
title: Utilizzare l’attività Combina flusso di lavoro
description: Scopri come utilizzare l’attività Combina flusso di lavoro
badge: label="Alpha" type="Positive"
source-git-commit: 98b4b43427266d5f9580733d4674db938713296d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 17%

---


# Combina {#combine}

Questa attività ti consente di elaborare i set sui dati in entrata. Puoi quindi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più destinazioni. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Il **Union** consente di raggruppare il risultato di più attività in un unico target.
* Il **Intersezione** consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata nell’attività.
* Il **Esclusione** consente di escludere elementi da una popolazione in base a determinati criteri.

## Configurazione

Per configurare il **Combina** attività:

1. Aggiungi più attività come **Creare un pubblico** attività per formare almeno due rami di esecuzione diversi.
1. Aggiungi un **Combina** a una delle transizioni di segmentazione precedenti.
1. Seleziona il tipo di segmentazione: unione, intersezione o esclusione.
1. Clic **Continua**.
1. In **Set da unire** , controlla tutte le attività precedenti a cui desideri partecipare.

Per **Union** e **Intersezione**, è necessario selezionare **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati:

* Solo tasti: questa è la modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
* Una selezione di colonne: seleziona questa opzione per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati. Devi innanzitutto selezionare il set principale (quello contenente i dati di origine), quindi le colonne da utilizzare per il join.

Per **Intersezione** e **Esclusione**, è possibile controllare **Genera completamento** se desideri elaborare la popolazione rimanente. Il complemento conterrà l’unione dei risultati di tutte le attività in entrata meno l’intersezione. Verrà quindi aggiunta all’attività un’ulteriore transizione in uscita.

Per **Esclusione**, seleziona la **Set primario** dalle transizioni in entrata, nella **Set da unire** sezione. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.

## Esempi

Nell’esempio seguente è stata aggiunta una **unione** che recupera tutti i profili delle due query: persone di età compresa tra 18 e 27 anni e persone di età compresa tra 34 e 40 anni.

![](../assets/workflow-union-example.png)

L&#39;esempio seguente mostra **intersezione** tra due attività di query. Viene utilizzato qui per recuperare profili che hanno tra i 18 e i 27 anni e il cui indirizzo e-mail è stato fornito.

![](../assets/workflow-intersection-example.png)

I seguenti elementi **esclusione** esempio mostra due query configurate per filtrare profili di età compresa tra i 18 e i 27 anni e con un dominio e-mail di adobe. I profili con un dominio e-mail adobe vengono quindi esclusi dal primo set.

![](../assets/workflow-exclusion-example.png)





