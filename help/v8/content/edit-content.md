---
audience: end-user
title: Modificare il contenuto dell’e-mail
description: Scopri come modificare il contenuto delle e-mail nell’interfaccia utente di Campaign Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 100%

---

# Configurare il contenuto dell’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creare il contenuto dell’e-mail"
>abstract="Questa sezione descrive come creare il contenuto dell’e-mail e utilizzare E-mail Designer per conferirgli un aspetto curato."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Parametri e-mail"
>abstract="I valori Nome mittente e Da e-mail sono definiti nel modello e-mail. La riga Oggetto può essere personalizzata utilizzando l’editor di espressioni."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Allegato e-mail"
>abstract="Seleziona uno o più file da inserire nel messaggio."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Opzioni di tracciamento"
>abstract="Per impostazione predefinita, il tracciamento è abilitato per la consegna. Puoi disattivare questa opzione da qui."

La schermata e-mail **[!UICONTROL Modifica contenuto]** consente di:
* Definire gli elementi di base del messaggio, ad esempio l’indirizzo del mittente e la riga dell’oggetto
* Eseguire azioni aggiuntive, ad esempio aggiungere gli allegati o configurare le offerte
* Accedi a [E-mail Designer](get-started-email-designer.md#start-authoring) per iniziare a creare il contenuto corretto dell’e-mail

Per configurare o modificare il contenuto di un’e-mail, segui i passaggi indicati di seguito.

1. Fai clic sul pulsante **[!UICONTROL Modifica contenuto]** dalla schermata della [dashboard di consegna e-mail](../email/create-email.md).

   ![](assets/email-edit-content-button.png)

1. Viene visualizzata la schermata di modifica del contenuto dell’e-mail.

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >Se stai configurando una nuova e-mail, i campi **[!UICONTROL Nome mittente]** e **[!UICONTROL Da e-mail]** sono già popolati.

1. Il **[!UICONTROL Nome mittente]** è definito nel modello e-mail. Se desideri modificarlo, utilizza un nome facilmente identificabile dai destinatari, ad esempio il nome del tuo marchio, per aumentare il tasso di apertura delle consegne.

   >[!NOTE]
   >
   >Per migliorare ulteriormente l’esperienza del destinatario, puoi aggiungere il nome di una persona, ad esempio &quot;Eva da Luma&quot;.

1. Anche il campo dell’indirizzo **[!UICONTROL Da e-mail]** è definito nel modello e-mail. Assicurati che il dominio dell’indirizzo sia lo stesso del sottodominio che hai delegato ad Adobe.

   >[!NOTE]
   >
   >È possibile modificare la parte che precede “@”, ma non l’indirizzo del dominio.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Definisci l’**[!UICONTROL Oggetto]** del messaggio e-mail. Digita l’oggetto direttamente nel campo dedicato oppure apri l’editor espressioni per aggiungere la personalizzazione mediante vari attributi e blocchi di contenuto o offerte. [Scopri come personalizzare il contenuto](../personalization/personalize.md)

1. Se desideri allegare un file all’e-mail, fai clic sul pulsante **[!UICONTROL Aggiungi allegato]** quindi seleziona uno o più file.

   >[!NOTE]
   >
   >    Per evitare problemi di prestazioni, si consiglia di non includere più di un allegato per e-mail.

   <!--limitation on size + number of files?-->

1. Se desideri inviare offerte con il messaggio e-mail, selezionale utilizzando il pulsante **[!UICONTROL Configura offerte]**.

   Puoi quindi inserirle nell’e-mail utilizzando i campi di personalizzazione. [Scopri come inviare offerte](offers.md)

1. Fai clic sul pulsante **[!UICONTROL Modifica corpo e-mail]** per strutturare e progettare il contenuto dell’e-mail utilizzando [E-mail designer](#start-authoring). Per ulteriori informazioni sulla progettazione del contenuto delle e-mail, consulta le seguenti sezioni:

   * [Creare di e-mail da zero](create-email-content.md)
   * [Personalizzare lo stile del contenuto](get-started-email-style.md)

   >[!NOTE]
   >
   >Puoi anche passare il cursore sull’anteprima e-mail e selezionare **[!UICONTROL Apri E-mail designer]**.

1. Per impostazione predefinita, il tracciamento è abilitato per la consegna. Puoi disattivare questa opzione dalla sezione **[!UICONTROL Funzioni facoltative]**. [Scopri come aggiungere collegamenti e gestire il tracciamento](message-tracking.md)

1. Una volta definito il contenuto dell’e-mail, prima di inviarla utilizza il pulsante **[!UICONTROL Simula contenuto]** per controllarne l’aspetto. [Scopri come visualizzare in anteprima e testare il messaggio e-mail](../preview-test/preview-test.md)

