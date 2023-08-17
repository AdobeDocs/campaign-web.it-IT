---
audience: end-user
title: Creare una consegna SMS
description: Scopri come creare e inviare SMS con Adobe Campaign Web
badge: label="Alfa"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: 4f7cedc4197a983d4d13294744e30836a0263d3a
workflow-type: tm+mt
source-wordcount: '312'
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
>abstract="Seleziona il pubblico migliore per il messaggio SMS."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selezione modello SMS"
>abstract="Seleziona un modello predefinito per avviare la consegna SMS."

1. Dalla pagina home delle **[!UICONTROL Consegne]**, fai clic su **[!UICONTROL Crea consegna]**.

1. Nella sezione **[!UICONTROL Canale]**, scegli SMS come canale e seleziona un modello. [Ulteriori informazioni sui modelli](../msg/delivery-template.md)

1. Fai clic sul pulsante **[!UICONTROL Crea una consegna]** per confermare.

   ![](assets/sms_create_1.png)

1. Immetti un’**[!UICONTROL etichetta]** per la consegna e accedi al menu a discesa **[!UICONTROL Opzioni aggiuntive]**.

   +++Configura le seguenti impostazioni in base alle tue esigenze.
   * **[!UICONTROL Nome interno]**: assegna un identificatore univoco alla consegna.
   * **[!UICONTROL Cartella]**: memorizza la consegna in una cartella specifica.
   * **[!UICONTROL Codice di consegna]**: organizza le consegne in base alla convenzione di denominazione.
   * **[!UICONTROL Descrizione]**: specifica una descrizione della consegna.
   * **[!UICONTROL Natura]**: specifica la natura dell’e-mail a scopo di classificazione.
+++

1. Fai clic sul pulsante **[!UICONTROL Seleziona pubblico]** per eseguire il targeting di un pubblico esistente o crearne uno tuo. [Ulteriori informazioni](../audience/about-audiences.md).

   ![](assets/sms_create_2.png)

1. Attiva l’opzione **[!UICONTROL Abilita gruppo di controllo]** per impostare un gruppo di controllo per misurare l’impatto della consegna che consente di confrontare il comportamento della popolazione che ha ricevuto il messaggio con quello dei contatti che non lo hanno fatto. [Ulteriori informazioni](../audience/control-group.md)

1. Fai clic su **[!UICONTROL Modifica contenuto]** per iniziare a progettare il contenuto del messaggio SMS. [Ulteriori informazioni](content-sms.md)

   ![](assets/sms_create_4.png)

   Da questa schermata, è possibile anche [simulare i contenuti](../preview-test/preview-test.md) e [configurare le offerte](../content/offers.md).

1. Per pianificare la consegna a una data e un’ora specifiche, attiva l’opzione **[!UICONTROL Abilita pianificazione]**. Dopo aver avviato la consegna, il messaggio viene inviato automaticamente nella data e nell’ora esatte definite per il destinatario.

1. Fai clic su **[!UICONTROL Configura le impostazioni di consegna]** per accedere alle opzioni avanzate relative al modello di consegna. [Ulteriori informazioni](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
