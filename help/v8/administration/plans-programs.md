---
audience: end-user
title: Piani e programmi
description: Scopri come creare e configurare piani e programmi in Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 640
ht-degree: 5%

---

# Piani e programmi {#plan-and-programs}

Adobe Campaign consente di configurare la gerarchia di cartelle per i piani e i programmi di marketing.

Per una migliore organizzazione di questi componenti, Adobe consiglia la seguente gerarchia: Pianificare `>` programmi `>` campagne.

* Un **piano** può contenere più programmi. Definisce obiettivi strategici per un periodo specifico.
* Un **programma** può contenere altri programmi, oltre a campagne, flussi di lavoro e pagine di destinazione.
* Una **campagna** può contenere consegne, flussi di lavoro e pagine di destinazione.

## Creare e configurare un piano {#create-plan}

Per creare un piano, creare una cartella con il tipo di cartella **[!UICONTROL Piano]**. [Ulteriori informazioni sulla creazione di una cartella](../get-started/work-with-folders.md)

![Schermata che mostra la creazione di una cartella del piano](assets/plan_create.png){zoomable="yes"}

Vai alle **[!UICONTROL impostazioni cartella]** del piano per gestirlo.

![Schermata che mostra le impostazioni della cartella per un piano](assets/plan_settings.png){zoomable="yes"}

Definisci **[!UICONTROL Opzioni personalizzate]** e imposta la data di pianificazione del piano.

![Schermata che mostra le opzioni personalizzate per un piano](assets/plan_options.png){zoomable="yes"}

Per gestire le **[!UICONTROL opzioni personalizzate]**:

1. Individua gli **[!UICONTROL Schemi]**.
1. Scegli gli schemi **[!UICONTROL Modificabili]** nei filtri.
1. Fai clic sullo schema.

![Schermata che mostra la modifica dei dettagli personalizzati per un piano](assets/plan_edit.png){zoomable="yes"}

1. Fare clic sul pulsante **[!UICONTROL Edizione schermo]**.

   ![](assets/plan_edit2.png){zoomable="yes"}

Configura le opzioni personalizzate:

![Schermata che mostra la configurazione dei campi personalizzati per un piano](assets/plan_customfields.png){zoomable="yes"}

## Creare e configurare un programma {#create-program}

I programmi sono disponibili dal menu di navigazione a sinistra, simile alle visualizzazioni elenco per campagne, consegne e flussi di lavoro. La voce **[!UICONTROL Programmi]** consente di creare un programma all&#39;interno di un programma esistente, non in un piano.

Per creare il primo programma di livello superiore in un piano, passare al piano in Esplora risorse (vedere questa [sezione](#create-plan)) e creare una cartella con il tipo di cartella **[!UICONTROL Programma]**. [Ulteriori informazioni sulla creazione di una cartella](../get-started/work-with-folders.md).

Per creare un programma all’interno di un programma esistente, effettua le seguenti operazioni:

1. Passare alla voce **[!UICONTROL Programmi]** nel menu di navigazione a sinistra. Questa visualizzazione elenca tutti i programmi e consente di eseguire ricerche e filtri. Facendo clic su un programma, questo viene aperto nella visualizzazione Esplora risorse.

   ![Schermata che mostra la visualizzazione dell&#39;elenco dei programmi](assets/program_view.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Crea programma]** e configura le seguenti opzioni:

   ![Schermata della schermata Crea programma](assets/program_create.png){zoomable="yes"}

   * Immetti un **[!UICONTROL etichetta]**.
   * Selezionare il programma esistente da utilizzare come **[!UICONTROL cartella principale]**.
   * Facoltativamente, impostare un **[!UICONTROL intervallo di date]** nella sezione **[!UICONTROL Pianifica]**.

   >[!TIP]
   >
   >Se si crea un programma dalla visualizzazione Esplora risorse, la cartella padre viene impostata automaticamente sul programma corrente.

1. Fai di nuovo clic su **[!UICONTROL Crea programma]** per salvare le modifiche e creare il programma. Il programma viene quindi visualizzato nella visualizzazione Esplora risorse. Puoi rinominarlo, eliminarlo e accedere alle relative impostazioni, come qualsiasi altra cartella. È inoltre possibile creare sottoprogrammi all&#39;interno di questo programma.

   ![Schermata che mostra il programma nella visualizzazione Esplora risorse](assets/program_explorer.png){zoomable="yes"}

Le opzioni personalizzate per un programma sono configurate nello stesso modo di un piano. Vedi [Creare e configurare un piano](#create-plan).

## Come collegare una campagna a un programma

Puoi collegare una campagna a un programma in due modi:

### Modo #1: disponi già di un programma e desideri creare una campagna collegata

Per collegare una nuova campagna al programma, creala direttamente all’interno del programma.

![Schermata che mostra la creazione di una campagna all&#39;interno di un programma](assets/program_campaign_create.png){zoomable="yes"}

Le impostazioni di **[!UICONTROL Cartella]** verranno compilate automaticamente con il percorso del programma.

![Schermata che mostra le impostazioni della cartella per una campagna collegata a un programma](assets/program_campaign_folder.png){zoomable="yes"}

### #2: disponi già di una campagna e desideri collegarla a un programma esistente

Passa al pulsante **[!UICONTROL Impostazioni]** della campagna da collegare al programma.

![Schermata che mostra il pulsante delle impostazioni per una campagna](assets/campaign_settings.png){zoomable="yes"}

Nelle **[!UICONTROL Proprietà]**, fai clic sull&#39;icona **[!UICONTROL Cartella]** nelle impostazioni **[!UICONTROL Cartella]** per scegliere la cartella **[!UICONTROL Programma]**.

![Schermata che mostra la selezione della cartella per collegare una campagna a un programma](assets/campaign_folder.png){zoomable="yes"}

Seleziona la cartella **[!UICONTROL Programma]**, fai clic sul pulsante **[!UICONTROL Conferma]** e quindi sul pulsante **[!UICONTROL Salva e chiudi]**.

![Schermata che mostra una campagna collegata a un programma](assets/campaign_linked.png){zoomable="yes"}

La campagna è ora elencata nel programma.

![Schermata che mostra una campagna elencata in un programma](assets/campaign_in_program.png){zoomable="yes"}