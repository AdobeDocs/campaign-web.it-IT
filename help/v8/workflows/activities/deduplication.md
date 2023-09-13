---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Deduplicazione
description: Scopri come utilizzare l’attività del flusso di lavoro Deduplicazione
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 13%

---


# Deduplica {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Attività Fork"
>abstract="L’attività Deduplication ti consente di:"

L’attività Deduplication ti consente di eliminare i duplicati nei risultati delle attività in entrata.

L’attività Deduplication viene generalmente utilizzata dopo le attività di targeting e prima delle attività che consentono l’utilizzo di dati mirati.

## Configurazione

Per configurare il **Scheduler** attività:

1. Aggiungi un **Deduplicazione** al flusso di lavoro.

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
