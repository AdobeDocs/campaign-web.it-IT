---
audience: end-user
title: Inviare la prima e-mail
description: Scopri come inviare la prima e-mail con l’interfaccia utente web di Campaign
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 83%

---


# Creare il primo messaggio e-mail {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Introduzione alle e-mail"
>abstract="Puoi creare una consegna e-mail autonoma o un messaggio e-mail nel contesto di un flusso di lavoro della campagna. Scopri come creare la consegna, selezionare il pubblico e progettare il contenuto dell’e-mail."

Scopri come creare la tua prima e-mail con targeting. In questo caso d’uso, viene pianificato l’invio di un’e-mail ai membri fidelizzati Silver e Gold in una data specifica.

In base a un [modello di progettazione](../email/create-email-templates.md) predefinito, l’e-mail presenta anche contenuti personalizzati in base agli attributi del profilo cliente.

➡️ [Scopri questa funzione nel video](#video)

## Creare una consegna e-mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selezionare un modello di e-mail"
>abstract="Un modello e-mail è una configurazione di consegna specifica che contiene impostazioni predefinite, ad esempio regole di tipologia e parametri di personalizzazione o di indirizzamento. I modelli sono definiti nella console client di Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Definire le proprietà dell’e-mail"
>abstract="Le proprietà sono i parametri di consegna comuni che consentono di denominare e classificare la consegna. Le impostazioni aggiuntive sono facoltative. Se la consegna è basata su uno schema esteso definito nella console Adobe Campaign v8, sono disponibili alcuni campi specifici di **Opzioni personalizzate**."

Puoi creare una consegna e-mail autonoma o un messaggio e-mail nel contesto di un flusso di lavoro della campagna. I passaggi seguenti descrivono la procedura per una consegna e-mail autonoma (singola). Ulteriori informazioni sui passaggi per la creazione della consegna in Adobe Campaign sono disponibili in [questa pagina](../msg/gs-deliveries.md).

Per creare una nuova consegna e-mail autonoma, segui i passaggi indicati di seguito.

1. Passa al menu **[!UICONTROL Consegne]** nella barra di navigazione a sinistra, quindi fai clic sul pulsante **[!UICONTROL Crea consegna]**.

   ![](../msg/assets/create-a-delivery.png)

1. Seleziona il canale **[!UICONTROL E-mail]** e scegli un modello di consegna e-mail dall’elenco.

   >[!NOTE]
   >
   >I modelli sono impostazioni di consegna preconfigurate e salvate per poter essere riutilizzate. [Ulteriori informazioni](../msg/delivery-template.md)

   ![](assets/channel-template.png){zoomable="yes"}

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.
1. Specifica un’etichetta per la consegna e configura opzioni aggiuntive in base alle tue esigenze:

   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: utilizza questo campo per organizzare le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura dell’e-mail a scopo di classificazione.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Se hai esteso lo schema con campi personalizzati specifici, puoi accedervi nella sezione **[!UICONTROL Opzioni personalizzate]**.

   ![](assets/email-properties.png){zoomable="yes"}

1. Inoltre, è possibile accedere alle impostazioni avanzate, come le regole di tipologia e le mappature dei target, tramite il pulsante **[!UICONTROL Impostazioni]** che si trova in alto a destra della schermata. Queste impostazioni sono preconfigurate nel modello selezionato, ma possono essere modificate in base alle esigenze per questo specifico messaggio e-mail. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

## Definire il pubblico {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Selezionare un pubblico per la consegna"
>abstract="Seleziona il pubblico migliore per il messaggio di marketing. Puoi scegliere un pubblico esistente (già definito in un’istanza di Campaign v8 o da Adobe Experience Platform), creare un nuovo pubblico utilizzando il query modeler oppure caricare un file contenente il pubblico. I gruppi di controllo non sono abilitati per l’opzione **Seleziona da file** e viceversa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=it" text="Selezionare il pubblico principale"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=it" text="Impostare un gruppo di controllo"

In questo caso d’uso, l’e-mail verrà inviata a un pubblico esistente.

Per istruzioni su come lavorare con i tipi di pubblico, consulta [questa sezione](../audience/about-recipients.md).

1. Per selezionare il pubblico a cui inviare l’e-mail, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]** e scegli un pubblico esistente tra quelli elencati.

   In questo esempio, verrà utilizzato un pubblico di targeting esistente per i clienti appartenenti ai livelli di punti fedeltà Silver e Gold.

   ![](assets/create-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >I tipi di pubblico disponibili nell’elenco provengono dall’istanza Campaign v8 oppure, se nell’istanza è stata configurata l’integrazione Destinazione/Origine, da Adobe Experience Platform. Questa integrazione consente di inviare segmenti di Experience Platform ad Adobe Campaign e di inviare i registri di consegna e tracciamento di Campaign ad Adobe Experience Platform. Scopri come utilizzare Campaign e Adobe Experience Platform, consultando la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.

1. Una volta selezionato il pubblico, puoi perfezionare ulteriormente il target applicando regole aggiuntive.

   ![](assets/audience-selected.png){zoomable="yes"}

1. Puoi anche impostare un gruppo di controllo per analizzare il comportamento dei destinatari delle e-mail rispetto a quelli non interessati dal targeting. [Scopri come utilizzare i gruppi di controllo](../audience/control-group.md)

## Definire il contenuto dell’e-mail {#create-content}

Per iniziare a creare il contenuto delle e-mail, segui i passaggi seguenti. In questo caso d’uso, per progettare l’e-mail viene utilizzato un [modello di consegna](../msg/delivery-template.md) e-mail già definito.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Nella dashboard della consegna e-mail, fai clic sul pulsante **[!UICONTROL Modifica contenuto]**.

   ![](assets/email-edit-content.png){zoomable="yes"}

   Viene visualizzata un’interfaccia dedicata in cui puoi configurare il contenuto dell’e-mail e accedere a E-mail designer. [Ulteriori informazioni](edit-content.md)

   ![](assets/edit-content.png){zoomable="yes"}

1. Immetti l’oggetto dell’e-mail e personalizzalo utilizzando l’editor di espressioni. [Scopri come personalizzare i contenuti](../personalization/personalize.md)

   ![](assets/subject-line.png){zoomable="yes"}

1. Per progettare il contenuto dell’e-mail, fai clic sul pulsante **[!UICONTROL Modifica corpo e-mail]**.

   Scegli il metodo da utilizzare per creare il contenuto delle e-mail. In questo esempio, utilizza un [modello di contenuto già definito](create-email-templates.md).

   ![](assets/select-template.png){zoomable="yes"}

1. Dopo aver selezionato il modello, questo viene visualizzato in [E-mail designer](create-email-content.md), dove puoi apportare le modifiche necessarie e aggiungere la personalizzazione.

   Ad esempio, per aggiungere la personalizzazione al titolo dell’e-mail, seleziona il blocco del componente e fai clic su **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/add-perso.png){zoomable="yes"}

1. Una volta ottenuto il contenuto desiderato, salva e chiudi il progetto. Fai clic su **[!UICONTROL Salva]** per tornare alla schermata di creazione dell’e-mail.

   ![](assets/save-content.png){zoomable="yes"}

## Pianificare l’invio {#schedule}

Quando una consegna viene inviata nel contesto di un flusso di lavoro, è necessario utilizzare l&#39;attività **Scheduler**. Ulteriori informazioni in [questa pagina](../workflows/activities/scheduler.md). I passaggi seguenti si applicano solo alle consegne autonome.

1. Passa alla sezione **[!UICONTROL Pianificazione]** delle proprietà di consegna.

1. Utilizza l’opzione **[!UICONTROL Abilita pianificazione]** per attivarla.

1. Imposta la data e l’ora desiderate per l’invio.

   ![](assets/schedule.png){zoomable="yes"}

Una volta inviata la consegna, l’invio effettivo inizia dalla data di contatto definita.

Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Anteprima di un’e-mail e invio di bozze {#preview-test}

Prima di inviare l’e-mail, puoi visualizzarla in anteprima e testarla per assicurarti che soddisfi le tue aspettative.

In questo caso d’uso, puoi visualizzare in anteprima il messaggio e-mail e inviare bozze a indirizzi e-mail specifici, rappresentando al contempo alcuni dei profili target.

Ulteriori informazioni su come visualizzare in anteprima un&#39;e-mail e inviare bozze sono disponibili in [questa sezione](../preview-test/preview-test.md).

1. Per esaminare l’e-mail, fai clic su **[!UICONTROL Rivedi e invia]**. Viene visualizzata un’anteprima del messaggio e-mail, nonché tutte le proprietà, il pubblico e la pianificazione configurati. Per modificare uno di questi elementi, fai clic sul pulsante Modifica.

1. Per visualizzare l&#39;anteprima dell&#39;e-mail e inviare le bozze, fare clic sul pulsante **[!UICONTROL Simula contenuto]**.

   ![](assets/review-email.png){zoomable="yes"}

1. Sul lato sinistro, seleziona i profili da utilizzare per visualizzare l’anteprima del messaggio e-mail.

   Nel riquadro a destra viene visualizzata un’anteprima del messaggio e-mail in base al profilo selezionato. Se hai aggiunto più profili, puoi passare da un profilo all’altro per visualizzare in anteprima l’e-mail corrispondente.

   ![](assets/preview.png){zoomable="yes"}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Per inviare le bozze, fai clic sul pulsante **[!UICONTROL Invia bozze]**, quindi scegli la modalità da utilizzare.

   In questo esempio, utilizza la modalità **[!UICONTROL Sostituisci da destinazione principale]**, che invia bozze a indirizzi e-mail specifici impersonando alcuni dei profili target dell&#39;e-mail.

   ![](assets/proof-mode.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi indirizzo]** e specifica gli indirizzi e-mail che ricevono le bozze.

   Per ogni indirizzo e-mail, seleziona il profilo da impersonare. Puoi anche consentire ad Adobe Campaign di selezionare un profilo casuale dal target.

   ![](assets/proof-test-profile.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Invia bozza]** e conferma l&#39;invio.

   Le bozze vengono inviate agli indirizzi e-mail specificati utilizzando il profilo selezionato con il prefisso **[Proof x]**.

   ![](assets/proof-sent.png){zoomable="yes"}

   Puoi controllare lo stato dell&#39;invio e accedere alle bozze inviate in qualsiasi momento facendo clic sul pulsante **[!UICONTROL Visualizza bozze]** nella schermata simula contenuto.

## Inviare e monitorare l’e-mail {#prepare-send}

Dopo aver rivisto e testato l’e-mail, puoi avviarne la preparazione e inviarla.

1. Per avviare la preparazione dell’e-mail, fai clic su **[!UICONTROL Prepara]**. [Scopri come preparare un’e-mail](../monitor/prepare-send.md)

   ![](assets/preparation.png){zoomable="yes"}

1. Quando l’e-mail è pronta per essere inviata, fai clic sul pulsante **[!UICONTROL Invia]** (oppure su **[!UICONTROL Invia come pianificato]**, se ne hai pianificato l’invio) e conferma l’invio.

1. Durante il processo di invio, puoi tracciarne l’avanzamento e visualizzare le statistiche in tempo reale direttamente in questa schermata.

   ![](assets/sending-email.png){zoomable="yes"}

   <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

   Puoi anche accedere a informazioni dettagliate sull’invio facendo clic sul pulsante **[!UICONTROL Registri]**. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

1. Dopo l’invio dell’e-mail, puoi accedere ai rapporti dedicati per ulteriori analisi facendo clic sul pulsante **[!UICONTROL Reporting]**.

![](assets/reports.png){zoomable="yes"}

## Video dimostrativo {#video}

Scopri come creare una consegna e-mail da zero, definire il pubblico, progettare il contenuto, simulare l’anteprima e inviare una bozza.

>[!VIDEO](https://video.tv.adobe.com/v/3425866/?quality=12)
