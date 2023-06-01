---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 8aa76369-c9f3-4c5b-9a51-101b239727e6
source-git-commit: 1e1f1bbdd5c1a8e659c455078b5995b23209c511
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 7%

---

# Avviare e monitorare l’esecuzione del flusso di lavoro {#start-monitor}

Dopo aver creato il flusso di lavoro e progettato le attività da eseguire nell’area di lavoro, puoi avviarlo e monitorarne l’esecuzione.

## Avviare il flusso di lavoro {#start}

Per avviare il flusso di lavoro, passa a **[!UICONTROL Flussi di lavoro]** o la campagna associata e fai clic sul pulsante **[!UICONTROL Inizio]** nell’angolo superiore destro dell’area di lavoro.

Una volta eseguito il flusso di lavoro, ogni attività nell’area di lavoro viene eseguita in ordine sequenziale, fino al raggiungimento della fine del flusso di lavoro.

Puoi monitorare l’avanzamento dei profili target in tempo reale utilizzando un flusso visivo. Questo consente di identificare rapidamente lo stato di ciascuna attività e il numero di profili che passano da un’attività all’altra.

![](assets/workflow-execution.png)

>[!NOTE]
>
>È possibile disattivare il flusso visivo utilizzando **[!UICONTROL Nascondi progressione]** nella barra delle azioni superiore dell’area di lavoro.

## Monitorare l’esecuzione dell’attività {#activities}

Gli indicatori visivi nell’angolo superiore destro di ciascuna casella di attività ti consentono di controllarne l’esecuzione:

| Indicatore visivo | Descrizione |
|-----|------------|
| ![](assets/activity-status-pending.png) | L’attività è attualmente in esecuzione. |
| ![](assets/activity-status-orange.png) | L’attività richiede la tua attenzione. Ciò può comportare la conferma dell’invio di una consegna o l’adozione di un’azione necessaria. |
| ![](assets/activity-status-red.png) | L’attività ha riscontrato un errore. Per risolvere il problema, apri i registri del flusso di lavoro per ulteriori informazioni. |
| ![](assets/activity-status-green.png) | L&#39;attività è stata eseguita correttamente. |

## Monitorare registri e attività

Il monitoraggio dei registri e delle attività dei flussi di lavoro è un passaggio chiave per analizzare i flussi di lavoro e assicurarsi che vengano eseguiti correttamente. Sono accessibili dalla sezione **[!UICONTROL Registri]** disponibile nella barra degli strumenti delle azioni e nel riquadro delle proprietà di ogni attività.

Il **[!UICONTROL Registri e attività]** fornisce una cronologia dell’esecuzione del flusso di lavoro, registrando tutte le azioni dell’utente e gli errori riscontrati. Questa cronologia viene salvata per la durata specificata nel flusso di lavoro [opzioni di esecuzione](workflow-settings.md). Durante questo periodo, tutti i messaggi vengono salvati, anche dopo un riavvio del flusso di lavoro. Se non desideri salvare i messaggi di un’esecuzione precedente, fai clic sul pulsante **[!UICONTROL Cancella cronologia]** pulsante.

![](assets/workflow-logs.png)

Sono disponibili due tipi di informazioni:

* Il **[!UICONTROL Log]** contiene la cronologia di esecuzione di tutte le attività del flusso di lavoro. Questi registri indicizzano in ordine cronologico le operazioni effettuate e gli errori di esecuzione.
* Il **[!UICONTROL Attività]** La scheda descrive la sequenza di esecuzione delle attività.

In entrambe le schede, puoi scegliere le colonne visualizzate e il loro ordine, applicare filtri e utilizzare il campo di ricerca per trovare rapidamente le informazioni desiderate.

## Comandi di esecuzione del flusso di lavoro {#execution-commands}

La barra delle azioni nell’angolo in alto a destra fornisce comandi che consentono di gestire l’esecuzione del flusso di lavoro. È possibile eseguire le seguenti operazioni:

* **[!UICONTROL Inizio]** / **[!UICONTROL Riprendi]** l’esecuzione del flusso di lavoro, che assume quindi lo stato In corso. Se il flusso di lavoro è stato sospeso, viene ripreso, altrimenti viene avviato e le attività iniziali vengono quindi attivate.

* **[!UICONTROL Pausa]** l’esecuzione del flusso di lavoro, che assume quindi lo stato In pausa. Non verranno attivate nuove attività finché non viene ripresa, ma le operazioni in corso non vengono sospese.

* **[!UICONTROL Interrompi]** un flusso di lavoro in esecuzione che assume lo stato Finished. Se possibile, le operazioni in corso vengono interrotte. Non è possibile riprendere dal flusso di lavoro dalla stessa posizione in cui è stato interrotto.
