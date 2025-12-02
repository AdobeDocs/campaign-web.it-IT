---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 30%

---

# Avviare e monitorare i flussi di lavoro {#start-monitor}

Dopo aver creato il flusso di lavoro e progettato le attività da eseguire nell’area di lavoro, puoi avviarlo e monitorarne l’esecuzione.

## Avviare il flusso di lavoro {#start}

Per avviare il flusso di lavoro, passa al menu **[!UICONTROL Flussi di lavoro]** o alla campagna associata e fai clic sul pulsante **[!UICONTROL Inizio]** nell&#39;angolo superiore destro dell&#39;area di lavoro.

Una volta eseguito il flusso di lavoro, ogni attività nell’area di lavoro viene eseguita in sequenza fino al raggiungimento della fine del flusso di lavoro.

Puoi monitorare l’avanzamento dei profili target in tempo reale utilizzando un flusso visivo. Questo consente di identificare rapidamente lo stato di ciascuna attività e il numero di profili che passano da un’attività all’altra.

![Rappresentazione visiva dell&#39;esecuzione del flusso di lavoro in corso.](assets/workflow-execution.png){zoomable="yes"}

## Transizioni del flusso di lavoro {#transitions}

Nei flussi di lavoro, i dati trasportati da un’attività all’altra tramite transizioni vengono memorizzati in una tabella di lavoro temporanea. Questi dati possono essere visualizzati per ogni transizione. Per visualizzare i dati, seleziona una transizione per aprirne le proprietà sul lato destro dello schermo.

* Fai clic su **[!UICONTROL Anteprima schema]** per visualizzare lo schema della tabella di lavoro.
* Fai clic su **[!UICONTROL Anteprima risultati]** per visualizzare i dati trasportati nella transizione selezionata.

![Esempio di proprietà di transizione e anteprima dei dati.](assets/transition.png){zoomable="yes"}

## Monitorare l’esecuzione dell’attività {#activities}

Gli indicatori visivi nell’angolo superiore destro di ciascuna casella di attività ti consentono di controllarne lo stato di esecuzione:

| Indicatore visivo | Descrizione |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | L’attività è attualmente in esecuzione. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | L’attività richiede la tua attenzione. Ciò potrebbe implicare la conferma dell’invio di una consegna o l’adozione di un’azione necessaria. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | L’attività ha rilevato un errore. Per risolvere il problema, apri i registri del flusso di lavoro per ulteriori informazioni. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | L&#39;attività è stata eseguita correttamente. |

## Monitorare i registri e le attività {#logs-tasks}

Il monitoraggio dei registri e delle attività dei flussi di lavoro è un passaggio chiave per analizzarli e garantirne il corretto funzionamento. I registri e le attività sono accessibili dall&#39;icona **[!UICONTROL Registri]**, disponibile nella barra degli strumenti delle azioni e nel riquadro delle proprietà di ogni attività.

Il menu **[!UICONTROL Registri e attività]** fornisce una cronologia dell&#39;esecuzione del flusso di lavoro, registrando tutte le azioni dell&#39;utente e gli errori riscontrati. Questa cronologia viene salvata per la durata specificata nelle [opzioni di esecuzione](workflow-settings.md) del flusso di lavoro. Durante questo periodo, tutti i messaggi vengono salvati, anche dopo il riavvio di un flusso di lavoro. Se non si desidera salvare i messaggi di un&#39;esecuzione precedente, fare clic sul pulsante **[!UICONTROL Rimuovi cronologia]**.

![Esempio di interfaccia per i registri del flusso di lavoro e le attività.](assets/workflow-logs.png){zoomable="yes"}

Sono disponibili due tipi di informazioni:

* La scheda **[!UICONTROL Registro]** contiene la cronologia di esecuzione di tutte le attività del flusso di lavoro. Indica le operazioni eseguite e gli errori di esecuzione in ordine cronologico.
* Nella scheda **[!UICONTROL Attività]** viene illustrata la sequenza di esecuzione delle attività.

In entrambe le schede, puoi scegliere le colonne visualizzate e il loro ordine, applicare filtri e utilizzare il campo di ricerca per trovare rapidamente le informazioni desiderate.

## Comandi di esecuzione del flusso di lavoro {#execution-commands}

La barra delle azioni nell’angolo in alto a destra fornisce i comandi per gestire l’esecuzione del flusso di lavoro. Puoi eseguire le seguenti azioni:

* **[!UICONTROL Avvia]** / **[!UICONTROL Riprendi]** l&#39;esecuzione del flusso di lavoro. Se il flusso di lavoro è stato messo in pausa, viene ripreso. In caso contrario, si avvia e vengono attivate le attività iniziali.
* **[!UICONTROL Sospendi]** l&#39;esecuzione del flusso di lavoro. Il flusso di lavoro assume quindi lo stato In pausa. Non vengono attivate nuove attività finché non riprendono, ma le operazioni in corso non vengono sospese.
* **[!UICONTROL Interrompi]** un flusso di lavoro in esecuzione. Il flusso di lavoro assume quindi lo stato Finito. Se possibile, le operazioni in corso vengono interrotte. Non è possibile riprendere il flusso di lavoro dal punto in cui è stato interrotto.