---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Notifica push
description: Scopri come utilizzare l’attività del flusso di lavoro Notifica push
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '324'
ht-degree: 100%

---


# Notifica push {#push-activity}

L’attività di consegna **Notifica push** ti consente di configurare l’invio di una notifica push in un flusso di lavoro.

>[!BEGINTABS]

>[!TAB Notifica push (Android)]

1. Dopo aver creato e configurato un nuovo flusso di lavoro, aggiungi un’attività Creazione del pubblico per selezionare un pubblico esistente o utilizza il generatore di regole per definire una query personalizzata.

1. Aggiungi un’attività del canale di notifica push (Android) nel flusso di lavoro.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Seleziona l’attività. Dal menu di consegna, seleziona i modelli che desideri utilizzare per questa consegna. Ulteriori informazioni sui modelli

1. Fai clic su Crea consegna per configurare la consegna della notifica push. Per ulteriori informazioni sulla consegna delle notifiche push (Android), consulta questa pagina.

1. Una volta che la consegna è pronta per essere inviata, torna al flusso di lavoro e fai clic su Avvia per avviarlo.

1. Per impostazione predefinita, l’avvio di un flusso di lavoro di consegna attiva la fase di preparazione dei messaggi, senza inviare immediatamente il messaggio.

   Per confermare l’invio, fai clic su Rivedi e invia dal menu avanzato dell’attività del canale per le notifiche push (Android).

1. Dalla dashboard di consegna delle notifiche push, fai clic su Invia.

>[!TAB Notifica push (iOS)]

1. Dopo aver creato e configurato un nuovo flusso di lavoro, aggiungi un’attività Creazione del pubblico per selezionare un pubblico esistente o utilizza il generatore di regole per definire una query personalizzata.

1. Aggiungi un’attività del canale di notifica push (iOS) nel flusso di lavoro.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Seleziona l’attività. Dal menu di consegna, seleziona i modelli che desideri utilizzare per questa consegna. Ulteriori informazioni sui modelli

1. Fai clic su Crea consegna per configurare la consegna della notifica push. Per ulteriori informazioni sulla consegna delle notifiche push (iOS), consulta questa pagina.

1. Una volta che la consegna è pronta per essere inviata, torna al flusso di lavoro e fai clic su Avvia per avviarlo.

1. Per impostazione predefinita, l’avvio di un flusso di lavoro di consegna attiva la fase di preparazione dei messaggi, senza inviare immediatamente il messaggio.

   Per confermare l’invio, fai clic su Rivedi e invia dal menu avanzato dell’attività del canale per le notifiche push (iOS).

1. Dalla dashboard di consegna delle notifiche push, fai clic su Invia.

>[!ENDTABS]