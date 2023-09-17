---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Deduplicazione
description: Scopri come utilizzare l’attività del flusso di lavoro Deduplicazione
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Deduplica {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Attività di deduplicazione"
>abstract="Il **Deduplicazione** attività ti consente di eliminare i duplicati nei risultati delle attività in entrata. Viene utilizzato principalmente dopo le attività di targeting e prima delle attività che consentono l’utilizzo di dati mirati."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generare un complemento"
>abstract="Puoi generare una transizione in uscita aggiuntiva con la popolazione rimanente, che è stata esclusa come duplicato. A tale scopo, attiva l’opzione **Genera complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Impostazioni di deduplicazione"
>abstract="Per eliminare i duplicati nei dati in arrivo, definisci il metodo di deduplicazione nei campi seguenti. Per impostazione predefinita, viene mantenuto un solo record. Devi anche selezionare la modalità di deduplicazione in base a un’espressione o a un attributo. Per impostazione predefinita, il record da escludere dai duplicati viene selezionato in modo casuale."

Il **Deduplicazione** l&#39;attività è un **Targeting** attività. Questa attività ti consente di eliminare i duplicati nei risultati delle attività in entrata. Il **Deduplicazione** l’attività viene generalmente utilizzata dopo le attività di targeting e prima delle attività che consentono l’utilizzo di dati mirati.

## Configurazione

Per configurare il **Deduplicazione** attività:

1. Aggiungi un **Deduplicazione** al flusso di lavoro.

   ![](../assets/workflow-deduplication.png)

1. In **Campi per identificare i duplicati** , fare clic sul pulsante **Aggiungi attributo** per specificare i campi per i quali i valori identici consentono l’identificazione dei duplicati: indirizzo e-mail, nome, cognome, ecc. L’ordine dei campi ti consente di specificare quali elaborare per primi.

1. Seleziona il numero di univoci **Duplicati da mantenere**. Il valore predefinito per questo campo è 1. Il valore 0 ti consente di conservare tutti i duplicati.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Seleziona la **Metodo di deduplicazione** da utilizzare:

   * **Selezione casuale**: seleziona in modo casuale il record da escludere dai duplicati.
   * **Utilizzo di un’espressione**: questo ti consente di conservare i record in cui il valore dell’espressione immessa è il minore o il maggiore. ++ Expression ++ Sort
   * **Seguendo un elenco di valori**: ti consente di definire un valore di priorità per uno o più campi. Per definire i valori, fai clic su **Attributo** per selezionare un campo o creare un’espressione, aggiungi i valori nella tabella appropriata. Per definire un nuovo campo, fai clic sul pulsante Aggiungi situato sopra l’elenco dei valori. ++ Ordina

1. Controlla la **Genera complemento** se desideri sfruttare il gruppo rimanente. Il complemento è costituito da tutti i duplicati. Verrà quindi aggiunta una transizione aggiuntiva all’attività.

## Esempio

