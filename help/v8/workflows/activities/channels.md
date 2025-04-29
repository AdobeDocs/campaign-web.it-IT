---
audience: end-user
title: Utilizzare un’attività di consegna nei flussi di lavoro
description: Scopri come aggiungere un’attività del flusso di lavoro di consegna (e-mail, push, SMS, direct mail)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 50%

---

# Attività di e-mail, SMS, push e direct mail {#channel}

Adobe Campaign Web consente di automatizzare ed eseguire campagne di marketing su e-mail, SMS, direct mail e canali push. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela.

Ad esempio, crea una campagna e-mail di benvenuto che includa una serie di messaggi su diversi canali, come e-mail, SMS, push e direct mail. Puoi anche inviare un’e-mail di follow-up dopo che un cliente ha completato un acquisto o inviare un messaggio di compleanno personalizzato a un cliente tramite SMS.

Utilizzando le attività dei canali, crea campagne complete e personalizzate che coinvolgono i clienti in più punti di contatto e favoriscono le conversioni.

>[!NOTE]
>
>Puoi anche creare una consegna una tantum all’esterno del contesto di un flusso di lavoro della campagna. Per ulteriori informazioni, consulta le sezioni seguenti:
>* [Creare una consegna e-mail autonoma](../../email/create-email.md)
>* [Creare una consegna SMS autonoma](../../sms/create-sms.md)
>* [Creare una consegna push autonoma](../../push/create-push.md)
>* [Crea consegna direct mailing autonoma](../../direct-mail/create-direct-mail.md)

## Prerequisiti {#channel-activity-prereq}

Inizia a creare il flusso di lavoro con le attività pertinenti:

* Prima di inserire un’attività di canale, definisci il pubblico. Il pubblico è il target principale della consegna: i profili che ricevono i messaggi. Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico del messaggio non è definito nell’attività del canale, ma all’interno di un’attività dedicata, ad esempio:

   * Un&#39;attività **Genera pubblico**. [Ulteriori informazioni](build-audience.md).

     ![Schermata che mostra l&#39;aggiunta di una consegna in un flusso di lavoro](../../msg/assets/add-delivery-in-wf.png)

   * Attività **Load file** seguita da attività **Reconciliation**. [Ulteriori informazioni](load-file.md).

     ![Schermata che mostra i criteri di riconciliazione del flusso di lavoro](../assets/workflow-reconciliation-criteria.png)

* Per inviare una consegna ricorrente, avvia il flusso di lavoro con un&#39;attività **Scheduler**. Utilizza un&#39;attività **Scheduler** per singole consegne una tantum per impostare la data di contatto per quella consegna. Tale data di contatto può essere impostata anche nelle impostazioni di consegna. Consulta [questa sezione](scheduler.md).

## Configurare l’attività Canale {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Attività e-mail"
>abstract="L’attività E-mail facilita l’invio di e-mail all’interno del flusso di lavoro, consentendo l’invio di messaggi sia una tantum che ricorrenti. Consente di automatizzare il processo di invio di e-mail a una destinazione calcolata all’interno dello stesso flusso di lavoro. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="Attività SMS"
>abstract="L’attività SMS facilita l’invio di SMS all’interno del flusso di lavoro, consentendo l’invio di messaggi sia una tantum che ricorrenti. Consente di automatizzare il processo di invio di SMS a una destinazione calcolata all’interno dello stesso flusso di lavoro. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Attività push iOS"
>abstract="L’attività Push iOS semplifica il processo di invio delle notifiche push di iOS come parte del flusso di lavoro. Consente la consegna di messaggi sia singoli che ricorrenti, automatizzando l’invio di notifiche push iOS a una destinazione predefinita all’interno dello stesso flusso di lavoro. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Attività push Android"
>abstract="L’attività Push Android semplifica il processo di invio delle notifiche push Android come parte del flusso di lavoro. Consente la consegna di messaggi sia singoli che ricorrenti, automatizzando l’invio di notifiche push Android a una destinazione predefinita all’interno dello stesso flusso di lavoro. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Attività direct mail"
>abstract="L’attività direct mail facilita l’invio con direct mail all’interno del flusso di lavoro, consentendo l’invio di messaggi sia una tantum che ricorrenti. Consente di automatizzare il processo di generazione del file di estrazione richiesto dai provider di direct mail. Puoi combinare le attività dei canali nell’area del flusso di lavoro per creare flussi di lavoro cross-channel in grado di attivare azioni basate sui dati e sul comportamento della clientela."

Per impostare una consegna nel contesto di un flusso di lavoro, segui i passaggi seguenti:

1. Aggiungi un&#39;attività del canale: **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notifica push (Android)]**, **[!UICONTROL Notifica push (iOS)]** o **[!UICONTROL Direct mail]**.

1. Seleziona il **Tipo di consegna**: singola o ricorrente.

   * Una **consegna singola** è una consegna singola inviata una sola volta, ad esempio un&#39;e-mail del Black Friday.
   * Una **consegna ricorrente** viene inviata più volte in base alla frequenza di esecuzione definita in una [attività di pianificazione](scheduler.md). Ogni volta che viene eseguito il flusso di lavoro, il pubblico viene ricalcolato e la consegna viene inviata al pubblico aggiornato con il contenuto aggiornato. Può trattarsi di una newsletter settimanale o di un’e-mail di compleanno ricorrente.

1. Seleziona un **Modello** di consegna. I modelli sono impostazioni di consegna preconfigurate specifiche di un canale. Per impostazione predefinita, per ogni canale è disponibile un modello incorporato, precompilato. [Ulteriori informazioni](../../msg/delivery-template.md)

   ![Schermata che mostra l&#39;attività di consegna in un flusso di lavoro](../assets/delivery-activity-in-wf.png)

   Seleziona il modello dal riquadro a sinistra della configurazione dell’attività del canale. Se il pubblico selezionato in precedenza non è compatibile con il canale, non puoi selezionare un modello. Per risolvere questo problema, aggiorna l’attività **Crea pubblico** per selezionare un pubblico con la mappatura target corretta. Per ulteriori informazioni sulle mappature target, consulta [questa sezione](../../audience/targeting-dimensions.md).

1. Fai clic su **Crea consegna**. Definisci le impostazioni e il contenuto del messaggio seguendo la stessa procedura con cui si crea una consegna indipendente. Testare e simulare il contenuto. [Ulteriori informazioni](../../msg/gs-messages.md)

1. Torna al flusso di lavoro. Per continuare il flusso di lavoro, attiva l&#39;opzione **Genera una transizione in uscita** per aggiungere una transizione dopo l&#39;attività del canale.

1. Fai clic su **Avvia** per avviare il flusso di lavoro.

   Per impostazione predefinita, l’avvio di un flusso di lavoro attiva la fase di preparazione dei messaggi senza inviare immediatamente il messaggio.

1. Apri l&#39;attività del canale per confermare l&#39;invio dal pulsante **Rivedi e invia**.

1. Nella dashboard della consegna, fai clic su **Invia**.

## Esempi {#cross-channel-workflow-sample}

Di seguito è riportato un esempio di flusso di lavoro cross-channel con segmentazione e due consegne. Il flusso di lavoro è destinato a tutti i clienti che vivono a Parigi e sono interessati alle macchine da caffè. Tra questa popolazione, viene inviata un’e-mail ai clienti normali e un SMS ai client VIP.

![Schermata che mostra un esempio di flusso di lavoro cross-channel](../assets/workflow-channel-example.png)

Puoi anche creare un flusso di lavoro ricorrente per inviare un SMS personalizzato ogni primo giorno del mese alle 20 a tutta la clientela che vive a Parigi.

![Schermata con un esempio di flusso di lavoro ricorrente](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->