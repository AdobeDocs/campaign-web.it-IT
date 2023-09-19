---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Modifica dimensione
description: Scopri come utilizzare l’attività del flusso di lavoro Modifica dimensione
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 6%

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

Il **Cambia dimensione** l&#39;attività è un **Targeting** attività. Questa attività ti consente di modificare la dimensione di targeting durante la creazione di un pubblico. Questa attività sposta l’asse a seconda del modello di dati e della dimensione di input. Ad esempio, puoi passare dalla dimensione &quot;contratti&quot; alla dimensione &quot;clienti&quot;.

## Configurazione

Per configurare il **Cambia dimensione** attività:

1. Aggiungi un **Cambia dimensione** al flusso di lavoro.

   ![](../assets/workflow-change-dimension.png)

1. Definisci il **Nuova dimensione di destinazione**. Durante la modifica della dimensione vengono conservati tutti i record. Altre opzioni non sono ancora disponibili.

1. Esegui il flusso di lavoro per visualizzare il risultato. Confronta i dati nelle tabelle prima e dopo l’attività di modifica della dimensione e confronta la struttura delle tabelle del flusso di lavoro.



