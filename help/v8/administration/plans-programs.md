---
audience: end-user
title: Piani e programmi
description: Scopri come creare e configurare piani e programmi in Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 3%

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
1. Fai clic sull&#39;icona **[!UICONTROL Modifica dettagli personalizzati]**.

![Schermata che mostra la modifica dei dettagli personalizzati per un piano](assets/plan_edit.png){zoomable="yes"}

Configura le opzioni personalizzate:

![Schermata che mostra la configurazione dei campi personalizzati per un piano](assets/plan_customfields.png){zoomable="yes"}

## Creare e configurare un programma

Per creare un programma nel piano ([Ulteriori informazioni sulla creazione di un piano](#create-plan)), passare al piano e creare una cartella con il tipo di cartella **[!UICONTROL Programma]**. [Ulteriori informazioni sulla creazione di una cartella](../get-started/work-with-folders.md).

![Schermata che mostra la creazione di una cartella di programmi](assets/program_create.png){zoomable="yes"}

Vai a **[!UICONTROL Impostazioni cartella]** del programma per gestirlo.

![Schermata che mostra le impostazioni della cartella per un programma](assets/program_settings.png){zoomable="yes"}

Definisci **[!UICONTROL Opzioni personalizzate]** e imposta la data di pianificazione del programma.

![Schermata che mostra le opzioni personalizzate per un programma](assets/program_options.png){zoomable="yes"}

Per gestire le **[!UICONTROL opzioni personalizzate]**:

1. Individua gli **[!UICONTROL Schemi]**.
1. Scegli gli schemi **[!UICONTROL Modificabili]** nei filtri.
1. Fai clic sull&#39;icona **[!UICONTROL Modifica dettagli personalizzati]**.

![Schermata che mostra la modifica dei dettagli personalizzati per un programma](assets/program_edit.png){zoomable="yes"}

Configura le opzioni personalizzate:

![Schermata che mostra la configurazione dei campi personalizzati per un programma](assets/program_customfields.png){zoomable="yes"}

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