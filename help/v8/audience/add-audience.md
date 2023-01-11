---
audience: end-user
title: Aggiungere un pubblico
description: Documentazione Web di Campaign v8
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 4%

---

# Seleziona un pubblico {#add-audience}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selezionare un pubblico esistente"
>abstract="I tipi di pubblico sono definiti nella console Adobe Campaign v8. Se disponi di un’integrazione Adobe Experience Platform disponibile, dovresti essere in grado di visualizzare anche i tipi di pubblico definiti da Platform."

In questa sezione viene illustrato come selezionare un pubblico esistente durante la definizione della popolazione target di una consegna e-mail. Per creare un nuovo pubblico, consulta [sezione](segment-builder.md).

1. Da **Pubblico** nell’assistente per la creazione della consegna, fai clic sul pulsante **[!UICONTROL Selezionare il pubblico]** pulsante .

   ![](assets/create-audience.png)

1. Scegli **[!UICONTROL Selezionare il pubblico]** per utilizzare un pubblico esistente. Per creare un nuovo pubblico da utilizzare in questo messaggio e-mail, scegli **Crea il tuo**. Fai riferimento a questo [sezione](segment-builder.md).

   In questa schermata vengono visualizzati tutti i tipi di pubblico esistenti definiti nella console Adobe Campaign o da Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Per sfruttare i tipi di pubblico di Adobe Experience Platform, devi configurare l’integrazione con le destinazioni. Fai riferimento a [Documentazione sulle destinazioni](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=it).

1. Scegli un pubblico e fai clic su **Seleziona**.

1. Fai clic su **Modifica regole** per perfezionare il pubblico.

   ![](assets/create-audience3.png)

1. Utilizzando il generatore di regole, puoi arricchire il pubblico con filtri aggiuntivi o combinando diversi tipi di pubblico. Vedi questo [sezione](segment-builder.md).

   ![](assets/create-audience4.png)

1. Fai clic su **Salva**.

Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceverà il messaggio. Ciò ti consente di confrontare il comportamento della popolazione che ha ricevuto il messaggio con il comportamento dei contatti che non lo hanno fatto. Vedi [sezione](control-group.md).