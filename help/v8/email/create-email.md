---
audience: end-user
title: Crea la tua prima e-mail
description: Documentazione Web di Campaign v8
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# Invia la tua prima e-mail {#first-email}

>[!NOTE]
>
>Questa documentazione è in fase di costruzione e viene aggiornata frequentemente. La versione finale di questo contenuto sarà pronta a gennaio 2023.

Questo caso d’uso illustra come creare la tua prima e-mail

In questo esempio, pianificheremo l’invio di un’e-mail in una data specifica ai clienti fidelizzati in argento e oro. Questo messaggio e-mail verrà progettato utilizzando un modello HTML predefinito da un file ZIP e includerà la personalizzazione utilizzando gli attributi del profilo.

![](assets/delivery-list.png)

## Creare l’e-mail {#create-email}

1. Crea una nuova consegna da **[!UICONTROL Consegne]** menu.
1. Seleziona la **[!UICONTROL E-mail]** canale e modello da utilizzare, quindi fai clic su **[!UICONTROL Crea]**.

   >[!NOTE]
   >
   >informazioni sui modelli. controllare le informazioni in V7 doc

   ![](assets/channel-template.png)

1. Fornisci un’etichetta per la consegna e configura opzioni aggiuntive a seconda delle tue esigenze:

   * Nome interno:
   * Cartella:
   * Codice di consegna:
   * Descrizione:
   * Natura:

   controlla quali impostazioni sono definite nel modello e menzionale (descrizione? cartella?, natura?)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >informazioni sul pulsante delle impostazioni di consegna + collegamento a doc

## Creare il contenuto dell’e-mail {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Crea il tuo primo contenuto e-mail utilizzando E-mail Designer."
>abstract="Creare il primo contenuto e-mail"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creare il contenuto dell’e-mail"
>abstract="TBC"

1. Fai clic sul pulsante **[!UICONTROL Modifica contenuto]** per iniziare a creare il contenuto dell’e-mail.

   Questa schermata ti consente di configurare il contenuto dell’e-mail e progettarlo utilizzando E-mail Designer.

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >Nel modello e-mail selezionato, le informazioni Da e da sono predefinite.
   >
   >Per impostazione predefinita, il tracciamento delle e-mail è abilitato per aperture e clic. Per disattivare queste opzioni, deselezionale dalla sezione Funzioni facoltative .

1. Specifica l’oggetto dell’e-mail utilizzando l’editor espressioni. [Scopri come personalizzare i contenuti](../personalization/personalize.md)

   In questo esempio, vogliamo personalizzare la riga dell’oggetto utilizzando il nome del profilo.

   ![](assets/subject-line.png)

1. Aggiungi un file allegato alla tua e-mail, se necessario. Scopri come modificare il contenuto delle e-mail

1. Fai clic sul pulsante **[!UICONTROL Modifica corpo del messaggio e-mail]** per creare e progettare il contenuto dell’e-mail.

   Scegli il metodo da utilizzare per creare il contenuto delle e-mail. In questo esempio, vogliamo importare un contenuto HTML esistente.

   ![](assets/import-html.png)

1. Seleziona il file HTML o ZIP da importare, quindi fai clic su **[!UICONTROL Successivo]**.

   Se la cartella contiene risorse, scegli l’istanza e la cartella in cui devono essere memorizzate, quindi fai clic su **[!UICONTROL Importa]**. (+ collegamento a documentazione sulle risorse?)

   ![](assets/import-folder.png)

1. Dopo l’importazione, il contenuto viene visualizzato in E-mail Designer, che consente di modificarlo se necessario e di aggiungere personalizzazioni.

   In questo esempio, vogliamo aggiungere la personalizzazione nel titolo dell’e-mail. A questo scopo, seleziona il blocco componente e fai clic su **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/add-perso.png)

1. Quando il contenuto è pronto, salvalo e fai clic sulla freccia per tornare alla schermata di creazione dell’e-mail.

   ![](assets/save-content.png)

## Definire il pubblico {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definire il pubblico"
>abstract="TBC"

1. Fai clic sul pulsante **[!UICONTROL Selezionare il pubblico]** quindi scegli un pubblico esistente o creane uno nuovo.

   In questo esempio, vogliamo utilizzare un pubblico esistente per i clienti appartenenti ai livelli di punti fedeltà argento e oro.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >I tipi di pubblico disponibili nell’elenco provengono dall’istanza Campaign V8 o da Adobe Experience Platform se l’integrazione Destinazione/Origini è stata implementata nell’istanza. Scopri come selezionare il pubblico dell’e-mail

1. Una volta selezionato il pubblico, puoi modificare le regole, se necessario. Puoi anche impostare un gruppo di controllo per analizzare il comportamento dei destinatari delle e-mail rispetto al comportamento dei profili non interessati dal targeting. Scopri come utilizzare i gruppi di controllo

## Pianifica l’invio {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Pianifica l’invio"
>abstract="TBC"

Per pianificare l’invio dell’e-mail, fai clic su Abilita , quindi specifica la data e l’ora desiderate.

= conferma prima dell’opzione di invio : cosa succede alla data pianificata: notifica per confermare l’invio del messaggio?

![](assets/schedule.png)

## Visualizzare l’anteprima e verificare l’e-mail {#preview-test}

Una volta che l’e-mail è pronta, puoi visualizzarla in anteprima e testarla prima di avviarne l’invio.

1. Fai clic su **[!UICONTROL Revisione da inviare]**. Viene visualizzata un’anteprima del messaggio e-mail con tutte le proprietà, il pubblico e la pianificazione configurati. Puoi modificare uno qualsiasi di questi elementi utilizzando il pulsante Modifica.

   ![](assets/review-email.png)

1. Fai clic sul pulsante **[!UICONTROL Simulazione del contenuto]** per visualizzare in anteprima l’e-mail e inviare le bozze.

1. Nell’area a sinistra, seleziona i profili da utilizzare per visualizzare l’anteprima dell’e-mail. Puoi utilizzare profili di destinazione o profili di test dedicati.

1. Un’anteprima del messaggio e-mail viene visualizzata nell’area a destra in base al profilo selezionato. Se hai aggiunto più profili, puoi passare da uno all’altro per visualizzare in anteprima l’e-mail corrispondente.

   ![](assets/preview.png)

   >[!NOTE]
   >
   >Inoltre, la **[!UICONTROL Invia e-mail di rendering]** consente di visualizzare in anteprima l’e-mail utilizzando più dispositivi o provider di posta. Scopri come visualizzare in anteprima il rendering delle e-mail

1. Per inviare le bozze dell’e-mail, fai clic sul pulsante **[!UICONTROL Test]** quindi seleziona i profili che riceveranno la bozza. In questo esempio, desideriamo inviare le bozze a un profilo di test specifico.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >Puoi anche verificare i messaggi impersonando alcuni dei profili target e inviando il messaggio di bozza all’indirizzo e-mail che preferisci. Scopri come utilizzare Sostituisci dalla modalità di destinazione

1. Fai clic su **[!UICONTROL Invia e-mail di test]** quindi conferma l’invio.

   Una volta inviate le bozze, puoi controllarne lo stato facendo clic sul pulsante **[!UICONTROL Visualizza registro e-mail di prova]** pulsante .

## Inviare e monitorare l’e-mail {#prepare-send}

Dopo aver rivisto e verificato l’e-mail, puoi avviarne la preparazione e inviarla.

1. Fai clic su **[!UICONTROL Preparare]** per avviare la preparazione del messaggio.

   Puoi tenere traccia dell’avanzamento della preparazione in tempo reale, insieme alle statistiche. Al termine della preparazione, puoi accedere ai registri dettagliati per ulteriori analisi. Scopri come monitorare le consegne

   ![](assets/preparation.png)

1. Una volta che l’e-mail è pronta per essere inviata, fai clic su **[!UICONTROL Invia]** quindi conferma l’invio.

   Puoi tenere traccia dell’invio in tempo reale, insieme alle statistiche. Inoltre, la **[!UICONTROL Registri]** ti consente di accedere a informazioni dettagliate sull’invio dell’e-mail. Scopri come monitorare le consegne

   ![](assets/logs.png)

1. Dopo l’invio dell’e-mail, puoi accedere ai rapporti dedicati per ulteriori scopi di analisi.

   ![](assets/reports.png)
