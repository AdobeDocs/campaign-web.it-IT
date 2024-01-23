---
audience: end-user
title: Utilizzare un pubblico di Adobe Experience Platform
description: Scopri come utilizzare un pubblico da Adobe Experience Platform
badge: label="Disponibilità limitata"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 85%

---

# Utilizzare un pubblico di Adobe Experience Platform{#aep-audience}

I connettori di origine e destinazione del Cloud Service gestito di Adobe Campaign consentono un’integrazione ottimizzata tra Adobe Campaign e Adobe Experience Platform.

Dopo aver creato un pubblico di Adobe Experience Platform e averlo reso disponibile nella console client, puoi utilizzarlo nello stesso modo in cui lo useresti per un pubblico di Campaign per personalizzare e inviare messaggi.

>[!NOTE]
>
>Per utilizzare i tipi di pubblico di Adobe Experience Platform in Campaign, devi configurare l’integrazione con origini e destinazioni di Adobe. Consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=it){target="_blank"}.

Per selezionare il pubblico di una consegna, puoi anche:

* Creare un nuovo pubblico. [Ulteriori informazioni](../query/query-modeler-overview.md)
* Caricare un pubblico da un file esterno. [Ulteriori informazioni](file-audience.md)
* Utilizzare un pubblico esistente di Campaign. [Ulteriori informazioni](add-audience.md).

Per selezionare un pubblico di Adobe Experience Platform per la consegna, segui questi passaggi:

1. Dalla sezione **Pubblico** nell’assistente per la creazione della consegna, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   ![](assets/create-audience.png)

1. Scegli **[!UICONTROL Seleziona pubblico]** per utilizzare un pubblico esistente. Per creare un nuovo pubblico da utilizzare in questo messaggio e-mail, scegli **Crea nuovo**. Fai riferimento a questa [sezione](../query/query-modeler-overview.md).

   In questa schermata vengono visualizzati tutti i tipi di pubblico esistenti che sono stati definiti nella console client di Adobe Campaign per la cartella corrente. Per scegliere un pubblico da Adobe Experience Platform, passa a `AEP Audiences folder` dalla sezione filtro dello schermo.

   ![](assets/select-audience-folder.png)

   Puoi anche definire una regola per filtrare in base all’origine dei tipi di pubblico, nel modo seguente:

   La sezione dei filtri consente di accedere alle opzioni di filtro per perfezionare l’elenco dei tipi di pubblico. A questo scopo, fai clic su **Aggiungi regole** per accedere a query modeler, che consente di creare filtri avanzati per l’elenco dei tipi di pubblico. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md)

   ![](assets/filter-on-aep-audience.png)

1. Scegli un pubblico e fai clic su **Seleziona**.

1. Per perfezionare il pubblico, fai clic su **Modifica regole**.

   ![](assets/refine-audience.png)

1. Utilizzando il modellatore di query, puoi arricchire il pubblico con filtri aggiuntivi o combinando tipi di pubblico diversi. Consulta questa [sezione](../query/query-modeler-overview.md).

1. Fai clic su **Salva**.
