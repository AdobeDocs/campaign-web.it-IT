---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Modulo di pianificazione
description: Scopri come utilizzare l’attività del flusso di lavoro Modulo di pianificazione
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 058a9347329b35e49463b7d74bffa5b3c69b4a92
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 40%

---

# Modulo di pianificazione {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Attività del Modulo di pianificazione"
>abstract="L’attività del **Modulo di pianificazione** consente di pianificare quando viene avviato il flusso di lavoro. Dovresti considerare questa attività come un avvio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro."

L’attività del **Modulo di pianificazione** è un’attività di **Controllo del flusso**. Consente di pianificare quando viene avviato il flusso di lavoro. Dovresti considerare questa attività come un avvio pianificato. Può essere utilizzata solo come prima attività del flusso di lavoro.

## Best practice {#scheduler-best-practices}

* Non pianificare l’esecuzione di un flusso di lavoro con una frequenza superiore a 15 minuti, in quanto ciò potrebbe impedire le prestazioni complessive del sistema e creare blocchi nel database.
* Per inviare una consegna unica nel flusso di lavoro, aggiungi un&#39;attività di pianificazione e impostala per l&#39;esecuzione di **Una volta**. Definisci la **Pianificazione** nelle impostazioni della consegna.
* Per inviare una consegna ricorrente nel flusso di lavoro, utilizza un&#39;attività **Scheduler** e imposta la frequenza di esecuzione. L’attività di consegna ricorrente non ti consente di definire una pianificazione.

## Configurare l’attività di pianificazione {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validità del modulo di pianificazione"
>abstract="È possibile definire un periodo di validità per il modulo di pianificazione. Può essere permanente (impostazione predefinita) o valido fino a una data specifica."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Opzioni del modulo di pianificazione"
>abstract="Definisci la frequenza del modulo di pianificazione. Può essere eseguito in un determinato momento, una o più volte al giorno, alla settimana o al mese."

Per configurare l’attività del **Modulo di pianificazione**, segui questi passaggi:

![Interfaccia di configurazione attività modulo di pianificazione](../assets/workflow-scheduler.png)

1. Aggiungi un’attività del **Modulo di pianificazione** al flusso di lavoro.

1. Configura la **Frequenza di esecuzione**:

   * **Una volta**: il workflow viene eseguito una sola volta.
   * **Giornaliero**: il flusso di lavoro viene eseguito una volta al giorno a un&#39;ora specifica.
   * **Più volte al giorno**: il flusso di lavoro viene eseguito regolarmente più volte al giorno. Imposta le esecuzioni in momenti specifici o periodicamente.
   * **Settimanale**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte alla settimana.
   * **Mensile**: il flusso di lavoro viene eseguito in un determinato momento, una o più volte al mese. Seleziona i mesi in cui deve essere eseguito il flusso di lavoro. Puoi anche impostare le esecuzioni in giorni feriali specifici del mese, ad esempio il secondo martedì del mese.

1. Definisci i dettagli di esecuzione in base alla frequenza selezionata. I campi dettagliati possono variare a seconda della frequenza utilizzata (tempo, frequenza di ripetizione, giorni specificati e opzioni simili).

1. Fai clic su **Anteprima dei tempi di avvio** per controllare la pianificazione delle dieci esecuzioni successive del flusso di lavoro.

1. Definisci il periodo di validità del modulo di pianificazione:

   * **Permanente (non scade mai)**: il flusso di lavoro viene eseguito in base alla frequenza specificata, senza alcun limite all&#39;intervallo di tempo o al numero di iterazioni.
   * **Periodo di validità**: il flusso di lavoro viene eseguito in base alla frequenza specificata, fino a una data specifica. Specifica le date di inizio e fine.

>[!NOTE]
>Se si desidera avviare immediatamente il flusso di lavoro, fare clic su **Esegui attività in sospeso** nella barra delle azioni superiore della pianificazione. Questo pulsante è disponibile solo quando il flusso di lavoro è stato avviato.

## Esempio {#scheduler-example}

Nell’esempio seguente, l’attività è configurata in modo che il flusso di lavoro venga eseguito diverse volte al giorno alle 9 e alle 12, ogni giorno della settimana dal 1° ottobre 2023 al 1° gennaio 2024.

![Configurazione esempio attività modulo di pianificazione](../assets/workflow-scheduler2.png)
