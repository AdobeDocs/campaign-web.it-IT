---
audience: end-user
title: Testare il rendering delle e-mail
description: Scopri come testare il rendering delle e-mail nell’interfaccia utente di Campaign Web
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Alpha" type="Positive"
source-git-commit: 6bd112c3ceb283435809379403c91ac9c8ed2756
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 9%

---


# Testare il rendering delle e-mail {#email-rendering}

Prima di inviare l’e-mail, assicurati che il messaggio venga visualizzato ai destinatari in modo ottimale su diversi client e dispositivi web.

A questo scopo, puoi sfruttare **Litmus** account in [!DNL Adobe Campaign] per visualizzare all’istante l’anteprima del rendering di e-mail in contesti diversi e verificare la compatibilità nei desktop e nelle applicazioni principali (posta sul web, servizio messaggi, dispositivi mobili, ecc.).

>[!CAUTION]
>
>L’utilizzo del rendering di e-mail in Campaign invia un messaggio e-mail di prova a un sistema di terze parti. Collegando il tuo account Litmus con [!DNL Campaign], riconosci che Adobe non è responsabile per i dati che puoi inviare a tale terza parte. I criteri e-mail di conservazione dei dati Litmus si applicano a queste e-mail, inclusi i dati di personalizzazione che possono essere inclusi in questi messaggi di test. Per accedere o eliminare tali dati, dovrai contattare direttamente Litmus.

Per accedere alle funzionalità di rendering di e-mail, devi:

* Avere un account Litmus
* Selezionare i profili di test: scopri come in [questa sezione](preview-content.md)

Quindi, segui i passaggi indicati di seguito.

1. In [Modifica contenuto](../content/edit-content.md) schermo o nella [E-mail Designer](../content/get-started-email-designer.md), fare clic su **[!UICONTROL Simula contenuto]** pulsante.

1. Seleziona la **[!UICONTROL Rendering e-mail]** pulsante.

   ![](assets/simulate-rendering-button.png)

1. Clic **Connetti il tuo account Litmus** nella sezione superiore destra.

   ![](assets/simulate-rendering-litmus.png)

1. Immetti le credenziali e accedi.

   ![](assets/simulate-rendering-credentials.png)

1. Fai clic su **Esegui test** per generare anteprime e-mail.

1. Controlla i contenuti delle e-mail nei client desktop, mobili e basati su Web più diffusi.

   ![](assets/simulate-rendering-previews.png)

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->