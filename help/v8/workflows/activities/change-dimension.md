---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Cambia dimensione
description: Scopri come utilizzare l’attività Cambia dimensione nel flusso di lavoro
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 46%

---

# Cambiare dimensione {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generare un complemento"
>abstract="Puoi generare una transizione in uscita aggiuntiva con la popolazione rimanente, che è stata esclusa come duplicato. A tale scopo, attiva l’opzione **Genera complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Attività Cambia dimensione"
>abstract="Questa attività ti consente di modificare la dimensione targeting durante la creazione di un pubblico. Sposta l’asse in base al modello di dati e alla dimensione di input. Ad esempio, puoi passare dalla dimensione &quot;contratti&quot; alla dimensione &quot;clienti&quot;."

L’attività **Cambia dimensione** è un’attività di **targeting**. Questa attività ti consente di modificare la dimensione targeting durante la creazione del flusso di lavoro. Sposta l’asse in base al modello di dati e alla dimensione di input. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions).

Ad esempio, puoi cambiare la dimensione di targeting di un flusso di lavoro da &quot;Destinatari&quot; a &quot;Applicazione abbonati&quot; per inviare notifiche push ai destinatari interessati.

>[!IMPORTANT]
>
>Le attività **[!UICONTROL Modifica dimensione]** e **[!UICONTROL Modifica origine dati]** non devono essere aggiunte in una riga. Se devi utilizzare entrambe le attività consecutivamente, includi un&#39;attività **[!UICONTROL Arricchimento]** tra di esse. In questo modo si garantisce la corretta esecuzione e si evitano potenziali conflitti o errori.

## Configurare l’attività Cambia dimensione {#configure}

Per configurare l’attività **Cambia dimensione** segui questi passaggi:

1. Aggiungi un’attività **Cambia dimensione** al flusso di lavoro.

   ![Schermata che mostra l&#39;attività Modifica dimensione aggiunta a un flusso di lavoro](../assets/workflow-change-dimension.png)

1. Definisci la **Nuova dimensione target**. Durante la modifica della dimensione, tutti i record vengono mantenuti. Altre opzioni non sono ancora disponibili.

1. Esegui il flusso di lavoro per visualizzare il risultato. Confronta i dati nelle tabelle prima e dopo l’attività Modifica dimensione e confronta la struttura delle tabelle del flusso di lavoro.

## Esempio {#example}

In questo esempio, invia una consegna SMS a tutti i profili che hanno effettuato un acquisto. Innanzitutto, utilizza un&#39;attività **[!UICONTROL Genera pubblico]** collegata a una dimensione di targeting &quot;Acquisto&quot; personalizzata per eseguire il targeting di tutti gli acquisti che si sono verificati.

Quindi, utilizza un&#39;attività **[!UICONTROL Modifica dimensione]** per cambiare la dimensione di targeting del flusso di lavoro in &quot;Destinatari&quot;. Questo consente di eseguire il targeting dei destinatari che corrispondono alla query.

![Schermata che mostra un esempio dell&#39;attività Change dimension utilizzata in un flusso di lavoro](../assets/workflow-change-dimension-example.png)