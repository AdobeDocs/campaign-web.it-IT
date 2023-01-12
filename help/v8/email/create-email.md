---
audience: end-user
title: Crea la tua prima e-mail
description: Documentazione Web di Campaign v8
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 2%

---

# Invia la tua prima e-mail {#first-email}

![](../assets/do-not-localize/badge.png)

Questo caso d’uso illustra come creare la tua prima e-mail. Pianificheremo l&#39;invio di un&#39;e-mail in una data specifica ai clienti fidelizzati in argento e oro. Questo messaggio e-mail verrà progettato utilizzando un modello predefinito e includerà la personalizzazione utilizzando gli attributi del profilo.

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

1. Crea una nuova consegna da **[!UICONTROL Consegne]** menu.

1. Seleziona la **[!UICONTROL E-mail]** canale e modello da utilizzare, quindi fai clic su **[!UICONTROL Crea]**.

   >[!NOTE]
   >
   >Un modello è una configurazione di consegna specifica salvata come modello per essere riutilizzata. I modelli di consegna sono configurati dagli utenti amministratori nella console Adobe Campaign. [Scopri come utilizzare i modelli di consegna](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-delivery-templates/about-templates.html?lang=it){target="_blank"}

   ![](assets/channel-template.png)

1. Fornisci un’etichetta per l’e-mail e configura opzioni aggiuntive in base alle tue esigenze:

   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna,
   * **[!UICONTROL Cartella]**: memorizzare la consegna in una cartella specifica,
   * **[!UICONTROL Codice di consegna]**: utilizza questo campo per organizzare le consegne in base alla convenzione di denominazione,
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna,
   * **[!UICONTROL Natura]**: specifica la natura dell’e-mail a scopo di classificazione.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Se hai esteso lo schema con campi personalizzati specifici, puoi accedervi dalla **[!UICONTROL Opzioni personalizzate]** sezione .

   ![](assets/email-properties.png)

   Inoltre, impostazioni avanzate (regola di tipologia, mappature di destinazione, ecc.) sono disponibili dal pulsante situato accanto al nome della consegna. Sono predefiniti nel modello selezionato al momento della creazione dell’e-mail. Se necessario, puoi modificarli.

## Creare il contenuto dell’e-mail {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Scopri come progettare il contenuto delle e-mail utilizzando E-mail Designer."
>abstract="Scopri come progettare il contenuto"

In questo caso d’uso, progetteremo l’e-mail utilizzando un modello predefinito. Informazioni dettagliate su come configurare il contenuto delle e-mail sono disponibili in [questa sezione](../content/edit-content.md).

1. Fai clic sul pulsante **[!UICONTROL Modifica contenuto]** per iniziare a creare il contenuto dell’e-mail.

   Questa schermata ti consente di configurare il contenuto dell’e-mail e progettarlo utilizzando E-mail Designer.

   ![](assets/edit-content.png)

1. Specifica l’oggetto dell’e-mail e personalizzalo utilizzando l’editor espressioni. [Scopri come personalizzare i contenuti](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Fai clic sul pulsante **[!UICONTROL Modifica corpo del messaggio e-mail]** per creare e progettare il contenuto dell’e-mail.

   Scegli il metodo da utilizzare per creare il contenuto delle e-mail. In questo esempio, vogliamo utilizzare un modello di progettazione esistente.

   ![](assets/import-html.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Dopo aver selezionato il modello, questo viene visualizzato in E-mail Designer, che consente di modificarlo se necessario e di aggiungere personalizzazioni.

   In questo esempio, vogliamo aggiungere la personalizzazione nel titolo dell’e-mail. A questo scopo, seleziona il blocco componente e fai clic su **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/add-perso.png)

1. Quando il contenuto è pronto, salvalo e fai clic sulla freccia per tornare alla schermata di creazione dell’e-mail.

   ![](assets/save-content.png)

## Definire il pubblico {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definire il pubblico"
>abstract="Seleziona il pubblico migliore per il messaggio di marketing. Puoi scegliere un pubblico esistente già definito in un’istanza Campaign v8 o da Adobe Experience Platform oppure puoi scegliere di creare un nuovo pubblico con il generatore di regole."

In questo caso d’uso, invieremo l’e-mail a un pubblico esistente. Sono disponibili ulteriori informazioni su come lavorare con i tipi di pubblico in [questa sezione](../audience/about-audiences.md).

1. Fai clic sul pulsante **[!UICONTROL Selezionare il pubblico]** quindi scegli un pubblico esistente di cui eseguire il targeting.

   In questo esempio, vogliamo utilizzare un pubblico esistente per i clienti appartenenti ai livelli di punti fedeltà argento e oro.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >I tipi di pubblico disponibili nell’elenco provengono dall’istanza Campaign V8 o da Adobe Experience Platform se l’integrazione Destinazione/Origini è stata configurata nell’istanza.
   >
   >L’integrazione Destinazione/Origini ti consente di inviare segmenti di Experience Platform ad Adobe Campaign e di inviare i registri di consegna e tracciamento di Campaign a Adobe Experience Platform. [Scopri come utilizzare Campaign e Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html)

1. Una volta selezionato il pubblico, puoi perfezionarlo utilizzando regole aggiuntive.

   Puoi anche impostare un gruppo di controllo per analizzare il comportamento dei destinatari delle e-mail rispetto al comportamento dei profili non interessati dal targeting. [Scopri come utilizzare i gruppi di controllo](../audience/control-group.md)

## Pianifica l’invio {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Pianifica l’invio"
>abstract="Definisci la data e l’ora esatta dell’invio. Scegliendo l’orario più appropriato per il messaggio di marketing, massimizzerai le percentuali di apertura."

Per pianificare l’invio dell’e-mail, fai clic su **[!UICONTROL Abilita]** quindi specifica la data e l’ora desiderate per l’invio.

Per impostazione predefinita, la **[!UICONTROL Conferma prima dell’invio]** è abilitata, il che significa che dovrai confermare l’invio per consentire l’invio dell’e-mail alla data e all’ora specificate. Disattiva questa opzione per consentire l’invio dell’e-mail alla data e all’ora pianificate senza alcuna conferma necessaria.

![](assets/schedule.png)

## Visualizzare l’anteprima e verificare l’e-mail {#preview-test}

Una volta che l’e-mail è pronta, puoi visualizzarla in anteprima e testarla prima di avviarne l’invio.

In questo caso d’uso, visualizzeremo l’anteprima dell’e-mail e invieremo una bozza utilizzando i profili esistenti.

Sono disponibili ulteriori informazioni su come visualizzare in anteprima e verificare le e-mail in [questa sezione](../preview-test/preview-test.md).

1. Fai clic su **[!UICONTROL Revisione da inviare]**. Viene visualizzata un’anteprima del messaggio e-mail con tutte le proprietà, il pubblico e la pianificazione configurati. Puoi modificare uno qualsiasi di questi elementi utilizzando il pulsante Modifica.

1. Fai clic sul pulsante **[!UICONTROL Simulazione del contenuto]** per visualizzare in anteprima l’e-mail e inviare le bozze.

   ![](assets/review-email.png)

1. Nell’area a sinistra, seleziona i profili da utilizzare per visualizzare l’anteprima del messaggio e-mail.

1. Nel riquadro a destra viene visualizzata un’anteprima del messaggio e-mail in base al profilo selezionato. Se hai aggiunto più profili, puoi passare da uno all’altro per visualizzare in anteprima l’e-mail corrispondente.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Per inviare le bozze dell’e-mail, fai clic sul pulsante **[!UICONTROL Test]** quindi seleziona i profili che riceveranno la bozza.

   <!--TO REPLACE WITH SUBSTITUTION PROFILE-->In this example, we want to send the proofs to a specific test profile, which is a seed address that is not part of the target. [Learn how to work with seed addresses](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/about-seed-addresses.html){target="_blank"}

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >Puoi anche verificare i messaggi impersonando alcuni dei profili target e inviando il messaggio di bozza all’indirizzo e-mail che preferisci. [Scopri come inviare bozze](../preview-test/preview-test.md)

1. Fai clic su **[!UICONTROL Invia e-mail di test]** quindi conferma l’invio.

   Una volta inviate le bozze, puoi controllarne lo stato facendo clic sul pulsante **[!UICONTROL Visualizza registro e-mail di prova]** pulsante .

## Inviare e monitorare l’e-mail {#prepare-send}

Dopo aver rivisto e verificato l’e-mail, puoi avviarne la preparazione e inviarla.

1. Fai clic su **[!UICONTROL Preparare]** per avviare la preparazione del messaggio. [Scopri come preparare un’e-mail](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Una volta che l’e-mail è pronta per essere inviata, fai clic su **[!UICONTROL Invia]** quindi conferma l’invio.

   Puoi tenere traccia dell’invio in tempo reale, insieme alle statistiche. Inoltre, la **[!UICONTROL Registri]** ti consente di accedere a informazioni dettagliate sull’invio dell’e-mail. [Scopri come monitorare i registri di consegna](../monitor/delivery-logs.md)
   ![](assets/logs.png)

1. Dopo l’invio dell’e-mail, puoi accedere a [rapporti](../reporting/reports.md) per ulteriori analisi.

   ![](assets/reports.png)
