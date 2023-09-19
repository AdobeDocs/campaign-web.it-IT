---
audience: end-user
title: Utilizzare un’attività di consegna nei flussi di lavoro
description: Scopri come aggiungere un’attività di consegna (e-mail, push, SMS) nei flussi di lavoro
badge: label="Beta"
source-git-commit: 2894766336d5ac52625175981c6969a0ac5882d8
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 61%

---


# Attività di e-mail, SMS e push {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su canali e-mail, SMS e push. Puoi combinare più attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare specifiche azioni in base al comportamento dei clienti.

Ad esempio, puoi creare una campagna e-mail di benvenuto che include una serie di messaggi su diversi canali, come e-mail, SMS e push. Puoi anche inviare un’e-mail di follow-up dopo che un cliente ha completato un acquisto o inviare un messaggio di auguri di compleanno personalizzato a un cliente tramite SMS.

Utilizzando le attività dei canali, puoi creare campagne complete e personalizzate che coinvolgono i clienti su più punti di contatto e danno impulso alle conversioni.

>[!NOTE]
>
>Puoi anche creare una consegna una tantum, al di fuori del contesto di un flusso di lavoro della campagna. Per ulteriori informazioni, consulta le sezioni seguenti:
>* [Creare la consegna e-mail autonoma](../../email/create-email.md)
>* [Creare una consegna SMS indipendente](../../sms/create-sms.md)
>* [Creare una consegna push autonoma](../../push/create-push.md)

## Creare il flusso di lavoro{#build-your-workflow}

Inizia a creare il flusso di lavoro con le attività pertinenti prima di inserire la consegna:

* Se desideri inviare una consegna ricorrente, avvia il flusso di lavoro con una **Scheduler** attività. Se desideri inviare una consegna unica, puoi definire la data di contatto utilizzando una **Scheduler** o definisci la pianificazione nelle impostazioni della consegna. Consulta [questa sezione](scheduler.md).

* Aggiungi un’attività **Crea pubblico.** Il pubblico è il target principale della consegna: i destinatari che ricevono i messaggi. Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico del messaggio non è definito nell’attività del canale, ma nell’attività **Crea pubblico**. Consulta [questa sezione](build-audience.md).

  ![](../../msg/assets/add-delivery-in-wf.png)

## Configurare l’attività Canale {#create-a-delivery-in-a-workflow}


>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Attività e-mail"
>abstract="Automatizza ed esegui campagne di marketing su canali e-mail, SMS e push. Puoi combinare più attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare specifiche azioni in base al comportamento dei clienti."


>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="Attività SMS"
>abstract="Automatizza ed esegui campagne di marketing su canali e-mail, SMS e push. Puoi combinare più attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare specifiche azioni in base al comportamento dei clienti."


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Attività push iOS"
>abstract="Automatizza ed esegui campagne di marketing su canali e-mail, SMS e push. Puoi combinare più attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare specifiche azioni in base al comportamento dei clienti."


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Attività push Android"
>abstract="Automatizza ed esegui campagne di marketing su canali e-mail, SMS e push. Puoi combinare più attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel che possono attivare specifiche azioni in base al comportamento dei clienti."

Per impostare una consegna nel contesto di un flusso di lavoro, segui i passaggi seguenti:

1. Aggiungi un’attività di canale: **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notifica push (Android)]** o **[!UICONTROL Notifica push (iOS)]**.

1. Seleziona la **Tipo di consegna**: singolo o ricorrente.

   * **Consegna singola**: si tratta di una consegna in un’unica soluzione, inviata una sola volta, ad esempio un’e-mail del Black Friday.
   * **Consegna ricorrente**: per questo tipo di consegna, imposta la frequenza di esecuzione utilizzando una [attività di pianificazione](scheduler.md). Ogni volta che viene eseguito il flusso di lavoro, il pubblico viene ricalcolato e la consegna viene inviata con il contenuto aggiornato. Può trattarsi di una newsletter settimanale o di un’e-mail di compleanno ricorrente.

1. Seleziona un **Modello** di consegna. I modelli sono impostazioni di consegna preconfigurate, specifiche per un canale. Per ogni canale è disponibile un modello incorporato, precompilato per impostazione predefinita. [Ulteriori informazioni](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   Puoi selezionare un altro modello dal riquadro a sinistra della configurazione dell’attività del canale. Se il pubblico selezionato in precedenza non è compatibile con il canale, non puoi selezionare un modello. Per risolvere questo problema, aggiorna l’attività **Crea pubblico** per selezionare un pubblico con la mappatura target corretta. Per ulteriori informazioni sulle mappature di destinazione, consulta la [documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=it){target="_blank"}.

1. Fai clic su **Crea consegna**. Definisci le impostazioni e il contenuto del messaggio seguendo la stessa procedura con cui si crea una consegna indipendente. Puoi anche pianificare e simulare il contenuto. [Ulteriori informazioni](../../msg/gs-messages.md).

1. Torna al workflow. Scegli se desideri continuare il flusso di lavoro **Generare una transizione in uscita** se desideri aggiungere una transizione dopo l’attività del canale.

1. Fai clic su **Avvia** per avviare il flusso di lavoro.

   Per impostazione predefinita, l’avvio di un flusso di lavoro di consegna attiva la fase di preparazione dei messaggi, senza inviare immediatamente il messaggio.

1. Apri l’attività di consegna per confermare l’invio, mediante il pulsante **Rivedi e invia**.

1. Nella dashboard della consegna, fai clic su **Invia**.

## Esempi {#cross-channel-workflow-sample}

Di seguito è riportato un esempio di flusso di lavoro cross-channel con una segmentazione e due consegne. Il flusso di lavoro esegue il targeting di tutti i clienti che vivono a Parigi e che sono interessati alle macchine da caffè. Tra questa popolazione, viene inviata un’e-mail ai clienti regolari e un SMS ai clienti VIP.

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

Puoi anche creare un flusso di lavoro ricorrente per inviare un SMS personalizzato ogni primo giorno del mese alle 20 a tutti i clienti che vivono a Parigi.

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
