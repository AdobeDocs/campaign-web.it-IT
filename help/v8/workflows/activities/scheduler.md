---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Scheduler
description: Scopri come utilizzare l’attività del flusso di lavoro Scheduler
badge: label="Beta"
source-git-commit: 4f53f8765aeb2254a52eb48591d5e14250afc69d
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 10%

---


# Attività Scheduler {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Attività Scheduler"
>abstract="Il **Scheduler** attività ti consente di pianificare quando viene avviato il flusso di lavoro. Questa attività deve essere considerata come un inizio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro."


Il **Scheduler** l&#39;attività è un **Controllo del flusso** attività. Consente di pianificare l’avvio del flusso di lavoro. Questa attività deve essere considerata come un inizio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro.

## Best practice{#scheduler-best-practices}

* Non pianificare l’esecuzione di un flusso di lavoro con una frequenza superiore a 15 minuti, in quanto ciò potrebbe impedire le prestazioni complessive del sistema e creare blocchi nel database.
* Se desideri inviare una consegna unica nel flusso di lavoro, puoi aggiungere un’attività di pianificazione e impostarla per l’esecuzione **Una volta**. Puoi anche definire **Pianificazione** nelle impostazioni della consegna.
* Se desideri inviare una consegna ricorrente nel flusso di lavoro, devi utilizzare una **Scheduler** e impostare la frequenza di esecuzione. L’attività di consegna ricorrente non ti consente di definire una pianificazione.

## Configurazione{#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validità modulo di pianificazione"
>abstract="È possibile definire un periodo di validità per lo scheduler. Può essere permanente (impostazione predefinita) o valida fino a una data specifica."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Opzioni modulo di pianificazione"
>abstract="Definisci la frequenza del modulo di pianificazione. Può essere eseguito in un determinato momento, una o più volte al giorno, settimana o mese."

Per configurare il **Scheduler** attività:

![](../assets/workflow-scheduler.png)

1. Aggiungi un **Scheduler** al flusso di lavoro.

1. Configurare **Frequenza di esecuzione**:

   * **Una volta**: il flusso di lavoro viene eseguito una sola volta.

   * **Giornaliero**: il flusso di lavoro viene eseguito una volta al giorno a un’ora specifica.

   * **Più volte al giorno:** il flusso di lavoro viene eseguito regolarmente diverse volte al giorno. Puoi impostare esecuzioni in orari specifici o periodicamente.

   * **Ogni settimana**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte alla settimana.

   * **Mensile**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte al mese. Puoi selezionare i mesi, quando devi eseguire il flusso di lavoro. Puoi anche impostare le esecuzioni in giorni settimanali specifici del mese, ad esempio il secondo martedì del mese.

1. Definisci i dettagli di esecuzione in base alla frequenza selezionata. I campi dettagliati possono variare a seconda della frequenza utilizzata (tempo, frequenza di ripetizione, giorni specificati, ecc.).

1. Clic **Anteprima orari di avvio** per controllare la pianificazione delle dieci esecuzioni successive del flusso di lavoro.

1. Definire il periodo di validità dello scheduler:

   * **Permanente (non scade mai)**: il flusso di lavoro viene eseguito, in base alla frequenza specificata, senza alcun limite all’intervallo di tempo o al numero di iterazioni.

   * **Periodo di validità**: il flusso di lavoro viene eseguito in base alla frequenza specificata, fino a una data specifica. È necessario specificare le date di inizio e di fine.

>[!NOTE]
>
>Se desideri avviare immediatamente il flusso di lavoro, puoi fare clic sul pulsante **Esegui attività in sospeso** nella barra delle azioni superiore dell&#39;utilità di pianificazione. Questo pulsante è disponibile solo quando hai avviato il flusso di lavoro.

## Esempio{#scheduler-example}

Nell’esempio seguente, l’attività è configurata in modo che il flusso di lavoro venga eseguito diverse volte al giorno alle 9 e alle 12, ogni giorno della settimana dal 1° ottobre 2023 al 1° gennaio 2024.

![](../assets/workflow-scheduler2.png)



