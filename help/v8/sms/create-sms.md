---
audience: end-user
title: Creare una consegna SMS
description: Scopri come creare e inviare SMS con Adobe Campaign Web
badge: label="Beta"
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 4ea25f0877fd3f0ab02f3023f041bd040e0530a3
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 100%

---

# Creare una consegna SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Proprietà di consegna SMS"
>abstract="Le proprietà includono i parametri di consegna comuni che consentono di denominare e classificare la consegna. Se la consegna è basata su uno schema esteso, sono disponibili campi specifici di opzioni personalizzate."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definisci il pubblico dell’SMS"
>abstract="Puoi creare un nuovo pubblico o selezionarne uno esistente facendo clic sul pulsante **Seleziona pubblico**. Se necessario, aggiungi un gruppo di controllo per misurare l’impatto della consegna."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=it" text="Impostare un gruppo di controllo"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selezione modello SMS"
>abstract="Seleziona un modello predefinito per avviare la consegna SMS. I modelli di consegna ti consentono di riutilizzare facilmente contenuti e impostazioni personalizzati in tutte le campagne e le consegne."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=it" text="Utilizzare i modelli di consegna"


Puoi creare una consegna SMS autonoma o un SMS nel contesto di un flusso di lavoro della campagna. I passaggi seguenti descrivono la procedura per una consegna SMS autonoma (singola). Se stai utilizzando il contesto del flusso di lavoro di una campagna, i passaggi di creazione sono descritti in [questa sezione](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Per creare una consegna SMS autonoma, segui i seguenti passaggi:

1. Passa al menu **[!UICONTROL Consegne]** nella barra di navigazione a sinistra, quindi fai clic sul pulsante **[!UICONTROL Crea consegna]**.

1. Nella sezione **[!UICONTROL Canale]**, scegli SMS come canale e seleziona un modello. [Ulteriori informazioni sui modelli](../msg/delivery-template.md)

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.

   ![](assets/sms_create_1.png)

1. Immetti un’**[!UICONTROL etichetta]** per la consegna e accedi al menu a discesa **[!UICONTROL Opzioni aggiuntive]**. Se la consegna è basata su uno schema esteso, sono disponibili campi specifici di **Opzioni personalizzate**.

   +++Configura le seguenti impostazioni in base alle tue esigenze.
   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: organizza le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura dell’e-mail a scopo di classificazione.
+++

1. Fai clic sul pulsante **[!UICONTROL Seleziona pubblico]** per eseguire il targeting di un pubblico esistente o crearne uno tuo. [Ulteriori informazioni sui tipi di pubblico](../audience/about-recipients.md)

   ![](assets/sms_create_2.png)

   Scopri come selezionare un pubblico esistente in [questa pagina](../audience/add-audience.md)

   Per scoprire come creare un nuovo pubblico, consulta [questa pagina](../audience/one-time-audience.md)

1. Attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]** per impostare un gruppo di controllo per misurare l’impatto della consegna. I messaggi non vengono inviati a tale gruppo di controllo, in modo da poter confrontare il comportamento di chi ha ricevuto il messaggio con quello dei contatti che non lo hanno ricevuto. [Ulteriori informazioni](../audience/control-group.md)

1. Fai clic su **[!UICONTROL Modifica contenuto]** per iniziare a progettare il contenuto del messaggio SMS. [Ulteriori informazioni](content-sms.md)

   ![](assets/sms_create_4.png)

   Da questa schermata, è possibile anche [simulare i contenuti](../preview-test/preview-test.md) e [configurare le offerte](../content/offers.md).

1. Per pianificare la consegna a una data e un’ora specifiche, attiva l’opzione **[!UICONTROL Abilita pianificazione]**. Dopo aver avviato la consegna, il messaggio viene inviato automaticamente nella data e nell’ora esatte definite per il destinatario. Per ulteriori informazioni sulla pianificazione della consegna, consulta [questa sezione](../msg/gs-messages.md#gs-schedule).

1. Fai clic su **[!UICONTROL Configura le impostazioni di consegna]** per accedere alle opzioni avanzate relative al modello di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
