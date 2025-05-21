---
audience: end-user
title: Gestire le risorse con Adobe Experience Manager as a Cloud Service
description: Scopri come gestire i contenuti con Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 4%

---

# Gestisci modelli con [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Introduzione a [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

L’integrazione dell’interfaccia web di Adobe Campaign con Adobe Experience Manager consente di gestire in modo semplificato i contenuti e i moduli per la consegna e-mail direttamente all’interno della piattaforma Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Ulteriori informazioni su Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Crea un modello in [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Passa all&#39;istanza dell&#39;autore [!DNL Adobe Experience Manager] e fai clic su Adobe Experience nell&#39;angolo superiore sinistro della pagina. Scegliere **[!UICONTROL Siti]** dal menu.

1. Accedi a **[!UICONTROL Campagne > Nome del tuo marchio > Area principale > Nome della tua pagina]**.

1. Fai clic su **[!UICONTROL Crea]** e seleziona **[!UICONTROL Pagina]** dal menu a discesa.

   ![Schermata che mostra il pulsante &quot;Crea&quot; e l&#39;opzione &quot;Pagina&quot; nel menu a discesa.](assets/aem_1.png)

1. Seleziona il modello **[!UICONTROL E-mail Adobe Campaign]** e assegna un nome alla newsletter.

   ![[Schermata che mostra la selezione del modello &quot;E-mail Adobe Campaign&quot; e il campo di denominazione.]](assets/aem_2.png)

1. Personalizza il contenuto delle e-mail aggiungendo componenti, ad esempio campi di personalizzazione di Adobe Campaign. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Quando l&#39;e-mail è pronta, passa al menu **[!UICONTROL Informazioni pagina]** e fai clic su **[!UICONTROL Avvia flusso di lavoro]**.

   ![Schermata che mostra il menu &quot;Informazioni pagina&quot; e l&#39;opzione &quot;Avvia flusso di lavoro&quot;.](assets/aem_3.png)

1. Dal primo elenco a discesa, selezionare **[!UICONTROL Approva Adobe Campaign]** come modello di flusso di lavoro e fare clic su **[!UICONTROL Avvia flusso di lavoro]**.

1. Nella parte superiore della pagina verrà visualizzata una dichiarazione di non responsabilità che indica `This page is subject to the workflow Approve for Adobe Campaign`. Fai clic su **[!UICONTROL Completa]** accanto alla liberatoria per confermare la revisione, quindi fai clic su **[!UICONTROL Ok]**.

   ![Schermata che mostra la liberatoria e il pulsante &quot;Completa&quot;.](assets/aem_4.png)

1. Fai di nuovo clic su **[!UICONTROL Completa]** e seleziona **[!UICONTROL Approvazione newsletter]** nel menu a discesa **[!UICONTROL Passaggio successivo]**.

La newsletter è ora pronta e sincronizzata in Adobe Campaign.

## Importare un modello Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Una volta che il modello Experience Manager è disponibile in Adobe Campaign Web come modello di contenuto, puoi identificare e incorporare il contenuto necessario per l’e-mail, inclusa la personalizzazione.

1. In Campaign Web, dal menu **[!UICONTROL Consegne]**, fai clic su **[!UICONTROL Crea consegna]**.

1. Nella finestra del modello e-mail, seleziona il modello predefinito **[!UICONTROL Email delivery with AEM content]**.

   ![Schermata che mostra la selezione del modello &quot;Email delivery with AEM content&quot;.](assets/aem_5.png)

1. Immetti un **[!UICONTROL Etichetta]** per la consegna e configura opzioni aggiuntive in base alle tue esigenze:

   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice consegna]**: utilizza questo campo per organizzare le consegne in base alla tua convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specificare una descrizione per la consegna.
   * **[!UICONTROL Natura]**: specifica la natura dell&#39;e-mail a scopo di classificazione.

1. Definisci un **[!UICONTROL pubblico]** per l&#39;e-mail. [Ulteriori informazioni](../email/create-email.md#define-audience)

1. Fare clic su **[!UICONTROL Modifica contenuto]**.

1. Dal menu **[!UICONTROL Modifica contenuto]**, fare clic su **[!UICONTROL Seleziona contenuto AEM]**.

   ![Schermata che mostra l&#39;opzione &quot;Seleziona contenuto AEM&quot; nel menu &quot;Modifica contenuto&quot;.](assets/aem_6.png)

1. Sfoglia il modello AEM e seleziona quello da importare su Campaign Web.

   ![Schermata che mostra l&#39;interfaccia di selezione del modello di AEM.](assets/aem_8.png)

1. Il contenuto non viene sincronizzato automaticamente. Se vengono apportate modifiche ai modelli direttamente in Adobe Experience Manager, seleziona **[!UICONTROL Aggiorna contenuto AEM]** per aggiornare alla versione più recente del modello.

1. Per rimuovere il collegamento tra Experience Manager e Campaign o per personalizzare ulteriormente il modello Experience Manager nella finestra di progettazione e-mail, fai clic su **[!UICONTROL Scollega contenuto AEM]**.

   ![Schermata che mostra l&#39;opzione &quot;Scollega contenuto AEM&quot;.](assets/aem_9.png)

1. Se hai aggiunto contenuti personalizzati al tuo modello di Experience Manager, fai clic su **[!UICONTROL Simula contenuto]** per visualizzare in anteprima come apparirà nel messaggio utilizzando i profili di test.

[Ulteriori informazioni sull’anteprima e sui profili di test](../preview-test/preview-content.md)

1. Quando visualizzi l’anteprima del messaggio, tutti gli elementi personalizzati vengono automaticamente sostituiti con i dati corrispondenti del profilo di test selezionato.

   Se necessario, aggiungere altri profili di test tramite il pulsante **[!UICONTROL Gestisci profili di test]**.

La consegna è ora pronta per essere inviata.