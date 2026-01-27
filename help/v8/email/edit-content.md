---
audience: end-user
title: Modificare il contenuto dell’e-mail
description: Scopri come modificare il contenuto delle e-mail nell’interfaccia utente web di Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 65%

---

# Configurare il contenuto dell’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definire il contenuto dell’e-mail"
>abstract="La schermata **Modifica contenuto** consente di definire gli elementi di base del messaggio come l’indirizzo del mittente e l’oggetto, eseguire ulteriori azioni come l’aggiunta di allegati o offerte, e accedere a E-mail designer per conferire al messaggio un aspetto professionale."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Impostare le proprietà dell’e-mail"
>abstract="La sezione **Dettagli di base** consente di aggiornare l’indirizzo del mittente e l’indirizzo di risposta e di definire la riga dell’oggetto utilizzando l’editor di espressioni."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Allegare file all’e-mail"
>abstract="Seleziona uno o più file da inserire nel messaggio. Per evitare problemi di prestazioni, si consiglia di non includere più di un allegato per e-mail."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Modificare il tracciamento"
>abstract="Per impostazione predefinita, quando il tracciamento è abilitato per la consegna, vengono tracciati tutti i collegamenti inclusi nel contenuto del messaggio. Puoi disattivare questa opzione da qui."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Aggiungere collegamenti e tenere traccia dei messaggi"

La schermata e-mail **[!UICONTROL Modifica contenuto]** consente di:

* Definire gli elementi di base del messaggio, ad esempio l’indirizzo del mittente e la riga dell’oggetto
* Eseguire azioni aggiuntive, ad esempio aggiungere gli allegati o configurare le offerte
* Accedi a [E-mail Designer](get-started-email-designer.md#start-authoring) per iniziare a creare il contenuto corretto dell’e-mail
* Aggiungi varianti di lingua alle consegne. [Ulteriori informazioni](../msg/multilingual.md)

>[!NOTE]
>
>Tutti i campi di testo modificabili di questa schermata possono essere compilati utilizzando i campi di personalizzazione. [Scopri come personalizzare il contenuto](../personalization/personalize.md)

## Configurare la consegna

Per configurare o modificare il contenuto di un’e-mail, segui i passaggi indicati di seguito.

1. Fai clic sul pulsante **[!UICONTROL Modifica contenuto]** dalla schermata della [dashboard di consegna e-mail](../email/create-email.md).

   ![Schermata che mostra il pulsante Modifica contenuto nel dashboard di consegna e-mail.](assets/email-edit-content-button.png){zoomable="yes"}

1. Viene visualizzata la schermata di modifica del contenuto dell’e-mail.

   ![Schermata che mostra il dashboard dell&#39;edizione del contenuto dell&#39;e-mail.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se stai configurando una nuova e-mail, i campi **[!UICONTROL Da nome]** e **[!UICONTROL Da e-mail]** sono già compilati.

1. Il **[!UICONTROL Nome mittente]** è definito nel modello e-mail. Se desideri modificarlo, utilizza un nome facilmente identificabile dai destinatari, ad esempio il nome del tuo marchio, per aumentare il tasso di apertura delle consegne.

   >[!NOTE]
   >
   >Per migliorare ulteriormente l’esperienza del destinatario, puoi aggiungere il nome di una persona, ad esempio &quot;Eva da Luma&quot;.

1. Anche il campo dell’indirizzo **[!UICONTROL Da e-mail]** è definito nel modello e-mail. Assicurati che il dominio dell’indirizzo corrisponda al sottodominio delegato ad Adobe.

   >[!NOTE]
   >
   >È possibile modificare la parte che precede “@”, ma non l’indirizzo del dominio.

1. Espandi la sezione **[!UICONTROL Campi Rispondi a]**. Il nome e gli indirizzi del mittente vengono utilizzati per le risposte per impostazione predefinita. Tuttavia, Adobe consiglia di utilizzare un indirizzo reale esistente, ad esempio l’assistenza clienti del tuo marchio. In questo caso, se un destinatario invia una risposta, il team di assistenza clienti potrà gestirla.

   ![Schermata che mostra la sezione dei campi di risposta nell&#39;editor dei contenuti e-mail.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Definisci l’**[!UICONTROL Oggetto]** del messaggio e-mail. Digita l&#39;oggetto direttamente nel campo dedicato, oppure apri l&#39;editor espressioni per aggiungere [personalizzazione](../personalization/personalize.md) utilizzando vari attributi, frammenti di espressione o offerte.

1. Per allegare un file all&#39;e-mail, fare clic sul pulsante **[!UICONTROL Aggiungi allegato]**, quindi selezionare uno o più file.

   >[!NOTE]
   >
   >Per evitare problemi di prestazioni, si consiglia di non includere più di un allegato per e-mail.

   <!--limitation on size + number of files?-->

1. Se desideri inviare offerte con il messaggio e-mail, selezionale utilizzando il pulsante **[!UICONTROL Configura offerte]**.

   Puoi quindi inserirli nell’e-mail utilizzando i campi di personalizzazione. [Scopri come inviare offerte](../msg/offers.md)

## Modifica il corpo dell’e-mail

1. Fai clic sul pulsante **[!UICONTROL Modifica corpo e-mail]** per strutturare e progettare il contenuto dell&#39;e-mail utilizzando [E-mail Designer](get-started-email-designer.md#start-authoring).

   >[!NOTE]
   >
   >Puoi anche passare il puntatore sull’anteprima e-mail e selezionare **[!UICONTROL Apri E-mail designer]**.


   Per ulteriori informazioni sulla progettazione del contenuto delle e-mail, consulta le seguenti sezioni:

   * [Creare di e-mail da zero](create-email-content.md)
   * [Personalizzare lo stile del contenuto](get-started-email-style.md)

1. Per impostazione predefinita, il tracciamento è abilitato per la consegna. Puoi disattivare questa opzione dalla sezione **[!UICONTROL Funzioni facoltative]**. [Scopri come aggiungere collegamenti e gestire il tracciamento](message-tracking.md)

1. Una volta definito il contenuto dell’e-mail, prima di inviarla utilizza il pulsante **[!UICONTROL Simula contenuto]** per controllarne l’aspetto. Puoi anche verificare la qualità dei contenuti per valutarne la leggibilità, l’efficacia del CTA e la qualità complessiva. [Ulteriori informazioni sulla convalida della qualità dei contenuti](../content/brands-score.md#validate-quality)

1. [Scopri come visualizzare in anteprima e verificare l&#39;e-mail](../preview-test/preview-test.md).
