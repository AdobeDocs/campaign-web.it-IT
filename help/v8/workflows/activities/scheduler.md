---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Modulo di pianificazione
description: Scopri come utilizzare l’attività del flusso di lavoro Modulo di pianificazione
badge: label="Disponibilità limitata"
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 023777b88fa5c80e110fcf334517f7cef1c7f1ee
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 99%

---

# Modulo di pianificazione {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Attività del Modulo di pianificazione"
>abstract="L’attività del **Modulo di pianificazione** consente di pianificare quando viene avviato il flusso di lavoro. Dovresti considerare questa attività come un avvio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro."


L’attività del **Modulo di pianificazione** è un’attività di **Controllo del flusso**. Consente di pianificare quando viene avviato il flusso di lavoro. Dovresti considerare questa attività come un avvio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro.

## Best practice{#scheduler-best-practices}

* Non pianificare l’esecuzione di un flusso di lavoro con una frequenza superiore a 15 minuti, in quanto ciò potrebbe ostacolare le prestazioni complessive del sistema e creare blocchi nel database.
* Se desideri inviare una consegna unica nel flusso di lavoro, puoi aggiungere un’attività di pianificazione e impostarla per essere eseguita **una volta**. Puoi anche definire la **Pianificazione** nelle impostazioni della consegna.
* Se desideri inviare una consegna ricorrente nel flusso di lavoro, devi utilizzare un’attività del **Modulo di pianificazione** e impostare la frequenza di esecuzione. L’attività di consegna ricorrente non ti consente di definire una pianificazione.

## Configurare l’attività Scheduler {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validità del modulo di pianificazione"
>abstract="È possibile definire un periodo di validità per il modulo di pianificazione. Può essere permanente (impostazione predefinita) o valido fino a una data specifica."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Opzioni del modulo di pianificazione"
>abstract="Definisci la frequenza del modulo di pianificazione. Può essere eseguito in un determinato momento, una o più volte al giorno, alla settimana o al mese."

Per configurare l’attività del **Modulo di pianificazione**, segui questi passaggi:

![](../assets/workflow-scheduler.png)

1. Aggiungi un’attività del **Modulo di pianificazione** al flusso di lavoro.

1. Configura la **Frequenza di esecuzione**:

   * **Una volta**: il flusso di lavoro viene eseguito una sola volta.

   * **Ogni giorno**: il flusso di lavoro viene eseguito una volta al giorno a un’ora specifica.

   * **Più volte al giorno:** il flusso di lavoro viene eseguito regolarmente diverse volte al giorno. Puoi impostare esecuzioni in orari specifici o periodicamente.

   * **Settimanalmente**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte alla settimana.

   * **Mensilmente**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte al mese. Puoi selezionare i mesi in cui desideri che il flusso di lavoro sia eseguito. Puoi anche impostare le esecuzioni in un giorno feriale specifico del mese, ad esempio il secondo martedì del mese.

1. Definisci i dettagli di esecuzione in base alla frequenza selezionata. I campi dettagliati possono variare a seconda della frequenza utilizzata (tempo, frequenza di ripetizione, giorni specificati, ecc.).

1. Fai clic su **Anteprima dei tempi di avvio** per controllare la pianificazione delle dieci esecuzioni successive del flusso di lavoro.

1. Definisci il periodo di validità del modulo di pianificazione:

   * **Permanente (nessuna scandenza)**: il flusso di lavoro viene eseguito in base alla frequenza specificata, senza alcun limite all’arco temporale o al numero di iterazioni.

   * **Periodo di validità**: il flusso di lavoro viene eseguito in base alla frequenza specificata, fino a una data specifica. È necessario specificare le date di inizio e di fine.

>[!NOTE]
>
>Se desideri avviare immediatamente il flusso di lavoro, puoi fare clic sul pulsante **Esegui attività in sospeso** nella barra delle azioni superiore del modulo di pianificazione. Questo pulsante è disponibile solo quando hai avviato il flusso di lavoro.

## Esempio{#scheduler-example}

Nell’esempio seguente, l’attività è configurata in modo che il flusso di lavoro venga eseguito diverse volte al giorno alle 9 e alle 12, ogni giorno della settimana dal 1° ottobre 2023 al 1° gennaio 2024.

![](../assets/workflow-scheduler2.png)
