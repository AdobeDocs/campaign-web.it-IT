---
audience: end-user
title: Preparare e inviare un’e-mail
description: Scopri come preparare e inviare un’e-mail con l’interfaccia utente web di Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 55%

---

# Preparare e inviare il messaggio e-mail {#prepare-send}

## Preparare l’invio {#prepare}

Quando definisci il tuo [contenuto](../email/edit-content.md), [pubblico](../audience/add-audience.md) e [pianificazione](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule), sei pronto per preparare la consegna delle e-mail.

Durante la preparazione della consegna, viene calcolata la popolazione target e viene generato il contenuto del messaggio per ogni profilo incluso nel target. Al termine della preparazione, i messaggi sono pronti per essere inviati immediatamente o alla data e all’ora pianificate.

Le regole di convalida utilizzate durante la preparazione della consegna sono descritte nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html?lang=it){target="_blank"}.

I passaggi principali per preparare l’invio sono elencati di seguito.

1. Dalla dashboard della consegna, fai clic su **[!UICONTROL Rivedi e invia]**.

   ![Pulsante Rivedi e invia nel dashboard di consegna](assets/email-review-and-send.png){zoomable="yes"}

1. Fai clic sul pulsante **[!UICONTROL Prepara]** nell&#39;angolo in alto a destra e conferma.

   ![Pulsante Prepara nel dashboard di consegna](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se pianifichi la consegna e disabiliti l&#39;opzione **[!UICONTROL Abilita conferma prima dell&#39;invio]**, i passaggi di preparazione e invio sono raggruppati sotto il pulsante **[!UICONTROL Prepara e invia]**. [Ulteriori informazioni sulla pianificazione](../msg/gs-deliveries.md#gs-schedule)

1. Viene visualizzato l’avanzamento della preparazione. A seconda della dimensione della popolazione target, questa operazione potrebbe richiedere del tempo.

   Puoi interrompere la preparazione in qualsiasi momento utilizzando il pulsante **[!UICONTROL Interrompi preparazione]**.

   ![Interrompi il pulsante di preparazione nel dashboard di consegna](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Durante la fase di preparazione, non vengono inviati messaggi. Puoi iniziare o interrompere senza rischiare di influire su nulla.

1. Al termine della preparazione, controlla i KPI. Se il numero di messaggi da inviare non corrisponde alle tue aspettative, modifica il pubblico e riavvia la preparazione.

   ![Schermata Preparazione completata con KPI](assets/email-preparation-complete.png){zoomable="yes"}

   Di seguito sono riportati i diversi KPI visualizzati:

   * **[!UICONTROL Destinati]**: il numero di destinatari interessati.
   * **[!UICONTROL Da consegnare]**: numero di messaggi che verranno inviati.
   * **[!UICONTROL Da escludere]**&#x200B;[: numero di messaggi esclusi da una regola di tipologia](../advanced-settings/delivery-settings.md#typology).

1. Fai clic sul pulsante **[!UICONTROL Registri]** e verifica che non siano presenti errori. L’ultimo messaggio del registro presenta eventuali messaggi di errore e il numero di errori. [Ulteriori informazioni](delivery-logs.md)

   ![Pulsante Registri nel dashboard di consegna](assets/email-prepare-logs.png){zoomable="yes"}

1. Se la preparazione rileva un errore critico che impedisce l’invio della consegna, nella dashboard delle consegne lo stato di preparazione viene visualizzato come “Non riuscito”.

   ![Stato di errore nel dashboard di consegna](assets/email-prepare-error.png){zoomable="yes"}

1. Se apporti modifiche alla consegna dopo la preparazione, riavvia la preparazione affinché tali modifiche vengano prese in considerazione.

Una volta completata la preparazione senza errori, il messaggio è pronto per essere inviato.

## Inviare il messaggio {#send}

Una volta completata la [preparazione](#prepare), puoi inviare la tua e-mail.

Se il messaggio è pianificato, viene inviato alla data e all’ora definite. [Ulteriori informazioni sulla pianificazione](../msg/gs-deliveries.md#gs-schedule)

### Inviare immediatamente {#send-immediately}

Per inviare immediatamente un’e-mail, segui la procedura indicata di seguito.

1. Nella dashboard delle consegne, fai clic sul pulsante **[!UICONTROL Invia]** in alto a destra.

   ![Pulsante Invia nel dashboard di consegna](assets/email-send.png){zoomable="yes"}

1. Conferma questa azione per inviare immediatamente il messaggio al target principale.

1. Viene visualizzato l’avanzamento dell’invio.

### Pianificare l’invio {#schedule-the-send}

Se pianifichi l’invio dell’e-mail in una data e in un’ora successive, segui i passaggi indicati di seguito.

1. Prima di fare clic sul pulsante **[!UICONTROL Rivedi e invia]**, assicurati di definire una pianificazione per l&#39;e-mail. [Ulteriori informazioni sulla pianificazione](../msg/gs-deliveries.md#gs-schedule)

1. Dal dashboard di consegna, fai clic sul pulsante **[!UICONTROL Invia come pianificato]** nell&#39;angolo in alto a destra.

   ![Pulsante Invia come pianificato nel dashboard di consegna](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Conferma invio]**. La consegna viene inviata alla data pianificata al target principale.

   >[!NOTE]
   >
   >Se disattivi l&#39;opzione **[!UICONTROL Abilita conferma prima dell&#39;invio]**, i passaggi di preparazione e invio sono raggruppati sotto il pulsante **[!UICONTROL Prepara e invia]**. [Ulteriori informazioni sulla pianificazione](../msg/gs-deliveries.md#gs-schedule)

## Sospendere o interrompere l’invio {#pause-stop-sending}

Che la consegna sia pianificata o meno<!--TBC-->, è possibile eseguire due azioni in qualsiasi momento durante il processo di invio:

* Fai clic su **[!UICONTROL Pausa invio]** per interrompere l’invio dei messaggi. Puoi riprendere l’invio in qualsiasi momento.

* Fai clic su **[!UICONTROL Interrompi invio]** per interrompere immediatamente l’invio. Una volta interrotti, né la preparazione né l’invio possono essere ripresi.

![Sospendere o interrompere l&#39;invio di pulsanti nel dashboard di consegna](assets/email-send-pause-or-stop.png){zoomable="yes"}

## Controllare i KPI {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Consegnati"
>abstract="Numero di messaggi recapitati correttamente. Questo indicatore viene aggiornato ogni 5 minuti. La percentuale visualizzata si basa sul numero totale di messaggi inviati."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/reports/kpis" text="Comprendere i KPI"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aperture"
>abstract="Numero di messaggi aperti. Questo indicatore viene aggiornato ogni 5 minuti. La percentuale visualizzata è il rapporto tra il numero di aperture distinte e il numero di messaggi consegnati."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/reports/kpis" text="Comprendere i KPI"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Clic"
>abstract="Numero di destinatari che hanno fatto clic almeno una volta nell’e-mail. Questo indicatore viene aggiornato ogni 5 minuti. La percentuale visualizzata è il rapporto tra il numero di clic distinti e il numero di messaggi consegnati."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/reports/kpis" text="Comprendere i KPI"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Inviato"
>abstract="Numero totale di messaggi elaborati durante l’analisi della consegna."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/reports/kpis" text="Comprendere i KPI"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Errori"
>abstract="Totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/reports/kpis" text="Comprendere i KPI"

Una volta completato l’invio, puoi controllare i KPI visualizzati:

![KPI visualizzati dopo l&#39;invio](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Inviato]**: numero di messaggi consegnati. La percentuale visualizzata si basa sul numero totale di messaggi da consegnare.

* **[!UICONTROL Consegnati]**: numero di messaggi recapitati correttamente. La percentuale visualizzata si basa sul numero totale di messaggi inviati.

* **[!UICONTROL Aperture]**: numero di messaggi aperti. La percentuale visualizzata corrisponde al numero di aperture distinte rispetto al numero di messaggi consegnati.

* **[!UICONTROL Clic]**: numero di destinatari che hanno fatto clic almeno una volta nell’e-mail. La percentuale visualizzata corrisponde al numero di clic distinti rispetto al numero di messaggi consegnati.

* **[!UICONTROL Errori]**: numero di e-mail con lo stato di errore. La percentuale visualizzata si basa sul numero totale di messaggi inviati.

>[!NOTE]
>
>Tutti gli indicatori vengono aggiornati ogni 5 minuti dopo l’inizio della consegna. Gli indicatori di preparazione della consegna sono in tempo reale.

Ulteriori informazioni sui KPI in [questa pagina](../reporting/kpis.md).

Puoi anche controllare i registri. [Ulteriori informazioni](delivery-logs.md)