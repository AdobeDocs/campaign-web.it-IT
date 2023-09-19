---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Modifica dimensione
description: Scopri come utilizzare l’attività del flusso di lavoro Modifica dimensione
badge: label="Beta"
source-git-commit: fb144e4b7186717dd0c4049d8ce884998a1adefe
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 4%

---


# Cambiare dimensione {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generare un complemento"
>abstract="Puoi generare una transizione in uscita aggiuntiva con la popolazione rimanente, che è stata esclusa come duplicato. A tale scopo, attiva l’opzione **Genera complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Cambia attività dimensione"
>abstract="Questa attività ti consente di modificare la dimensione di targeting durante la creazione di un pubblico. Sposta l’asse in base al modello di dati e alla dimensione di input. Ad esempio, puoi passare dalla dimensione &quot;contratti&quot; alla dimensione &quot;clienti&quot;."

Il **Cambia dimensione** l&#39;attività è un **Targeting** attività. Questa attività ti consente di modificare la dimensione di targeting durante la creazione del flusso di lavoro. Sposta l’asse in base al modello di dati e alla dimensione di input. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions)

Ad esempio, puoi cambiare la dimensione di targeting di un flusso di lavoro da &quot;Destinatari&quot; a &quot;Applicazione abbonati&quot; per inviare notifiche push ai destinatari interessati.

## Configurare l’attività Modifica dimensione {#configure}

Per configurare il **Cambia dimensione** attività:

1. Aggiungi un **Cambia dimensione** al flusso di lavoro.

   ![](../assets/workflow-change-dimension.png)

1. Definisci il **Nuova dimensione di destinazione**. Durante la modifica della dimensione vengono conservati tutti i record. Altre opzioni non sono ancora disponibili.

1. Esegui il flusso di lavoro per visualizzare il risultato. Confronta i dati nelle tabelle prima e dopo l’attività di modifica della dimensione e confronta la struttura delle tabelle del flusso di lavoro.

## Esempio {#example}

In questo esempio, vogliamo inviare una consegna SMS a tutti i profili che hanno effettuato un acquisto. A questo scopo, utilizziamo prima un’ **[!UICONTROL Creare un pubblico]** Attività collegata a una dimensione di targeting &quot;Acquisto&quot; personalizzata per eseguire il targeting di tutti gli acquisti che si sono verificati.

Quindi utilizziamo un **[!UICONTROL Cambia dimensione]** attività per cambiare la dimensione di targeting del flusso di lavoro in &quot;Destinatari&quot;. Questo ci consente di eseguire il targeting dei destinatari che corrispondono alla query.

![](../assets/workflow-change-dimension-example.png)
