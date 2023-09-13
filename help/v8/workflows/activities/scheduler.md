---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Scheduler
description: Scopri come utilizzare l’attività del flusso di lavoro Scheduler
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 31%

---


# Attività Scheduler {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Attività Scheduler"
>abstract="L’attività Scheduler ti consente di..."

L’attività Scheduler ti consente di pianificare quando viene avviato un flusso di lavoro o un’attività.

L’attività Scheduler deve essere considerata come un inizio pianificato. Questa attività può essere utilizzata solo come prima attività del flusso di lavoro.

## Best practice

* Non pianificare l’esecuzione di un flusso di lavoro con una frequenza superiore a 15 minuti, in quanto ciò potrebbe impedire le prestazioni complessive del sistema e creare blocchi nel database.

## Configurazione

Per configurare il **Scheduler** attività:

1. Aggiungi un **Scheduler** al flusso di lavoro.

1. Configurare **Frequenza di esecuzione**:

   * Una volta: il flusso di lavoro viene eseguito una sola volta.

   * Giornaliero: il flusso di lavoro viene eseguito una volta al giorno a un’ora specifica.

   * Più volte al giorno: il flusso di lavoro viene eseguito regolarmente più volte al giorno. Puoi impostare esecuzioni in orari specifici o periodicamente.

   * Settimanale: il flusso di lavoro viene eseguito in un determinato momento, una o più volte alla settimana.

   * Mensile: il flusso di lavoro viene eseguito in un determinato momento, una o più volte al mese. Puoi selezionare i mesi, quando devi eseguire il flusso di lavoro. Puoi anche impostare le esecuzioni in un giorno feriale specifico del mese, ad esempio il secondo martedì del mese.
1. Definisci i dettagli di esecuzione in base alla frequenza selezionata. I campi dettagliati possono variare a seconda della frequenza utilizzata (tempo, frequenza di ripetizione, giorni specificati, ecc.).

1. Clic **Anteprima orari di avvio** per controllare la pianificazione delle dieci esecuzioni successive del flusso di lavoro.

1. Definire il periodo di validità dello scheduler:

   * Permanente (non scade mai): il flusso di lavoro viene eseguito, in base alla frequenza specificata, senza alcun limite all’intervallo di tempo o al numero di iterazioni.

   * Periodo di validità: il flusso di lavoro viene eseguito in base alla frequenza specificata, fino a una data specifica. Occorre pertanto precisare il termine per l’esecuzione.

## Esempio


