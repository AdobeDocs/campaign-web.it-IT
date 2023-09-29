---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Cambia dimensione
description: Scopri come utilizzare l’attività Cambia dimensione nel flusso di lavoro
badge: label="Beta"
source-git-commit: 2894766336d5ac52625175981c6969a0ac5882d8
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 100%

---


# Cambiare dimensione {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generare un complemento"
>abstract="Puoi generare una transizione in uscita aggiuntiva con la popolazione rimanente, che è stata esclusa come duplicato. A tale scopo, attiva l’opzione **Genera complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Attività Cambia dimensione"
>abstract="Questa attività ti consente di modificare la dimensione targeting durante la creazione di un pubblico. Sposta l’asse in base al modello di dati e alla dimensione di input. Ad esempio, puoi passare dalla dimensione “contratti” alla dimensione “clienti”."

L’attività **Cambia dimensione** è un’attività di **targeting**. Questa attività ti consente di modificare la dimensione targeting durante la creazione del flusso di lavoro. Sposta l’asse in base al modello di dati e alla dimensione di input. [Ulteriori informazioni sulle dimensioni targeting](../../audience/about-recipients.md#targeting-dimensions)

Ad esempio, puoi cambiare la dimensione di targeting di un flusso di lavoro da “Destinatari” ad “Applicazione per abbonati” per inviare notifiche push ai destinatari target.

## Configurare l’attività Cambia dimensione {#configure}

Per configurare l’attività **Cambia dimensione** segui questi passaggi:

1. Aggiungi un’attività **Cambia dimensione** al flusso di lavoro.

   ![](../assets/workflow-change-dimension.png)

1. Definisci la **Nuova dimensione target**. Durante la modifica della dimensione, tutti i record vengono mantenuti. Altre opzioni non sono ancora disponibili.

1. Esegui il flusso di lavoro per visualizzare il risultato. Confronta i dati nelle tabelle prima e dopo l’attività Cambia dimensione e confronta la struttura delle tabelle del flusso di lavoro.

## Esempio {#example}

In questo esempio, si desidera inviare una consegna SMS a tutti i profili che hanno effettuato un acquisto. A questo scopo, viene prima utilizzata un’ attività **[!UICONTROL Creazione del pubblico]** collegata a una dimensione targeting “Acquisto” personalizzata per eseguire il targeting di tutti gli acquisti effettuati.

Quindi viene utilizzata un’attività **[!UICONTROL Cambia dimensione]** per cambiare la dimensione targeting del flusso di lavoro in “Destinatari”. Questo consente di eseguire il targeting dei destinatari che corrispondono alla query.

![](../assets/workflow-change-dimension-example.png)
