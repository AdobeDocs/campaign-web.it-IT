---
audience: end-user
title: Invia la tua prima e-mail
description: Scopri come inviare la tua prima e-mail con l’interfaccia utente web di Campaign
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 871737ba2ab444eaaafde2a3822879629d956e1c
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 0%

---

# Invia la tua prima e-mail {#first-email}

![](../assets/do-not-localize/badge.png)

Scopri come creare la tua prima e-mail con targeting in questo caso d’uso. Pianificheremo l’invio di un’e-mail ai clienti fidelizzati in argento e oro in una data specifica.

Utilizzando un modello di progettazione predefinito, l’e-mail includerà anche contenuti personalizzati in base agli attributi del profilo del cliente.

![](assets/delivery-list.png)

## Creare l’e-mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selezionare un modello e-mail"
>abstract="Un modello è definito nella console Adobe Campaign v8. Si tratta di una configurazione di consegna specifica che contiene parametri predefiniti come regole di tipologia, parametri di personalizzazione o di indirizzamento."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Proprietà e-mail"
>abstract="Le proprietà sono i parametri di consegna comuni che consentono di denominare e classificare la consegna. Se la consegna è basata su uno schema esteso definito nella console Adobe Campaign v8, alcuni **Opzioni personalizzate** i campi sono disponibili."

1. Per creare una nuova consegna, vai alla pagina **[!UICONTROL Consegne]** menu e seleziona **[!UICONTROL E-mail]** come canale.

1. Seleziona il modello da utilizzare e fai clic su **[!UICONTROL Creare una consegna]**.

   >[!NOTE]
   >
   >I modelli sono impostazioni di consegna preconfigurate salvate per un utilizzo futuro. Possono essere create dagli utenti amministratori nella console Adobe Campaign. [Scopri come utilizzare i modelli di consegna](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. Fornisci un’etichetta per l’e-mail e configura opzioni aggiuntive in base alle tue esigenze:

   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna,
   * **[!UICONTROL Cartella]**: memorizzare la consegna in una cartella specifica,
   * **[!UICONTROL Codice di consegna]**: utilizza questo campo per organizzare le consegne in base alla convenzione di denominazione,
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna,
   * **[!UICONTROL Natura]**: specifica la natura dell’e-mail a scopo di classificazione.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Se hai esteso lo schema con campi personalizzati specifici, puoi accedervi nella sezione **[!UICONTROL Opzioni personalizzate]** sezione .

   ![](assets/email-properties.png)

   Inoltre, è possibile accedere alle impostazioni avanzate, come le regole di tipologia e le mappature di destinazione, facendo clic sul pulsante situato accanto al nome della consegna. Queste impostazioni sono preconfigurate nel modello selezionato, ma possono essere modificate in base alle esigenze per questo messaggio e-mail specifico.

## Creare il contenuto dell’e-mail {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Scopri come progettare il contenuto delle e-mail"
>abstract="Scopri come utilizzare E-mail Designer."

In questo caso d’uso, utilizzeremo un modello predefinito per progettare la nostra e-mail.

progetteranno l’e-mail utilizzando un modello predefinito. Istruzioni dettagliate sulla configurazione del contenuto delle e-mail sono disponibili in [questa sezione](../content/edit-content.md).

1. Per iniziare a creare il contenuto dell’e-mail, fai clic sul pulsante **[!UICONTROL Modifica contenuto]** pulsante .

   Verrà visualizzata un’interfaccia dedicata in cui puoi configurare il contenuto dell’e-mail e progettarlo utilizzando E-mail Designer.

   ![](assets/edit-content.png)

1. Digita l’oggetto dell’e-mail e personalizzalo utilizzando l’editor espressioni. [Scopri come personalizzare i contenuti](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Per progettare il corpo dell’e-mail, fai clic sul pulsante **[!UICONTROL Modifica corpo del messaggio e-mail]** pulsante .

   Scegli il metodo da utilizzare per creare il contenuto delle e-mail. In questo esempio, utilizzeremo un modello di progettazione predefinito.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Dopo aver selezionato il modello, questo verrà visualizzato in E-mail Designer, dove potrai apportare le modifiche necessarie e aggiungere la personalizzazione.

   Ad esempio, per aggiungere la personalizzazione al titolo dell’e-mail, seleziona il blocco di componente e fai clic su **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/add-perso.png)

1. Una volta ottenuto il contenuto desiderato, salva e chiudi il progetto. Fai clic su **[!UICONTROL Salva]** per tornare alla schermata di creazione dell’e-mail.

   ![](assets/save-content.png)

## Definire il pubblico {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definire il pubblico"
>abstract="Seleziona il pubblico migliore per il messaggio di marketing. Puoi scegliere un pubblico esistente già definito in un’istanza Campaign v8 o da Adobe Experience Platform oppure puoi scegliere di creare un nuovo pubblico con il generatore di regole."

In questo caso d’uso, invieremo l’e-mail a un pubblico esistente. Sono disponibili ulteriori istruzioni su come lavorare con i tipi di pubblico in [questa sezione](../audience/about-audiences.md).

1. Per selezionare il pubblico per l’e-mail, fai clic sul pulsante **[!UICONTROL Selezionare il pubblico]** e scegli un pubblico esistente dall’elenco.

   In questo esempio, vogliamo utilizzare un pubblico esistente per i clienti appartenenti ai livelli di punti fedeltà argento e oro.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >I tipi di pubblico disponibili nell’elenco provengono dall’istanza Campaign V8 o da Adobe Experience Platform se l’integrazione Destinazione/Origini è stata configurata nell’istanza.
   >
   >L’integrazione Destinazione/Origini ti consente di inviare segmenti di Experience Platform ad Adobe Campaign e di inviare i registri di consegna e tracciamento di Campaign a Adobe Experience Platform. [Scopri come utilizzare Campaign e Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. Una volta selezionato il pubblico, puoi perfezionare ulteriormente il target applicando regole aggiuntive.

   Puoi anche impostare un gruppo di controllo per analizzare il comportamento dei destinatari delle e-mail rispetto a quelli non interessati dal targeting. [Scopri come utilizzare i gruppi di controllo](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Pianifica l’invio {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Pianifica l’invio"
>abstract="Definisci la data e l’ora esatta dell’invio. Scegliendo l’orario più appropriato per il messaggio di marketing, massimizzerai le percentuali di apertura."

Per pianificare l’invio dell’e-mail, fai clic su **[!UICONTROL Abilita]** e imposta la data e l’ora desiderate per l’invio.

Per impostazione predefinita, la **[!UICONTROL Conferma prima dell’invio]** è abilitata e richiede di confermare l’invio prima che l’e-mail venga inviata alla data e all’ora pianificate. Se desideri inviare l’e-mail automaticamente alla data e all’ora pianificate, puoi disattivare questa opzione.

![](assets/schedule.png)

## Visualizzare l’anteprima e verificare l’e-mail {#preview-test}

Prima di inviare l’e-mail, puoi visualizzarla in anteprima e testarla per assicurarti che soddisfi le tue aspettative.

In questo caso d’uso, visualizzeremo l’anteprima dell’e-mail e invieremo versioni di prova a indirizzi e-mail specifici durante la rappresentazione di alcuni dei profili di destinazione.

Sono disponibili ulteriori informazioni su come visualizzare in anteprima e verificare le e-mail in [questa sezione](../preview-test/preview-test.md).

1. Per esaminare e inviare l’e-mail, fai clic su **[!UICONTROL Rivedi e invia]**. Verrà visualizzata un’anteprima del messaggio e-mail, insieme a tutte le proprietà, il pubblico e la pianificazione configurati. Per modificare uno qualsiasi di questi elementi, fai clic sul pulsante Modifica .

1. Per visualizzare in anteprima l’e-mail e inviare le versioni di prova, fai clic sul pulsante **[!UICONTROL Simulazione del contenuto]** pulsante . Viene aperta l’interfaccia di anteprima.

   ![](assets/review-email.png)

1. Sul lato sinistro, seleziona i profili da utilizzare per visualizzare l’anteprima del messaggio e-mail.

   Nel riquadro a destra viene visualizzata un’anteprima dell’e-mail in base al profilo selezionato. Se hai aggiunto più profili, puoi passare da un profilo all’altro per visualizzare in anteprima l’e-mail corrispondente.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Per inviare le versioni di prova dell’e-mail, fai clic sul pulsante **[!UICONTROL Test]** quindi scegliere la modalità da utilizzare.

   In questo esempio, utilizzeremo il **[!UICONTROL Sostituisci dal target principale]** , che invia le versioni di test a indirizzi e-mail specifici durante la rappresentazione di alcuni dei profili target dell’e-mail.

   ![](assets/proof-mode.png)

1. Fai clic su **[!UICONTROL Aggiungi indirizzo]** e specifica gli indirizzi e-mail che riceveranno le versioni di prova.

   Per ogni indirizzo e-mail, seleziona il profilo da rappresentare. Puoi anche consentire ad Adobe Campaign di selezionare un profilo casuale dal target.

   ![](assets/proof-test-profile.png)

1. Fai clic su **[!UICONTROL Invia e-mail di test]** e conferma l’invio.

   Le versioni di prova verranno inviate agli indirizzi e-mail specificati utilizzando il profilo selezionato con **[Prove x]** Prefisso.

   ![](assets/proof-sent.png)

   Puoi controllare lo stato dell’invio e accedere alle e-mail di test inviate in qualsiasi momento facendo clic sul pulsante **[!UICONTROL Visualizza registro e-mail di prova]** nella schermata di simulazione del contenuto.

## Inviare e monitorare l’e-mail {#prepare-send}

Dopo aver esaminato e verificato l’e-mail, puoi avviarne la preparazione e inviarla.

1. Per avviare la preparazione dell’e-mail, fai clic su **[!UICONTROL Preparare]**. [Scopri come preparare un’e-mail](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Quando l’e-mail è pronta per essere inviata, fai clic sul pulsante **[!UICONTROL Invia]** pulsante (o **[!UICONTROL Invia come programmato]** se hai pianificato l’invio) e conferma l’invio.

1. Durante il processo di invio, puoi tracciarne l’avanzamento e visualizzare le statistiche in tempo reale direttamente in questa schermata.

   ![](assets/sent-mail.png)

   Puoi anche accedere a informazioni dettagliate sull’invio facendo clic sul pulsante **[!UICONTROL Registri]** pulsante . [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)

1. Dopo l’invio dell’e-mail, puoi accedere ai rapporti dedicati per ulteriori analisi facendo clic sul pulsante **[!UICONTROL Reporting]** pulsante .

![](assets/reports.png)
