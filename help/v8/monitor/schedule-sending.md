---
audience: end-user
title: Pianificare l’invio di una consegna
description: Scopri come pianificare una consegna
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# Pianificare l’invio di una consegna {#schedule-sending}

Puoi pianificare l’invio di una consegna. I passaggi dipendono dal fatto che si tratti di una consegna indipendente (una tantum) o se si sta lavorando nel contesto di un flusso di lavoro della campagna.

## Consegna autonoma

Per le consegne autonome, puoi pianificare direttamente la data e l’ora nella consegna.
Di seguito sono riportati alcuni esempi per ogni tipo di consegna: e-mail, sms, notifica push.

### E-mail {#schedule-email-standalone}

Per pianificare l’invio di una consegna e-mail, effettua le seguenti operazioni:

1. Nella sezione **[!UICONTROL Pianifica]** delle proprietà di consegna, attiva l&#39;interruttore **[!UICONTROL Abilita pianificazione]**

1. Imposta la data e l&#39;ora desiderate per l&#39;invio e fai clic sul pulsante **[!UICONTROL Rivedi e invia]**.

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>Per impostazione predefinita, l’opzione **[!UICONTROL Abilita la conferma prima dell’invio]** è abilitata. Questa opzione richiede di confermare l’invio prima che la consegna venga inviata alla data e all’ora pianificate. Se devi **inviare la consegna automaticamente** alla data e all&#39;ora pianificate, devi disabilitare questa opzione.
>

1. Verificare che la pianificazione sia corretta e fare clic sul pulsante **[!UICONTROL Prepara]**.

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. Una volta completata la preparazione, i messaggi sono pronti per essere inviati. Vengono visualizzate le metriche chiave per la consegna: popolazione target totale, numero di messaggi da consegnare, numero di destinatari esclusi. Fai clic sul pulsante **[!UICONTROL Invia come pianificato]** per confermare che consenti l&#39;invio della consegna alla data e all&#39;ora pianificate per la destinazione principale.

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### SMS

Per pianificare la consegna dell&#39;sms a una data e un&#39;ora specifiche, i passaggi sono gli stessi delle consegne e-mail, [vedi sopra](#schedule-email-standalone).

![](assets/schedule-sms-standalone.png){zoomable="yes"}

Puoi anche verificare che la pianificazione venga presa in considerazione:

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Notifica push

Per pianificare una consegna push autonoma a una data e un&#39;ora specifiche, i passaggi sono gli stessi delle consegne e-mail, [vedi sopra](#schedule-email-standalone).

![](assets/schedule-push-standalone.png){zoomable="yes"}

Puoi anche verificare che la pianificazione venga presa in considerazione:

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Consegna autonoma in una campagna

Puoi creare una consegna autonoma all’interno di una campagna senza utilizzare un flusso di lavoro. Puoi impostare la data e l’ora di pianificazione per questa consegna come spiegato in precedenza.
La campagna può avere la propria pianificazione, con una data di inizio e una data di fine. Questa pianificazione non interferirà con la pianificazione della consegna.

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Pianificare una consegna in un flusso di lavoro della campagna

Nel contesto di un flusso di lavoro della campagna, la **best practice** consiste nell&#39;utilizzare l&#39;attività **[!UICONTROL Scheduler]** per applicare una data e un&#39;ora per l&#39;avvio del flusso di lavoro, che implica l&#39;invio della consegna. [Ulteriori informazioni sull&#39;utilità di pianificazione](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


È necessario configurare data e ora nell&#39;attività **[!UICONTROL Scheduler]**.

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>Quando utilizzi l&#39;attività **[!UICONTROL Scheduler]** per pianificare l&#39;invio della consegna in un flusso di lavoro, **non attivare** l&#39;opzione **[!UICONTROL Abilita pianificazione]** nelle impostazioni dell&#39;attività **[!UICONTROL Delivery]**. La consegna verrà inviata automaticamente.
>

Nel caso in cui si attivi l&#39;opzione **[!UICONTROL Abilita pianificazione]** nelle impostazioni dell&#39;attività **[!UICONTROL Consegna]** e si imposti una data e un&#39;ora, la consegna verrà inviata in questa data e ora. Ciò significa che in caso di ritardo tra la data di avvio del flusso di lavoro e la data di invio, il pubblico potrebbe non essere aggiornato.
