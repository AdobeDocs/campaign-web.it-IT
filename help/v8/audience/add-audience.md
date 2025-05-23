---
audience: end-user
title: Selezionare un pubblico esistente
description: Scopri come selezionare un pubblico
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 39%

---

# Selezionare un pubblico esistente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selezionare un pubblico esistente"
>abstract="Sfoglia l’elenco per selezionare un pubblico esistente. Utilizza l’icona “Mostra filtri” per filtrare l’elenco o seleziona una cartella specifica."

Questa sezione spiega come selezionare un pubblico esistente durante la definizione della popolazione target di una consegna. Quando definisci il target principale di una consegna, puoi anche:
* [Crea un pubblico una tantum](one-time-audience.md) utilizzando il modellatore di query.
* [Caricare un pubblico da un file esterno](file-audience.md) (solo per e-mail).

I tipi di pubblico che possono essere oggetto di targeting nelle consegne sono accessibili dal menu **Pubblico** a sinistra. Hanno origine da più origini, ad esempio la console client, i flussi di lavoro del pubblico web di Campaign o Adobe Experience Platform. [Ulteriori informazioni sui tipi di pubblico](manage-audience.md)

Per selezionare un pubblico esistente per il messaggio, segui questi passaggi:

1. Dalla sezione **Pubblico** dell&#39;assistente alla creazione della consegna, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**, quindi scegli **[!UICONTROL Seleziona pubblico]**.

   [Questa schermata mostra il pulsante **Seleziona pubblico** nell&#39;assistente per la creazione della consegna.](assets/create-audience.png){zoomable="yes"}

1. In questa schermata vengono visualizzati tutti i tipi di pubblico esistenti per la cartella corrente.

   [Questa schermata mostra l&#39;elenco dei tipi di pubblico esistenti nella cartella corrente.](assets/create-audience2.png){zoomable="yes"}

   Per scegliere un pubblico da Adobe Experience Platform, passa a `AEP Audiences folder` dalla sezione dei filtri della schermata. [Ulteriori informazioni sui tipi di pubblico di Adobe Experience Platform](manage-audience.md#monitor)

   [Questa schermata mostra la sezione dei filtri con la cartella Tipi di pubblico di AEP selezionata.](assets/select-audience-folder.png){zoomable="yes"}

1. La sezione dei filtri consente di accedere alle opzioni di filtro per perfezionare l’elenco dei tipi di pubblico. A questo scopo, fai clic su **Aggiungi regole** per accedere al modellatore di query, che consente di creare filtri avanzati per l&#39;elenco dei tipi di pubblico. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md)

   Ad esempio, puoi definire una regola per filtrare in base all’origine dei tipi di pubblico, come illustrato di seguito:

   [Questa schermata mostra un filtro applicato ai tipi di pubblico in base alla loro origine.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Fai clic su **Conferma** per aggiungere il pubblico come target principale della consegna. Al termine, puoi perfezionare il pubblico utilizzando Query Modeler facendo clic sul pulsante **Modifica regole**.

   [Questa schermata mostra il pulsante **Modifica regole** per perfezionare il pubblico.](assets/refine-audience.png){zoomable="yes"}

1. Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceve il messaggio. Ciò ti consente di confrontare il comportamento della popolazione che ha ricevuto il messaggio con il comportamento dei contatti che non lo hanno fatto. [Ulteriori informazioni](control-group.md)