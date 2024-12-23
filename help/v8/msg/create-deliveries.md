---
product: campaign
title: Utilizzare le consegne
description: Scopri come creare la prima consegna in Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 803a20ac-e75f-45c6-af89-054b84eb3405
source-git-commit: 387a69abf4b97cd202c1a7e24bcf14c6af442714
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 89%

---

# Creare una consegna {#create-delivery}

Puoi creare consegne autonome dal menu a sinistra **[!UICONTROL Consegne]**, oppure nel contesto di un flusso di lavoro, incluso o meno in una campagna.

Sfoglia le schede seguenti per scoprire come creare una consegna:

>[!BEGINTABS]

>[!TAB Creare una consegna indipendente]

Per creare una consegna indipendente, effettua le seguenti operazioni:

1. Passa al menu **[!UICONTROL Consegne]** nella navigazione a sinistra, quindi fai clic sul pulsante **[!UICONTROL Crea consegna]**.

   ![](assets/create-a-delivery.png){zoomable="yes"}

1. Scegli un canale per la consegna.
1. Definisci il pubblico della consegna per il target principale e il gruppo di controllo. [Ulteriori informazioni sui tipi di pubblico](../audience/about-recipients.md)

   ![](assets/select-audience.png){zoomable="yes"}{width="70%" align="left"}

1. Definisci il contenuto del messaggio. Per ulteriori informazioni sui canali di consegna e su come definirne il contenuto, consulta queste sezioni:

   * [Canale e-mail](../email/create-email.md)
   * [Canale di notifica push](../push/gs-push.md)
   * [Canale SMS](../sms/create-sms.md)

1. (facoltativo) Definisci la [pianificazione](#gs-schedule) della consegna. Se non è definita alcuna pianificazione, i messaggi vengono inviati immediatamente dopo aver fatto clic sul pulsante **[!UICONTROL Invia]**.
1. Fai clic sul pulsante **[!UICONTROL Rivedi e invia]** per verificare le impostazioni.
1. Utilizza il pulsante **[!UICONTROL Simula contenuto]** per verificare la consegna e le impostazioni di personalizzazione. Per ulteriori informazioni sulla simulazione di messaggi, consulta [questa sezione](../preview-test/preview-test.md).
1. Fai clic sul pulsante **[!UICONTROL Prepara]** per calcolare la popolazione target e generare i messaggi. La fase di preparazione può richiedere alcuni minuti. Una volta completata la preparazione, i messaggi sono pronti per l’invio. In caso di errore, passa a **Registri** per controllare avvisi e avvertenze.
1. Controllare i risultati e fare clic sul pulsante **[!UICONTROL Invia]** per iniziare a inviare messaggi.
1. Una volta inviati i messaggi, passa alla sezione **Rapporti** per accedere alle metriche chiave. Per ulteriori informazioni sui rapporti sulle consegne, consulta [questa sezione](../reporting/delivery-reports.md).

>[!TAB Creare una consegna in un flusso di lavoro]

Per creare una consegna in un flusso di lavoro, segui questi passaggi:

1. Crea un flusso di lavoro o apri un flusso di lavoro esistente. [Ulteriori informazioni sui workflow](../workflows/gs-workflow-creation.md#gs-workflow-steps)
1. Aggiungi e configura un&#39;attività [**[!UICONTROL Genera pubblico]**](../workflows/activities/build-audience.md).
1. Fai clic sull’icona `+` e seleziona un’attività di consegna: **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notifica push (Android)]** o **[!UICONTROL Notifica push (iOS)]**. Ulteriori informazioni sulle attività dei canali di consegna in un flusso di lavoro e su come definire un contenuto di consegna in [questa sezione](../workflows/activities/channels.md).

   ![](assets/add-delivery-in-wf.png){zoomable="yes"}

1. Avvia il flusso di lavoro e controlla i registri.

Puoi anche aggiungere consegne in una campagna senza creare un flusso di lavoro. A questo scopo, passa alla scheda **[!UICONTROL Consegne]** della campagna e fai clic sul pulsante **[!UICONTROL Crea consegna]**.

![](assets/new-campaign-delivery.png){zoomable="yes"}

I passaggi di configurazione sono simili a quelli per le consegne indipendenti.

Per ulteriori informazioni su come configurare una campagna e gestire le consegne che appartengono a una campagna, consulta [questa sezione](../campaigns/gs-campaigns.md).

>[!ENDTABS]

## Aggiungere la personalizzazione {#personalization}

I messaggi consegnati da Adobe Campaign possono essere personalizzati in vari modi. [Ulteriori informazioni sulle funzionalità di personalizzazione](../personalization/gs-personalization.md).

Utilizza Campaign per creare contenuti dinamici e inviare messaggi personalizzati. Le funzionalità di personalizzazione possono essere combinate per migliorare i messaggi e creare un’esperienza utente personalizzata.

Puoi personalizzare il contenuto del messaggio in diversi modi:

* Inserendo **campi di personalizzazione** dinamici

  I campi di personalizzazione vengono utilizzati per la personalizzazione di primo livello dei messaggi. Puoi selezionare qualsiasi campo disponibile nel database dall’editor di personalizzazione. Per una consegna, puoi selezionare qualsiasi campo correlato al destinatario, al messaggio o alla consegna. Questi attributi di personalizzazione possono essere inseriti nella riga dell’oggetto o nel corpo dei messaggi. [Ulteriori informazioni](../personalization/personalize.md)

* Inserimento di **frammenti di espressione predefiniti**

  Campaign viene fornito con un set di frammenti di espressione che contengono un rendering specifico che puoi inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di auguri o un collegamento alla pagina mirror del messaggio. i frammenti di espressione sono disponibili da una voce dedicata nell’editor di personalizzazione. Inoltre, puoi anche creare frammenti di espressione personalizzati in base alle tue esigenze. [Scopri come utilizzare i frammenti di espressione](../content/use-expression-fragments.md)

* Creare **contenuto condizionale**

  Configura il contenuto condizionale per aggiungere la personalizzazione dinamica, ad esempio in base al profilo del destinatario. I blocchi di testo e/o le immagini vengono inseriti quando viene soddisfatta una particolare condizione. [Ulteriori informazioni](../personalization/conditions.md)

* Aggiungere **offerte personalizzate**

  Inserisci offerte personalizzate nel contenuto del messaggio, a seconda della posizione del destinatario, del meteo corrente o dell’ultimo ordine di acquisto. [Ulteriori informazioni](../msg/offers.md)

## Anteprima e verifica delle consegne

Una volta definito il contenuto del messaggio, puoi visualizzarne l’anteprima per controllare il rendering dei messaggi e verificare le impostazioni di personalizzazione con i profili di test. [Ulteriori informazioni](../preview-test/preview-test.md)

## Pianificare l’invio della consegna {#gs-schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Imposta una data e un’ora di contatto"
>abstract="Definisci la data e l’ora esatta dell’invio della consegna. Scegliendo l’orario più appropriato per il messaggio di marketing, puoi ottimizzare i tassi di apertura."

Puoi impostare la data e l’ora esatta per l’invio dei messaggi. Scegliendo l’orario più appropriato per il messaggio di marketing, puoi ottimizzare i tassi di apertura.

Per pianificare l’invio dell’e-mail, apri la consegna e passa alla sezione **[!UICONTROL Pianificazione]**. Utilizza l’interruttore **[!UICONTROL Abilita pianificazione]** per attivarla e imposta la data e l’ora desiderate per l’invio. Una volta inviata la consegna, l’invio effettivo inizierà dalla data di contatto definita.

![](assets/schedule.png){zoomable="yes"}

Per impostazione predefinita, l’opzione **[!UICONTROL Abilita la conferma prima dell’invio]** è abilitata. Questa opzione richiede di confermare l’invio prima che la consegna venga inviata alla data e all’ora pianificate. Se desideri inviare la consegna automaticamente alla data e all’ora pianificate, puoi disattivare questa opzione.

Scopri i passaggi su come inviare una consegna pianificata in [questa sezione](../monitor/prepare-send.md#schedule-the-send).

## Registri di monitoraggio e di tracciamento {#gs-tracking-logs}

Il monitoraggio delle consegne dopo l’invio è un passaggio fondamentale per garantire l’efficienza delle campagne di marketing e l’effettivo raggiungimento dei clienti.

Puoi monitorare una consegna, oltre a capire come vengono gestiti errori e quarantene.

Scopri le funzionalità di monitoraggio e tracciamento in [questa sezione](../reporting/gs-reports.md).
