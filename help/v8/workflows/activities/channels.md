---
audience: end-user
title: Utilizzare un’attività del flusso di lavoro di consegna
description: Scopri come aggiungere un’attività del flusso di lavoro di consegna (e-mail, push, SMS)
badge: label="Alpha"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 12%

---


# E-mail, SMS e push {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su canali e-mail, SMS e push. Puoi combinare le attività dei canali nell’area di lavoro del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare azioni in base al comportamento dei clienti e ai dati.

Ad esempio, puoi creare una campagna e-mail di benvenuto che include una serie di messaggi su diversi canali, come e-mail, SMS e push. Puoi anche inviare un’e-mail di follow-up dopo che un cliente ha completato un acquisto, o inviare un messaggio di compleanno personalizzato a un cliente tramite SMS.

Utilizzando le attività di canale, puoi creare campagne complete e personalizzate che coinvolgono i clienti in più punti di contatto e favoriscono le conversioni.

Di seguito sono riportati i passaggi per aggiungere una **Canale** attività in un workflow:

1. Assicurati di aver aggiunto un **Creare un pubblico** attività. Il pubblico è il target principale della consegna: i destinatari che ricevono i messaggi. Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico del messaggio non è definito nell’attività del canale, ma nel **Creare un pubblico** attività. Vedi [questa sezione](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Seleziona un’attività di consegna: **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notifica push (Android)]** o **[!UICONTROL Notifica push (iOS)]**.

1. Seleziona una consegna **Modello**. I modelli sono impostazioni di consegna preconfigurate, specifiche di un canale. Per ogni canale è disponibile un modello incorporato, precompilato per impostazione predefinita. [Ulteriori informazioni](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   Puoi selezionare un altro modello dal riquadro a sinistra della configurazione dell’attività del canale. Se il pubblico selezionato in precedenza non è compatibile con il canale, non puoi selezionare un modello. Per risolvere questo problema, aggiorna il **Creare un pubblico** attività per selezionare un pubblico con la mappatura target corretta. Ulteriori informazioni sulle mappature di destinazione in [Documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it){target="_blank"}.

1. Clic **Creare una consegna**. Definisci le impostazioni e il contenuto del messaggio nello stesso modo in cui crei una consegna autonoma. Puoi anche pianificare e simulare il contenuto. [Ulteriori informazioni](../../msg/gs-messages.md).

1. Torna al flusso di lavoro e salva le modifiche.

1. Clic **Inizio** per avviare il workflow.

   Per impostazione predefinita, l’avvio di un flusso di lavoro attiva la fase di preparazione dei messaggi, senza inviare immediatamente il messaggio.

1. Apri l’attività di consegna per confermare l’invio da **Rivedi e invia** pulsante.

1. Dal dashboard di consegna, fai clic su **Invia**.

## Esempio

Di seguito è riportato un esempio di flusso di lavoro cross-channel con una segmentazione e due consegne. Il flusso di lavoro è destinato a tutti i clienti che vivono a Parigi e che sono interessati alle macchine da caffè. Tra questa popolazione, viene inviata un’e-mail ai clienti regolari e un SMS ai clienti VIP.

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->