---
audience: end-user
title: Utilizzare l’attività Combina flusso di lavoro
description: Scopri come utilizzare l’attività Combina flusso di lavoro
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 23%

---


# Combina {#combine}

Questa attività ti consente di elaborare i set sui dati in entrata. Puoi quindi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più destinazioni. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Il **Union** consente di raggruppare il risultato di più attività in un unico target.
* Il **Intersezione** consente di mantenere solo gli elementi comuni alle diverse popolazioni in entrata nell’attività.
* Il **Esclusione** consente di escludere elementi da una popolazione in base a determinati criteri.

Per configurare il **Combina** attività:

1. Aggiungi il **Combina** a una delle transizioni di segmentazione precedenti.
1. Seleziona il tipo di segmentazione: unione, intersezione o esclusione.
1. Clic **Continua**.
1. In **Set da unire** , controlla tutte le attività precedenti a cui desideri partecipare.

Per **Union** e **Intersezione**, è necessario selezionare **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati:

    * Solo tasti: è la modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
    * Una selezione di colonne: seleziona questa opzione per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati. Devi innanzitutto selezionare il set principale (quello contenente i dati di origine), quindi le colonne da utilizzare per il join.

Per **Intersezione** e **Esclusione**, è possibile controllare **Genera completamento** se desideri elaborare la popolazione rimanente. Il complemento conterrà l’unione dei risultati di tutte le attività in entrata meno l’intersezione. Verrà quindi aggiunta all’attività un’ulteriore transizione in uscita.

Per **Esclusione**, seleziona la **Set primario** dalle transizioni in entrata, nella **Set da unire** sezione. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.
