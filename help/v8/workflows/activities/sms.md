---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro SMS
description: Scopri come utilizzare l’attività del flusso di lavoro SMS
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---


# SMS {#sms}

Il **SMS** L’attività fornisce la funzionalità per inviare messaggi SMS all’interno di un flusso di lavoro. Consente l’automazione dell’invio di SMS a una destinazione specifica determinata all’interno dello stesso flusso di lavoro.

Per definire i destinatari dell’SMS, puoi impostarli prima dell’attività di consegna SMS nel flusso di lavoro utilizzando l’attività Genera pubblico. Ulteriori informazioni.

1. Dopo aver creato e configurato un nuovo flusso di lavoro, aggiungi un’attività Genera pubblico per selezionare un pubblico esistente o utilizza il generatore di regole per definire una query personalizzata.

1. Aggiungi un’attività del canale SMS al flusso di lavoro.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Seleziona l’attività. Dal menu di consegna, seleziona i modelli che desideri utilizzare per questa consegna. Ulteriori informazioni sui modelli

1. Fai clic su Crea consegna per configurare la consegna SMS. Per ulteriori informazioni sulla consegna di SMS, consulta questa pagina.

1. Una volta che la consegna è pronta per essere inviata, torna al flusso di lavoro e fai clic su Avvia per avviarlo.

1. Per impostazione predefinita, l’avvio di un flusso di lavoro di consegna attiva la fase di preparazione dei messaggi, senza inviare immediatamente il messaggio.

   Per confermare l’invio, fai clic su Revisione e invio dal menu avanzato dell’attività SMS.

1. Dal dashboard di consegna SMS, fai clic su Invia.
