---
audience: end-user
title: Modificare il contenuto dell’e-mail
description: Scopri come modificare il contenuto delle e-mail nell’interfaccia utente di Campaign Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: 46f2f42f724232b15f826f01c5957c0295c61f26
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configurare il contenuto dell’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creare il contenuto dell’e-mail"
>abstract="Questa sezione descrive come creare il contenuto dell’e-mail e utilizzare E-mail Designer per conferirgli un aspetto curato."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Parametri e-mail"
>abstract="I valori Da nome e Da e-mail sono definiti nel modello e-mail. La riga Oggetto può essere personalizzata utilizzando l’editor espressioni."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Allegato e-mail"
>abstract="Seleziona uno o più file da inserire nel messaggio."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Opzioni di tracciamento"
>abstract="Per impostazione predefinita, il tracciamento è abilitato per la consegna. Puoi disattivare questa opzione da qui."

Per iniziare a creare il contenuto di un’e-mail, fai clic su **[!UICONTROL Modifica contenuto]** dal pulsante [dashboard di consegna e-mail](../email/create-email.md) schermo.

![](assets/email-edit-content.png)

La schermata visualizzata consente di definire i dettagli di base, eseguire alcune azioni aggiuntive, ad esempio aggiungere allegati o impostare le offerte, e accedere al [E-mail Designer](#start-authoring) per creare i contenuti.

![](assets/email-edit-content-dashboard.png)

Per modificare il contenuto dell’e-mail, segui questi passaggi:

1. In **[!UICONTROL Nome mittente]** utilizza un nome facilmente identificabile dai destinatari, ad esempio il nome del tuo marchio, per aumentare il tasso di apertura delle consegne.

   Per migliorare ulteriormente l’esperienza del destinatario, puoi aggiungere il nome di una persona, ad esempio &quot;Emma from Megastore&quot;.

1. In **[!UICONTROL Da e-mail]** indirizzo, assicurati che il dominio dell’indirizzo sia lo stesso del sottodominio che hai delegato ad Adobe.

   >[!NOTE]
   >
   >    È possibile modificare la parte che precede &#39;@&#39;, ma non l&#39;indirizzo di dominio.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Definisci l’**[!UICONTROL Oggetto]** del messaggio e-mail. Inserisci l’oggetto direttamente nel campo dedicato, oppure apri l’editor espressioni per aggiungere personalizzazioni utilizzando vari attributi e blocchi di contenuto o offerte. [Scopri come personalizzare il contenuto](../personalization/personalize.md)

1. Se desideri allegare un file all’e-mail, fai clic sul pulsante **[!UICONTROL Aggiungi allegato]** quindi seleziona uno o più file.

   >[!NOTE]
   >
   >    Per evitare problemi di prestazioni, si consiglia di non includere più di un allegato per e-mail.

   <!--limitation on size + number of files?-->

1. Se desideri inviare offerte con il messaggio e-mail, selezionale utilizzando il pulsante **[!UICONTROL Configura offerte]**.

   Puoi quindi inserirle nell’e-mail utilizzando i campi di personalizzazione. [Scopri come inviare offerte](offers.md)

1. Fai clic su **[!UICONTROL Modifica corpo dell’e-mail]** per strutturare e progettare il contenuto dell’e-mail utilizzando [E-mail Designer](#start-authoring). Per ulteriori informazioni sulla progettazione del contenuto delle e-mail, consulta le seguenti sezioni:

   * [Scopri come progettare le e-mail](create-email-content.md)
   * [Personalizzare lo stile del contenuto](get-started-email-style.md)

1. Per impostazione predefinita, il tracciamento è abilitato per la consegna. Puoi disattivare questa opzione dalla sezione **[!UICONTROL Funzioni facoltative]**. [Scopri come aggiungere collegamenti e gestire il tracciamento](message-tracking.md)

1. Una volta definito il contenuto dell’e-mail, prima di inviarla utilizza il pulsante **[!UICONTROL Simula contenuto]** per controllarne l’aspetto. [Scopri come visualizzare in anteprima e testare il messaggio e-mail](../preview-test/preview-test.md)

