---
audience: end-user
title: Utilizzare l’attività Deduplica nei flussi di lavoro
description: Scopri come utilizzare l’attività Deduplica nei flussi di lavoro
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 53%

---

# Deduplica {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campi per identificare i duplicati"
>abstract="Nella sezione **Campi per identificare i duplicati**, fai clic sul pulsante **Aggiungi attributo** per specificare i campi per i quali i valori identici consentono l’identificazione dei duplicati, ad esempio: indirizzo e-mail, nome e cognome. L’ordine dei campi specifica quali elaborare per primi."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Attività Deduplica"
>abstract="L’attività **Deduplica** elimina i duplicati nei risultati delle attività in entrata. Viene utilizzata principalmente dopo le attività di targeting e prima delle attività che utilizzano dati target."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generare un complemento"
>abstract="Puoi generare una transizione in uscita aggiuntiva con la popolazione rimanente, che è stata esclusa come duplicato. A tale scopo, attiva l’opzione **Genera complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Impostazioni di deduplica"
>abstract="Per eliminare i duplicati nei dati in arrivo, definisci il metodo di deduplica nei campi seguenti. Per impostazione predefinita, viene mantenuto un solo record. Seleziona la modalità di deduplica in base a un’espressione o a un attributo. Per impostazione predefinita, il record da escludere dai duplicati viene selezionato in modo casuale."

L’attività **Deduplica** è un’attività di **targeting**. Questa attività elimina i duplicati nei risultati delle attività in entrata, ad esempio i profili duplicati nell’elenco dei destinatari. L&#39;attività **Deduplication** viene generalmente utilizzata dopo le attività di targeting e prima delle attività che utilizzano dati di destinazione.

## Configurare l’attività Deduplica {#deduplication-configuration}

Per configurare l’attività **Deduplica** segui questi passaggi:

![Processo di configurazione deduplicazione flusso di lavoro](../assets/workflow-deduplication.png)

1. Aggiungi un’attività **Deduplica** al flusso di lavoro.

1. Nella sezione **Campi per identificare i duplicati**, fai clic sul pulsante **Aggiungi attributo** per specificare i campi per i quali i valori identici consentono l’identificazione dei duplicati, ad esempio: indirizzo e-mail, nome e cognome. L’ordine dei campi specifica quelli da elaborare per primi. [Scopri come selezionare gli attributi e aggiungerli ai preferiti](../../get-started/attributes.md).

1. Nella sezione **Impostazioni deduplicazione** selezionare il numero di **duplicati univoci da mantenere**. Il valore predefinito per questo campo è 1. Il valore 0 mantiene tutti i duplicati.

   Ad esempio, se i record A e B sono considerati duplicati del record Y e il record C è considerato un duplicato del record Z:

   * Se il valore del campo è 1: vengono conservati solo i record Y e Z.
   * Se il valore del campo è 0: vengono conservati tutti i record.
   * Se il valore del campo è 2: vengono conservati i record C e Z e due record da A, B e Y, per caso o a seconda del metodo di deduplicazione selezionato.

1. Seleziona il **Metodo di deduplica** da utilizzare:

   * **Selezione casuale**: seleziona casualmente il record da escludere dai duplicati.
   * **Utilizzo di un&#39;espressione**: mantiene i record in cui il valore dell&#39;espressione immessa è il minore o il maggiore.
   * **Valori non vuoti**: mantiene i record per i quali l&#39;espressione non è vuota.
   * **Segue un elenco di valori**: definisce la priorità di un valore per uno o più campi. Per definire i valori, fare clic su **Attributo** per selezionare un campo o creare un&#39;espressione, quindi aggiungere i valori nella tabella appropriata. Per definire un nuovo campo, fare clic sul pulsante **Aggiungi** situato sopra l&#39;elenco dei valori.

1. Selezionare l&#39;opzione **Genera complemento** per sfruttare il gruppo rimanente. Il complemento è costituito da tutti i duplicati. Viene quindi aggiunta una transizione aggiuntiva all’attività.

## Esempio {#deduplication-example}

Nell’esempio seguente, utilizza un’attività di deduplica per escludere i duplicati dal target prima di inviare una consegna. I profili duplicati identificati vengono aggiunti a un pubblico dedicato che può essere riutilizzato, se necessario. Scegli l’indirizzo **E-mail** per identificare i duplicati. Mantieni una voce e seleziona il metodo di deduplica **Casuale**.

![Esempio di attività di deduplicazione in un flusso di lavoro](../assets/workflow-deduplication-example.png)