---
audience: end-user
title: Utilizzare un pubblico di Adobe Experience Platform
description: Scopri come utilizzare un pubblico da Adobe Experience Platform
badge: label="Alpha" type="Positive"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 958d3ca6ab7eb05a3201ed3344d4659a8756e3ef
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 40%

---

# Utilizzare un pubblico di Adobe Experience Platform{#aep-audience}

I connettori di origine e destinazione del Cloud Service gestito di Adobe Campaign consentono un’integrazione perfetta tra Adobe Campaign e Adobe Experience Platform.

Dopo aver creato un pubblico di Adobe Experience Platform e averlo reso disponibile nella console client, puoi utilizzarlo nello stesso modo in cui si farebbe per un pubblico di Campaign per personalizzare e inviare messaggi.

>[!NOTE]
>
>Per utilizzare i tipi di pubblico di Adobe Experience Platform in Campaign, devi configurare l’integrazione con Origini e Destinazioni Adobi. Fai riferimento a [Documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=it){target="_blank"}.


Per selezionare il pubblico di una consegna, puoi anche:

* Crea un nuovo pubblico. [Ulteriori informazioni](segment-builder.md)
* Carica un pubblico da un file esterno. [Ulteriori informazioni](file-audience.md)
* Utilizza un pubblico di Campaign esistente. [Ulteriori informazioni](add-audience.md).

Per selezionare un pubblico Adobe Experience Platform per la consegna, segui i passaggi seguenti:

1. Dalla sezione **Pubblico** nell’assistente per la creazione della consegna, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   ![](assets/create-audience.png)

1. Scegli **[!UICONTROL Seleziona pubblico]** per utilizzare un pubblico esistente. Per creare un nuovo pubblico da utilizzare in questo messaggio e-mail, scegli **Crea nuovo**. Fai riferimento a questa [sezione](segment-builder.md).

   In questa schermata vengono visualizzati tutti i tipi di pubblico esistenti definiti nella console client di Adobe Campaign per la cartella corrente. Per scegliere un pubblico da Adobe Experience Platform, passa a `AEP Audiences folder` dalla sezione filter (filtro) dello schermo.

   ![](assets/select-audience-folder.png)

   Puoi anche definire una regola per filtrare in base all’origine dei tipi di pubblico, come segue:

   ![](assets/filter-on-aep-audience.png)

1. Scegli un pubblico e fai clic su **Seleziona**.

1. Per perfezionare il pubblico, fai clic su **Modifica regole**.

   ![](assets/refine-audience.png)

1. Utilizzando il generatore di regole, puoi arricchire il pubblico con filtri aggiuntivi o combinando diversi tipi di pubblico. Consulta questa [sezione](segment-builder.md).

1. Fai clic su **Salva**.


