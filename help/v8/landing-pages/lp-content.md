---
title: Definire il contenuto specifico della pagina di destinazione
description: Scopri come progettare contenuti specifici per le pagine di destinazione nel web di Campaign
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: 4dee53676949282b7c0e7664405b7d5a35ef64d2
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 14%

---

# Definire il contenuto specifico della pagina di destinazione {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utilizzare i componenti per contenuti"
>abstract="I componenti per contenuti sono dei segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di una pagina di destinazione. Per definire contenuti specifici che consentano agli utenti di selezionare e inviare le proprie scelte, utilizza il componente modulo."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definire le impostazioni della pagina principale"
>abstract="La pagina principale viene visualizzata immediatamente dagli utenti dopo aver fatto clic sul collegamento alla pagina di destinazione, ad esempio da un’e-mail o da un sito web."

Puoi modificare il contenuto di qualsiasi pagina della pagina di destinazione.

La prima pagina, che viene visualizzata immediatamente dopo aver fatto clic sul collegamento alla pagina di destinazione, è già precompilata con il [componente modulo specifico per la pagina di destinazione](#use-form-component) per il modello selezionato<!-- to enable users to select and submit their choices-->.

Il contenuto della **[!UICONTROL Conferma]**, **[!UICONTROL Errore]** e **[!UICONTROL Scade]** anche le pagine sono precompilate. Modificali in base alle esigenze.

Puoi anche definire [stili per la pagina di destinazione](#lp-form-styles).

Per progettare ulteriormente il contenuto della pagina di destinazione:

* Puoi utilizzare gli stessi componenti utilizzati per progettare un’e-mail. [Ulteriori informazioni](../email/content-components.md#add-content-components)

* Puoi aggiungere contenuto condizionale alle pagine di destinazione, come faresti per un’e-mail. [Ulteriori informazioni](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >Questa funzionalità è a disponibilità limitata (LA). È limitato ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

## Utilizzare il componente modulo {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Impostare i campi del componente modulo"
>abstract="Definisci in che modo i destinatari visualizzeranno e invieranno le loro scelte dalla pagina di destinazione."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Eventi successivi al clic sul pulsante"
>abstract="Definisci gli eventi che si verificheranno dopo l’invio del modulo della pagina di destinazione."

Per definire un contenuto specifico che consenta agli utenti di selezionare e inviare le scelte effettuate dalla pagina di destinazione, modifica il **[!UICONTROL Modulo]** componente. A questo scopo, segui questi passaggi.

1. Le specifiche della pagina di destinazione **[!UICONTROL Modulo]** il componente è già visualizzato nell’area di lavoro del modello selezionato.

   >[!NOTE]
   >
   >Il **[!UICONTROL Modulo]** il componente può essere utilizzato una sola volta sulla stessa pagina.

1. Selezionala. Il **[!UICONTROL Contenuto modulo]** La scheda viene visualizzata nella palette a destra per consentire la modifica dei diversi campi del modulo.

   ![](assets/lp-form-component.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Passa a **[!UICONTROL Stili]** per modificare gli stili del contenuto del componente modulo. [Ulteriori informazioni](#lp-form-styles)

1. Espandere il primo campo di testo, se presente, o aggiungerne uno utilizzando **[!UICONTROL Aggiungi]** pulsante. Dalla sezione **[!UICONTROL Campo testo 1]** , è possibile modificare il tipo di campo, il campo del database da aggiornare, l&#39;etichetta e il testo che verrà visualizzato all&#39;interno del campo prima che gli utenti immettano un valore.

   ![](assets/lp-form-text-field.png){zoomable=&quot;yes&quot;}

1. Controlla la **[!UICONTROL Rendi obbligatorio il campo modulo]** se necessario. In tal caso, la pagina di destinazione può essere inviata solo se l’utente ha compilato questo campo.

   >[!NOTE]
   >
   >Se non viene compilato un campo obbligatorio, quando l’utente invia la pagina viene visualizzato un messaggio di errore.

1. Espandi la casella di controllo, se presente, oppure aggiungine una utilizzando **[!UICONTROL Aggiungi]** pulsante. Seleziona questa opzione se la casella di controllo deve aggiornare un servizio o un campo dal database.

   ![](assets/lp-form-checkbox.png){zoomable=&quot;yes&quot;}

   Se si seleziona **[!UICONTROL Abbonamento e servizi]**, seleziona un [servizio](../audience/manage-services.md) dall’elenco e scegli tra le due opzioni seguenti:

   * **[!UICONTROL Iscriviti se selezionato]**: gli utenti devono selezionare la casella per il consenso (opt-in).
   * **[!UICONTROL Annulla iscrizione se selezionato]**: gli utenti devono selezionare la casella per rimuovere il consenso (rinuncia).

   Se si seleziona **[!UICONTROL Campo]**, selezionare un campo dall&#39;elenco attributi e scegliere tra le due opzioni seguenti:

   * **[!UICONTROL Sì se selezionato]**.<!--TBC-->

   * **[!UICONTROL No se selezionato]**.<!--TBC-->

1. È possibile eliminare e aggiungere tutti i campi, ad esempio campi di testo, pulsanti di scelta, caselle di controllo, elenchi a discesa e così via. secondo necessità.

1. Una volta aggiunti o aggiornati tutti i campi, fai clic su **[!UICONTROL Invito all’azione]** per espandere la sezione corrispondente. Consente di definire il comportamento del pulsante nella **[!UICONTROL Modulo]** componente. [Scopri come](#define-actions-on-form-submission)

   ![](assets/lp-call-to-action.png){zoomable=&quot;yes&quot;}

1. Salva il contenuto per tornare a [proprietà pagina di destinazione](create-lp.md#create-landing-page).

### Definire le azioni per l’invio dei moduli {#define-actions-on-form-submission}

1. Definisci cosa accade quando fai clic sul pulsante:

   * **[!UICONTROL Pagina di conferma]**: per impostazione predefinita, l’utente viene reindirizzato al **[!UICONTROL Conferma]** set di pagine per la pagina di destinazione corrente.

   * **[!UICONTROL URL di reindirizzamento]**: immetti l’URL della pagina a cui verranno reindirizzati gli utenti.

   * **[!UICONTROL Pagina di destinazione]**: puoi selezionare un’altra pagina di destinazione a cui reindirizzare gli utenti. Assicurati di configurare di conseguenza la pagina di destinazione selezionata.

1. Per apportare ulteriori aggiornamenti all&#39;invio del modulo, selezionare **[!UICONTROL Aggiornamenti aggiuntivi]** e selezionare l&#39;elemento che si desidera aggiornare:
   * Un abbonamento [servizio](../audience/manage-services.md) : in tal caso, definisci se desideri dare il consenso o rinunciare agli utenti all’invio del modulo. Durante la progettazione di un’e-mail, se definisci un **[!UICONTROL Pagina di destinazione]**-type a questa pagina di destinazione, il servizio selezionato verrà utilizzato automaticamente. [Ulteriori informazioni sull&#39;inserimento di collegamenti](../email/message-tracking.md)

     >[!NOTE]
     >
     >Se desideri utilizzare diversi servizi con questa pagina di destinazione, utilizza **[!UICONTROL Servizio da URL]** descritto di seguito.

   * Canale: l’e-mail indirizzata utilizzata durante la compilazione del modulo.
   * Tutti i canali: dopo l’invio del modulo, gli utenti saranno inclusi o esclusi (a seconda del modello selezionato) da/per tutte le comunicazioni del tuo marchio su tutti i canali.
   * Campo del database: selezionare un campo dall&#39;elenco degli attributi e definire se deve essere impostato su True o False al momento dell&#39;invio del modulo.

   ![](assets/lp-form-additionnal-updates.png){zoomable=&quot;yes&quot;}

1. Seleziona la **[!UICONTROL Servizio da URL]** per consentire l’utilizzo della pagina di destinazione per diversi servizi, rendendola dinamica. Definisci se desideri dare il consenso o rinunciare agli utenti durante l’invio del modulo.

   >[!AVAILABILITY]
   >
   >Questa funzionalità è a disponibilità limitata (LA). È limitato ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

   ![](assets/lp-form-service-from-url.png){zoomable=&quot;yes&quot;}

   Durante la progettazione di un’e-mail, se definisci un **[!UICONTROL Pagina di destinazione]**-digita il collegamento a questa pagina di destinazione, potrai selezionare qualsiasi servizio dall’elenco. Puoi quindi selezionare altri servizi durante la definizione degli altri collegamenti a questa pagina di destinazione. [Ulteriori informazioni sull&#39;inserimento di collegamenti](../email/message-tracking.md)

   ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

## Definire gli stili del modulo della pagina di destinazione {#lp-form-styles}

1. Per modificare gli stili del contenuto del componente modulo, passa in qualsiasi momento a **[!UICONTROL Stili]** scheda.

1. Il **[!UICONTROL Campo di testo]** viene espansa per impostazione predefinita. Consente di modificare l&#39;aspetto dei campi di testo, ad esempio il carattere dell&#39;etichetta, la posizione dell&#39;etichetta, il colore di sfondo del campo o il bordo del campo.

   ![](assets/lp-text-styles.png){zoomable=&quot;yes&quot;}

1. Espandi **[!UICONTROL Casella di controllo]** per definire l&#39;aspetto delle caselle di controllo e del testo corrispondente. Ad esempio, è possibile regolare la famiglia e la dimensione del carattere o il colore del bordo della casella di controllo.

   ![](assets/lp-checkbox-style.png){zoomable=&quot;yes&quot;}

1. Espandi e modifica qualsiasi altra sezione corrispondente agli altri campi aggiunti (pulsante di opzione, elenco a discesa, data e ora, ecc.) al modulo.

1. Espandi **[!UICONTROL Invito all’azione]** per modificare l&#39;aspetto del pulsante nel modulo del componente. È ad esempio possibile modificare il tipo di carattere, aggiungere un bordo, modificare il colore dell&#39;etichetta al passaggio del mouse o regolare l&#39;allineamento del pulsante.

   ![](assets/lp-call-to-action-style.png){zoomable=&quot;yes&quot;}

   Puoi visualizzare in anteprima alcune impostazioni, ad esempio il colore delle etichette dei pulsanti al passaggio del mouse, utilizzando **[!UICONTROL Simula contenuto]** pulsante. [Ulteriori informazioni](create-lp.md#test-landing-page)

1. Salva le modifiche.
