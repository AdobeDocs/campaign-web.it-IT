---
audience: end-user
title: Creare una consegna di notifica push
description: Scopri come creare una consegna di notifiche push con Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 4e5840f8566fb511ef2d862833a09b581f0250c2
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 64%

---

# Creare una consegna di notifica push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modello di notifica push"
>abstract="Seleziona un modello di notifica push per avviare la consegna push. I modelli di consegna ti consentono di riutilizzare facilmente contenuti e impostazioni personalizzati in tutte le campagne e le consegne."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/start/delivery-template" text="Utilizzare i modelli di consegna"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Proprietà di consegna push"
>abstract="Definisci le proprietà di consegna push. Immetti l’etichetta del messaggio push e utilizza le **Opzioni aggiuntive** per configurare il nome interno, la cartella di consegna e il codice. Puoi anche immettere una descrizione personalizzata."

Puoi creare una consegna di notifica push autonoma o una notifica push nel contesto del flusso di lavoro di una campagna. I passaggi seguenti descrivono la procedura per una consegna push autonoma (singola). Se lavori nel contesto di un flusso di lavoro della campagna, i passaggi di creazione sono descritti in [questa sezione](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Creare una consegna push {#create-push-delivery}

Per creare una nuova consegna push autonoma, segui questi passaggi:

1. Passa al menu **[!UICONTROL Consegne]** nella barra a sinistra e fai clic sul pulsante **[!UICONTROL Crea consegna]**.

1. Nella sezione **[!UICONTROL Canale]**, scegli **Notifica push** come canale e seleziona un modello, a seconda del sistema operativo del dispositivo scelto: Android o iOS. [Ulteriori informazioni sui modelli](../msg/delivery-template.md)

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.

   ![Schermata che mostra la creazione di una consegna push](assets/push_create_1.png){zoomable="yes"}

## Configurare le impostazioni di consegna {#configure-push-settings}

Configura le impostazioni di consegna nel modo descritto di seguito:

1. Immetti un’**[!UICONTROL etichetta]** per la consegna. Per impostazione predefinita, l’etichetta viene impostata con l’etichetta del modello selezionato. Deve essere aggiornata.

1. Sfoglia le **[!UICONTROL Opzioni aggiuntive]** per personalizzare le opzioni, se necessario. Se la consegna è basata su uno schema esteso, sono disponibili campi specifici di **Opzioni personalizzate**.

   +++Configura le seguenti impostazioni in base alle tue esigenze.
   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: organizza le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura della consegna a scopo di classificazione.
   +++

1. Puoi configurare la notifica push come consegna multilingue per inviare messaggi in base alla lingua preferita di un profilo. [Ulteriori informazioni](../msg/multilingual.md).

## Selezionare il pubblico della consegna push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definire il pubblico della notifica push"
>abstract="Per definire il pubblico del messaggio, devi innanzitutto selezionare l’app associata alla consegna push. Per impostazione predefinita, la notifica push verrà inviata a tutti gli iscritti dell’applicazione. Puoi definire un pubblico specifico facendo clic sul pulsante **Seleziona pubblico**. Se necessario, aggiungi un gruppo di controllo per misurare l’impatto della consegna."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=it" text="Impostare un gruppo di controllo"

Devi innanzitutto selezionare l’app, quindi puoi perfezionare il pubblico delle notifiche push, nel modo descritto di seguito:

1. Dalla sezione **[!UICONTROL Pubblico]**, seleziona l’applicazione da utilizzare per questa consegna. Per impostazione predefinita, la notifica push verrà inviata a tutti gli iscritti dell’applicazione. Puoi definire un pubblico specifico facendo clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   ![Schermata che mostra la selezione del pubblico per la consegna push](assets/push_create_2.png){zoomable="yes"}

1. Seleziona un pubblico esistente o crea un pubblico personalizzato per perfezionare la popolazione target per la consegna push. Per la notifica push, la [dimensione di destinazione](../audience/about-recipients.md#targeting-dimensions) predefinita è **applicazione sottoscrittore** (nms:appSubscriptionRcp), collegata alla tabella dei destinatari.

   Scopri come selezionare un pubblico esistente in [questa pagina](../audience/add-audience.md).

   Scopri come creare un nuovo pubblico in [questa pagina](../audience/one-time-audience.md).

1. Attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]** per impostare un gruppo di controllo per misurare l’impatto della consegna. I messaggi non vengono inviati a tale gruppo di controllo, pertanto puoi confrontare il comportamento della popolazione che ha ricevuto il messaggio con quello dei contatti che non lo hanno fatto. [Ulteriori informazioni](../audience/control-group.md).

## Definire il contenuto delle notifiche push {#create-content-push}

Per definire il contenuto della notifica, fai clic su **[!UICONTROL Modifica contenuto]**. [Ulteriori informazioni](content-push.md).

![Schermata che mostra la modifica del contenuto per la consegna push](assets/push_create_5.png){zoomable="yes"}

Da questa schermata, è possibile anche [simulare i contenuti](../preview-test/preview-test.md) e [configurare le offerte](../msg/offers.md).

## Pianificare l’invio della consegna {#schedule-push}

Quando una consegna viene inviata nel contesto di un flusso di lavoro, è necessario utilizzare l&#39;attività **Scheduler**. Ulteriori informazioni in [questa pagina](../workflows/activities/scheduler.md). I passaggi seguenti si applicano solo alle consegne autonome.

Per pianificare una consegna push indipendente a una data e un’ora specifiche, effettua le seguenti operazioni:

1. Passa alla sezione **[!UICONTROL Pianificazione]** delle proprietà di consegna.

1. Utilizza il pulsante di attivazione **[!UICONTROL Abilita pianificazione]** per attivarla.

1. Imposta la data e l’ora desiderate per l’invio.

Dopo aver avviato la consegna, il messaggio viene inviato automaticamente nella data e nell’ora esatte definite per il destinatario.

![Schermata che mostra le opzioni di pianificazione per la consegna push](assets/push_create_3.png){zoomable="yes"}

Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-deliveries.md#gs-schedule).

## Impostazioni avanzate per la consegna {#adv-push}

Fai clic su **[!UICONTROL Configura le impostazioni di consegna]** per accedere alle opzioni avanzate relative al modello di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md).

![Schermata con le impostazioni avanzate per la consegna push](assets/push_create_4.png){zoomable="yes"}