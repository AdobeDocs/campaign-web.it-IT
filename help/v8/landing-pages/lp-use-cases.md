---
solution: Campaign, Campaign v8 Web User Interface
title: Casi di utilizzo della pagina di destinazione
description: Scopri i casi d’uso più comuni con le pagine di destinazione nell’interfaccia utente di Campaign Web
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: destinazione, pagina di destinazione, caso d’uso
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 9%

---

# Come utilizzare una pagina di destinazione {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copiare l’URL con attenzione"
>abstract="Per testare o sfruttare appieno la pagina di destinazione, non puoi copiare e incollare questo collegamento direttamente in un browser web o nelle consegne. Piuttosto, utilizza la funzione **Simula contenuto** per testarla e segui i passaggi descritti nella documentazione per utilizzare correttamente la pagina di destinazione."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="Copiare l’URL con attenzione"
>abstract="Durante la creazione di una pagina di destinazione, quattro modelli predefiniti consentono di implementare diversi casi d’uso: aggiungere o aggiornare un profilo al database di Campaign, iscrivere i clienti a un servizio, annullare l’iscrizione a un servizio o negare il consenso agli utenti."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=it#create-landing-page" text="Creare una pagina di destinazione"

Per utilizzare correttamente la pagina di destinazione, fai riferimento a essa come collegamento in un messaggio utilizzando l’opzione dedicata. Non puoi copiare e incollare il collegamento visualizzato nel dashboard di consegna pubblicato direttamente nelle consegne o in una pagina web. Utilizza invece la funzionalità **Simula contenuto** per verificarlo.

Nell&#39;interfaccia [!DNL Adobe Campaign Web], quattro modelli predefiniti consentono di implementare diversi casi d&#39;uso. Tuttavia, le fasi principali rimangono le stesse e sono descritte di seguito.

1. [Crea una pagina di destinazione](create-lp.md#create-landing-page) e seleziona il modello desiderato, in base al caso d&#39;uso.

1. Definisci le proprietà e le impostazioni della pagina di destinazione.

   ![Schermata che mostra l&#39;interfaccia delle proprietà e delle impostazioni della pagina di destinazione.](assets/lp-uc-properties.png){zoomable="yes"}

1. In base al tuo caso, seleziona la pagina **[!UICONTROL Acquisizione]**, **[!UICONTROL Abbonamento]**, **[!UICONTROL Annullamento dell&#39;abbonamento]** o **[!UICONTROL Inserisco nell&#39;elenco Bloccati di]**.

1. Viene visualizzato il contenuto della pagina. Seleziona la parte corrispondente al modulo della pagina di destinazione.

   ![Schermata che mostra l&#39;interfaccia del modulo della pagina di destinazione.](assets/lp-uc-form.png){zoomable="yes"}

1. Modifica il contenuto in base al modello selezionato:

   * [Acquisizione](#lp-acquisition)
   * [Iscrizione](#lp-subscription)
   * [Annullamento iscrizione](#lp-unsubscription)
   * [Elenco Bloccati](#lp-denylist)

1. Modifica il resto del contenuto in base alle esigenze, salva le modifiche e chiudi.

1. Modifica la pagina **[!UICONTROL Conferma]** in base alle esigenze, nonché le pagine **[!UICONTROL Errore]** e **[!UICONTROL Scadenza]**. La pagina **[!UICONTROL Conferma]** verrà visualizzata ai destinatari dopo l&#39;invio del modulo.

   ![Schermata che mostra l&#39;interfaccia della pagina di conferma.](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [Verifica](create-lp.md#test-landing-page) e [pubblica](create-lp.md#publish-landing-page) la tua pagina di destinazione.

1. Crea una consegna [e-mail](../email/create-email.md) per indirizzare il traffico alla pagina di destinazione.

1. [Inserisci un collegamento](../email/message-tracking.md#insert-links) nel contenuto del messaggio. Seleziona **[!UICONTROL Pagina di destinazione]** come **[!UICONTROL Tipo di collegamento]** e scegli la pagina di destinazione creata.

   ![Schermata che mostra l&#39;interfaccia di inserimento del collegamento e-mail.](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Per poter inviare il messaggio, assicurati che la pagina di destinazione selezionata non sia ancora scaduta. [Ulteriori informazioni](create-lp.md#create-landing-page)

Una volta ricevuta l’e-mail, se i destinatari fanno clic sul collegamento alla pagina di destinazione e inviano il modulo:

* Verranno indirizzati alla pagina di conferma.
* Verrà applicata qualsiasi altra azione definita nella pagina di destinazione. Ad esempio, gli utenti verranno abbonati al servizio o non riceveranno più comunicazioni da te.

Di seguito sono riportati alcuni esempi di come utilizzare le pagine di destinazione [!DNL Adobe Campaign] nei diversi casi d&#39;uso possibili.

## Acquisizione profilo {#lp-acquisition}

Il primo modello consente di aggiungere o aggiornare un profilo al database di Campaign.

1. Quando [crei la pagina di destinazione](create-lp.md#create-landing-page), seleziona il modello **[!UICONTROL Acquisizione]**.

1. Nelle proprietà della pagina di destinazione, seleziona l&#39;opzione **[!UICONTROL Precompila con i dati a cui si fa riferimento nel modulo]** per precaricare eventuali informazioni esistenti dal profilo ed evitare di creare duplicati.

1. Seleziona la pagina **[!UICONTROL Acquisizione]** per modificarne il contenuto.

1. Modifica i campi di testo in base alle esigenze, in base alle informazioni che desideri raccogliere sui profili.

1. Aggiungi una casella di controllo che invita i clienti ad abbonarsi al servizio newsletter. [Scopri come creare un servizio](../audience/manage-services.md)

   ![Schermata che mostra l&#39;interfaccia della pagina di acquisizione con una casella di controllo per l&#39;abbonamento a una newsletter.](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Modifica il contenuto in base alle esigenze e salva le modifiche.

1. Rivedi e [pubblica](create-lp.md#publish-landing-page) la tua pagina di destinazione.

1. Crea un [messaggio e-mail](../email/create-email.md) e [aggiungi un collegamento](../email/message-tracking.md#insert-links) alla pagina di destinazione.

Una volta ricevuta l’e-mail, se i destinatari fanno clic sul collegamento alla pagina di destinazione e inviano il modulo, il loro profilo verrà aggiunto al database di Campaign o aggiornato in base alle informazioni fornite.

![Schermata che mostra un profilo aggiornato nel database di Campaign.](assets/lp-uc-profile-updated.png){zoomable="yes"}

Se hanno acconsentito alla ricezione della newsletter, saranno abbonati al servizio corrispondente.

![Schermata che mostra la conferma dell&#39;abbonamento a una newsletter.](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Abbonamento a un servizio {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Impostare la pagina di destinazione dell&#39;iscrizione"
>abstract="Una pagina di iscrizione consente ai clienti di iscriversi a un servizio."

Uno dei casi d&#39;uso più comuni consiste nell&#39;invitare i clienti a [abbonarsi a un servizio](../audience/manage-services.md) (ad esempio una newsletter o un evento) tramite una pagina di destinazione. Segui i passaggi seguenti.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Crea un modello di conferma per gli utenti che si abbonano all’evento, in modo da poterlo selezionare facilmente durante la creazione del servizio. [Ulteriori informazioni](../audience/manage-services.md#create-confirmation-message)

   ![Schermata che mostra l&#39;interfaccia del modello e-mail di conferma.](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Crea un servizio di abbonamento, che memorizzerà gli utenti registrati per il tuo evento. [Scopri come creare un servizio](../audience/manage-services.md)

1. Seleziona il modello creato come e-mail di conferma che gli utenti riceveranno al momento dell’abbonamento.

   ![Schermata che mostra l&#39;interfaccia del servizio di sottoscrizione.](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [Crea una pagina di destinazione](create-lp.md#create-landing-page) per consentire ai destinatari di registrarsi all&#39;evento. Selezionare il modello **[!UICONTROL Sottoscrizione]**.

1. Selezionare la pagina **[!UICONTROL Sottoscrizione]** per modificarne il contenuto.

1. Viene visualizzato il contenuto della pagina. Selezionare la parte corrispondente al modulo della pagina di destinazione ed espandere la sezione **[!UICONTROL Casella di controllo 1]**.

1. Nel campo **[!UICONTROL Abbonamenti e servizi]**, seleziona il servizio creato per l&#39;evento. Lascia abilitata l&#39;opzione **[!UICONTROL Sottoscrivi se selezionata]**.

   ![Schermata che mostra l&#39;interfaccia della casella di controllo della sottoscrizione.](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Modifica il contenuto in base alle esigenze e salva le modifiche.

1. Rivedi e [pubblica](create-lp.md#publish-landing-page) la tua pagina di destinazione.

1. Crea un [messaggio e-mail](../email/create-email.md) e [aggiungi un collegamento](../email/message-tracking.md#insert-links) per indirizzare il traffico alla pagina di destinazione della registrazione.

1. Progetta l’e-mail per annunciare che la registrazione è ora aperta per il tuo evento.

Una volta ricevuta l’e-mail, se i destinatari fanno clic sul collegamento alla pagina di destinazione e inviano il modulo, verranno indirizzati alla pagina di conferma e aggiunti all’elenco degli abbonamenti.

## Annullamento iscrizione {#lp-unsubscription}

Puoi consentire ai clienti di annullare l’abbonamento a un servizio utilizzando una pagina di destinazione.

1. Crea un modello di conferma per gli utenti che annullano l’abbonamento al servizio, in modo da poterlo selezionare facilmente durante la creazione del servizio. [Ulteriori informazioni](../audience/manage-services.md#create-confirmation-message)

1. Nel [servizio di abbonamento](../audience/manage-services.md), seleziona il modello creato come e-mail di conferma che gli utenti riceveranno al momento dell&#39;annullamento dell&#39;abbonamento.

1. [Crea una pagina di destinazione](create-lp.md#create-landing-page). Selezionare il modello **[!UICONTROL Annulla sottoscrizione]**.

1. Selezionare la pagina **[!UICONTROL Annulla sottoscrizione]** per modificarne il contenuto.

1. Viene visualizzato il contenuto della pagina. Seleziona la parte corrispondente al modulo della pagina di destinazione.

1. Aggiungi una sezione **[!UICONTROL Checkbox]**, seleziona il servizio e, se selezionata, seleziona l&#39;opzione **[!UICONTROL Annulla iscrizione]**.

   ![Schermata che mostra l&#39;interfaccia della casella di controllo per l&#39;annullamento dell&#39;abbonamento.](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. Espandi la sezione **[!UICONTROL Invito all&#39;azione]** e seleziona l&#39;opzione **[!UICONTROL Aggiornamenti aggiuntivi]**. Seleziona il servizio e seleziona l&#39;opzione **[!UICONTROL Rinuncia]**.

   ![Schermata che mostra l&#39;interfaccia di call-to-action per l&#39;annullamento dell&#39;abbonamento.](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Modifica il contenuto in base alle esigenze e salva le modifiche.

1. Rivedi e [pubblica](create-lp.md#publish-landing-page) la tua pagina di destinazione.

1. Crea un [messaggio e-mail](../email/create-email.md) e [aggiungi un collegamento](../email/message-tracking.md#insert-links) alla pagina di destinazione.

Una volta ricevuta l’e-mail, se i destinatari fanno clic sul collegamento alla pagina di destinazione e inviano il modulo, verranno indirizzati alla pagina di conferma dell’annullamento dell’abbonamento e rimossi dal servizio di abbonamento corrispondente.

## Elenco Bloccati {#lp-denylist}

Come requisito legale, è necessario dare ai destinatari la possibilità di annullare l’abbonamento alla ricezione di comunicazioni da un marchio. Pertanto, devi sempre includere un **collegamento per annullare l&#39;iscrizione** in ogni e-mail inviata ai destinatari. Facendo clic su questo collegamento, i destinatari verranno indirizzati a una pagina di destinazione contenente un pulsante per confermare la rinuncia.

Inserire nell&#39;elenco Bloccati Puoi impostare una pagina di destinazione di **[!UICONTROL 1} che consentirà agli utenti di rinunciare a tutte le consegne.]**

1. Inserire nell&#39;elenco Bloccati Quando [crei la pagina di destinazione](create-lp.md#create-landing-page), seleziona il modello ****.

1. Selezionare la pagina **[!UICONTROL Inserisce nell&#39;elenco Bloccati]** per modificarne il contenuto.

1. Espandi la sezione **[!UICONTROL Invito all&#39;azione]** e seleziona l&#39;opzione **[!UICONTROL Aggiornamenti aggiuntivi]**.

1. Dall&#39;elenco a discesa corrispondente, seleziona **[!UICONTROL Canale (e-mail)]** per consentire ai destinatari di rinunciare solo alle comunicazioni e-mail. Puoi anche selezionare **[!UICONTROL Per tutti i canali]** per escluderli da tutte le comunicazioni su tutti i canali.

   ![Schermata che mostra l&#39;interfaccia call-to-action di di inserire nell&#39;elenco Bloccati.](assets/lp-uc-denylist.png){zoomable="yes"}

1. Modifica il contenuto in base alle esigenze e salva le modifiche.

1. Rivedi e [pubblica](create-lp.md#publish-landing-page) la tua pagina di destinazione.

1. Crea un [messaggio e-mail](../email/create-email.md) e [aggiungi un collegamento](../email/message-tracking.md#insert-links) alla pagina di destinazione per consentire agli utenti di rinunciare alla ricezione di comunicazioni.

Una volta ricevuta l’e-mail, se i destinatari fanno clic sul collegamento alla pagina di destinazione e inviano il modulo, verranno indirizzati alla pagina di conferma del inserisco nell&#39;elenco Bloccati di e il loro profilo verrà aggiornato con le informazioni fornite.

Per verificare che la scelta del profilo corrispondente sia stata aggiornata, passare al menu **[!UICONTROL Profili]** e selezionare tale profilo.

Ad esempio, se hai scelto di aggiornare l&#39;opzione **[!UICONTROL Canale (e-mail)]** nella pagina di destinazione, verrà selezionata l&#39;opzione **[!UICONTROL Non contattare più tramite e-mail]**.

![Schermata che mostra un profilo aggiornato con le preferenze di inserisce nell&#39;elenco Bloccati di.](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Questo profilo non riceverà comunicazioni e-mail dal tuo marchio, a meno che non si sia nuovamente iscritti.