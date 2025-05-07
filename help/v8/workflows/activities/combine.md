---
audience: end-user
title: Utilizzare l’attività Combina nei flussi di lavoro
description: Scopri come utilizzare l’attività Combina nei flussi di lavoro
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 62%

---

# Combina {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Attività Combina"
>abstract="L’attività **Combina** consente di eseguire la segmentazione sulla popolazione in entrata. Puoi quindi combinare più popolazioni, escluderne una parte o mantenere solo i dati comuni a più target."

L’attività **Combina** è un’attività di **targeting**. Questa attività consente di eseguire la segmentazione sulla popolazione in entrata. Puoi combinare più popolazioni, escluderne parte o mantenere i dati comuni a più destinazioni. Di seguito sono riportati i tipi di segmentazione disponibili:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* **Union** raggruppa il risultato di più attività in un&#39;unica destinazione.
* L&#39;**intersezione** mantiene solo gli elementi comuni alle diverse popolazioni in entrata nell&#39;attività.
* L’**esclusione** esclude elementi da una popolazione in base a determinati criteri.

## Configurare l’attività Combina {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opzioni di unione per Intersezione"
>abstract="L’intersezione mantiene solo gli elementi comuni alle diverse popolazioni in entrata all’interno dell’attività. Nella sezione Set da unire, seleziona tutte le attività precedenti che desideri unire."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opzioni di unione per Esclusione"
>abstract="L’esclusione esclude elementi da una popolazione in base a determinati criteri. Nella sezione Set da unire, seleziona tutte le attività precedenti che desideri unire."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Selezionare il tipo di segmentazione"
>abstract="Seleziona come combinare i tipi di pubblico. L’**unione** ti consente di raggruppare il risultato di più attività in un’unica destinazione. L’**intersezione** mantiene solo gli elementi comuni alle diverse popolazioni in entrata nell’attività. L’**esclusione** esclude elementi da una popolazione in base a determinati criteri."

Segui questi passaggi comuni per configurare l&#39;attività **Combina**:

![](../assets/workflow-combine.png)

1. Aggiungi più attività, ad esempio **Genera pubblico** attività, per formare almeno due rami di esecuzione diversi.
1. Aggiungi un’attività **Combina** ad uno dei rami precedenti.
1. Seleziona il tipo di segmentazione: [unione](#union), [intersezione](#intersection) o [esclusione](#exclusion).
1. Fai clic su **Continua**.
1. Nella sezione **Imposta per partecipare**, controlla tutte le attività precedenti a cui desideri partecipare.

## Unione {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Opzioni di riconciliazione"
>abstract="Seleziona il **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati. L’opzione **Chiavi** è attivata per impostazione predefinita; vale a dire che l’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. Utilizza l’opzione **Una seleziona di colonne** per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati."

Nell&#39;attività **Combina**, configura un **Unione** selezionando il **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati:

* **Solo chiavi**: modalità predefinita. L’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. È possibile utilizzare questa opzione solo se le popolazioni in entrata sono omogenee.
* **Selezione di colonne**: selezionare questa opzione per definire l&#39;elenco di colonne alle quali viene applicata la riconciliazione dei dati. Selezionare innanzitutto il set principale (i dati di origine), quindi le colonne da utilizzare per il join.

## Intersezione  {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Opzioni di riconciliazione dell’intersezione"
>abstract="Seleziona il **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati. L’opzione **Chiavi** è attivata per impostazione predefinita; vale a dire che l’attività mantiene un solo elemento quando gli elementi delle diverse transizioni in entrata hanno la stessa chiave. Utilizza l’opzione **Una seleziona di colonne** per definire l’elenco di colonne alle quali viene applicata la riconciliazione dei dati."

Nell&#39;attività **Combina**, configura un&#39;intersezione **** eseguendo i seguenti passaggi aggiuntivi:

1. Seleziona il **Tipo di riconciliazione** per definire la modalità di gestione dei duplicati. Consulta la sezione [Unione](#union).
1. Selezionare l&#39;opzione **Genera complemento** se si desidera elaborare la popolazione rimanente. Il complemento contiene l’unione dei risultati di tutte le attività in entrata meno l’intersezione. Viene quindi aggiunta all’attività un’ulteriore transizione in uscita.

## Esclusione {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Regole di esclusione"
>abstract="Se necessario, è possibile gestire le tabelle in entrata. Per escludere un target da un’altra dimensione, tale target deve essere restituito nella stessa dimensione targeting del target principale. Nella sezione Regole di esclusione, fai clic su Aggiungi una regola e specifica le condizioni di modifica della dimensione. La riconciliazione dei dati viene eseguita tramite un attributo o un’unione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Selezionare i set da combinare"
>abstract="Nella sezione **Set da unire**, dalle transizioni in entrata, seleziona **Set primario**. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Regole di esclusione"
>abstract="Se necessario, è possibile gestire le tabelle in entrata. Per escludere un target da un’altra dimensione, tale target deve essere restituito nella stessa dimensione targeting del target principale. Nella sezione Regole di esclusione, fai clic su Aggiungi una regola e specifica le condizioni di modifica della dimensione. La riconciliazione dei dati viene eseguita tramite un attributo o un’unione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Complemento generato da combinazione"
>abstract="Attiva l’opzione Genera complemento per elaborare la popolazione rimanente in una transizione aggiuntiva."

Nell&#39;attività **Combina**, configura un&#39;esclusione **Exclusion** eseguendo i seguenti passaggi aggiuntivi:

1. Nella sezione **Set da unire**, dalle transizioni in entrata, seleziona **Set primario**. Questo è il set da cui gli elementi sono esclusi. Gli altri set confrontano gli elementi prima che vengano esclusi dal set primario.
1. Se necessario, è possibile gestire le tabelle in entrata. Per escludere un target da un’altra dimensione, tale target deve essere restituito nella stessa dimensione targeting del target principale. Fai clic su **Aggiungi una regola** nella sezione **Regole di esclusione** e specifica le condizioni per la modifica della dimensione. La riconciliazione dei dati viene eseguita tramite un attributo o un’unione.
1. Selezionare l&#39;opzione **Genera complemento** se si desidera elaborare la popolazione rimanente. Consulta la sezione [Intersezione](#intersection).

## Esempi {#combine-examples}

Nell&#39;esempio seguente, un&#39;attività **Combine** utilizza una **Union** per recuperare tutti i profili delle due query: persone di età compresa tra i 18 e i 27 anni e persone di età compresa tra i 34 e i 40 anni.

![](../assets/workflow-union-example.png)

L&#39;esempio seguente mostra l&#39;**intersezione** tra due attività di query. Recupera i profili che hanno tra i 18 e i 27 anni e il cui indirizzo e-mail è stato fornito.

![](../assets/workflow-intersection-example.png)

L&#39;esempio di **esclusione** seguente mostra due query configurate per filtrare profili di età compresa tra i 18 e i 27 anni con un dominio e-mail di Adobe. I profili con un dominio e-mail Adobe sono esclusi dal primo set.

![](../assets/workflow-exclusion-example.png)