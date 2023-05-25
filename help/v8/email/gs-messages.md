---
audience: end-user
title: Introduzione ai messaggi e alle consegne in Campaign v8 Web
description: Scopri come utilizzare le consegne e inviare messaggi con Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 9f9b5b9ce08aa50986c75f1dd3afba8e2bc4f700
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 34%

---

# Introduzione ai messaggi in Campaign Web {#gs-messages}

Con Adobe Campaign, puoi inviare campagne cross-channel tra cui e-mail, SMS e notifiche push e misurarne l’efficacia utilizzando vari rapporti dedicati. Questi messaggi sono progettati e inviati tramite consegna e possono essere personalizzati per ogni destinatario. Queste consegne possono essere autonome o incluse nel contesto di una campagna di marketing.

Adobe Campaign v8 è dotato dei canali di consegna seguenti:

* **Canale e-mail**: le consegne e-mail ti consentono di inviare e-mail personalizzate alla popolazione target. Scopri come creare e inviare un’e-mail in [questa pagina](../email/create-email.md).

* **Canale SMS**: le consegne sui canali mobili ti consentono di inviare SMS personalizzati alla popolazione target.  Scopri come creare e inviare SMS in [questa pagina](../sms/create-sms.md).

* **Canale dell’app mobile**: le consegne tramite app mobile ti consentono di inviare notifiche ai sistemi iOS e Android.  Scopri come creare e inviare notifiche push in [questa pagina](../push/gs-push.md).

## Creare una consegna

Puoi creare consegne autonome dalla **Consegne** menu a sinistra, o creare consegne nel contesto di una campagna di marketing, dal menu **Campagne** menu a sinistra.

>[!BEGINTABS]

>[!TAB Creare una consegna autonoma]

Per creare una consegna autonoma, segui questi passaggi:

1. Accedi a **[!UICONTROL Consegne]** nel menu di navigazione a sinistra, quindi fai clic su **[!UICONTROL Creare una consegna]** pulsante.
1. Scegli un canale per la consegna. Per ulteriori informazioni sui canali di consegna e su come definirne il contenuto, consulta queste sezioni:

   * [Canale e-mail](../email/create-email.md)
   * [Canale di notifica push](../push/gs-push.md)
   * [Canale SMS](../sms/create-sms.md)

1. Definisci il pubblico della consegna per il target principale e il gruppo di controllo. Ulteriori informazioni sui tipi di pubblico in [questa sezione](../audience/about-audiences.md).
1. Definisci il contenuto del messaggio.
1. (facoltativo) definisci la pianificazione della consegna. Se non è definita alcuna pianificazione, i messaggi vengono inviati immediatamente dopo aver fatto clic sul pulsante **[!UICONTROL Invia]** pulsante.
1. Fai clic su  **[!UICONTROL Rivedi e invia]** per controllare le impostazioni.
1. Utilizza il  **[!UICONTROL Simula contenuto]** per testare la consegna e le impostazioni di personalizzazione. Ulteriori informazioni sulla simulazione dei messaggi in [questa sezione](../preview-test/preview-test.md).
1. Fai clic su  **[!UICONTROL Prepara]** per calcolare la popolazione target e generare i messaggi. Il passaggio di preparazione può richiedere alcuni minuti. Una volta completata la preparazione, i messaggi sono pronti per l’invio. In caso di errore, passa a **Registri** per controllare avvisi e avvisi.
1. Controllare i risultati e fare clic su  **[!UICONTROL Invia]** per iniziare a inviare messaggi.
1. Una volta inviati i messaggi, passa alla sezione Rapporti per accedere alle metriche chiave. Ulteriori informazioni sui rapporti di consegna in [questa sezione](../reporting/reports.md).

>[!TAB Creare una consegna in una campagna]

Per creare una consegna in una campagna, effettua le seguenti operazioni:

1. Crea una campagna o aprila.
1. Crea un flusso di lavoro o aprilo esistente.
1. Aggiungere e configurare un **Creare un pubblico** e fai clic sul pulsante `+`pulsante.
   ![](assets/add-delivery-in-wf.png)
1. Seleziona un’attività di consegna: e-mail, SMS, notifica push (Android) o notifica push (iOS). Per ulteriori informazioni sui canali di consegna e su come definirne il contenuto, consulta queste sezioni:

   * [Canale e-mail](../email/create-email.md)
   * [Canale di notifica push](../push/gs-push.md)
   * [Canale SMS](../sms/create-sms.md)

1. Avvia il flusso di lavoro e controlla i registri.

Per ulteriori informazioni su come configurare una campagna,

>[!ENDTABS]


## Scegli come inviare i messaggi{#gs-send-msg}

Dopo aver creato il messaggio e averne progettato e testato il relativo contenuto, puoi scegliere come inviarlo.

Campaign offre una serie di funzionalità per:

* Inviare messaggi manualmente al target principale

* Inviare messaggi associati a una [campagna di marketing](../campaigns/gs-campaigns.md)

* Inviare messaggi tramite un [flusso di lavoro](../workflows/channel-activities.md)


## Aggiungere personalizzazione{#personalization}

I messaggi consegnati da Adobe Campaign possono essere personalizzati in vari modi


## Registri di consegna e di tracciamento{#gs-tracking-logs}

Il monitoraggio delle consegne dopo l’invio è un passaggio fondamentale per garantire l’efficienza delle campagne di marketing e l’effettivo raggiungimento dei clienti. Puoi monitorare una consegna, oltre a capire come vengono gestiti errori e quarantene.
