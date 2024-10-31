---
audience: end-user
title: Piani e programmi
description: Scopri come creare e configurare piani e programmi in Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 5%

---

# Piani e programmi {#plan-and-programs}

Adobe Campaign consente di configurare la gerarchia di cartelle per i piani e i programmi di marketing.

Per organizzarle meglio, Adobe consiglia la seguente gerarchia: Pianificare `>` programmi `>` campagne

* Un **piano** può contenere più programmi. Definisce obiettivi strategici per un certo periodo di tempo.
* Un **programma** può contenere altri programmi, oltre a campagne, flussi di lavoro e pagine di destinazione.
* Una **campagna** può contenere consegne, flussi di lavoro e pagine di destinazione.

## Creare e configurare un piano {#create-plan}

Per creare un piano, devi creare una cartella con tipo di cartella **[!UICONTROL Piano]** [Ulteriori informazioni sulla creazione di una cartella](../get-started/work-with-folders.md).

![](assets/plan_create.png){zoomable="yes"}

Vai alle **[!UICONTROL impostazioni cartella]** del piano per gestirlo.

![](assets/plan_settings.png){zoomable="yes"}

Puoi definire **[!UICONTROL Opzioni personalizzate]** e impostare la data di pianificazione del piano.

![](assets/plan_options.png){zoomable="yes"}

Per gestire le **[!UICONTROL opzioni personalizzate]**:

1. Individua gli **[!UICONTROL schemi]**
1. Scegli gli schemi **[!UICONTROL Modificabili]** nei filtri
1. Fai clic sull&#39;icona di **[!UICONTROL Modifica dettagli personalizzati]**

![](assets/plan_edit.png){zoomable="yes"}

Puoi configurarli:

![](assets/plan_customfields.png){zoomable="yes"}

## Creare e configurare un programma

Per creare un programma nel piano ([Ulteriori informazioni sulla creazione di un piano](#create-plan)), devi essere nel piano e creare una cartella con il tipo di cartella **[!UICONTROL Programma]** [Ulteriori informazioni sulla creazione di una cartella](../get-started/work-with-folders.md).

![](assets/program_create.png){zoomable="yes"}

Vai a **[!UICONTROL Impostazioni cartella]** del programma per gestirlo.

![](assets/program_settings.png){zoomable="yes"}

Puoi definire **[!UICONTROL Opzioni personalizzate]** e impostare la data di pianificazione del programma.

![](assets/program_options.png){zoomable="yes"}

Per gestire le **[!UICONTROL opzioni personalizzate]**:

1. Individua gli **[!UICONTROL schemi]**
1. Scegli gli schemi **[!UICONTROL Modificabili]** nei filtri
1. Fai clic sull&#39;icona di **[!UICONTROL Modifica dettagli personalizzati]**

![](assets/program_edit.png){zoomable="yes"}

Puoi configurarli:

![](assets/program_customfields.png){zoomable="yes"}

## Come collegare una campagna a un programma

Puoi collegare una campagna a un programma in due modi:

### Modo #1: disponi già di un programma e desideri creare una campagna collegata

Per collegare una nuova campagna al programma, crea direttamente la campagna nel programma:

![](assets/program_campaign_create.png){zoomable="yes"}

Le impostazioni di **[!UICONTROL Cartella]** verranno archiviate automaticamente nel percorso del programma.

![](assets/program_campaign_folder.png){zoomable="yes"}

### #2: disponi già di una campagna e desideri collegarla a un programma esistente

Passa al pulsante **[!UICONTROL Impostazioni]** della campagna da collegare al programma:

![](assets/campaign_settings.png){zoomable="yes"}

Nelle **[!UICONTROL Proprietà]**, fai clic sull&#39;icona **[!UICONTROL Cartella]** nelle impostazioni **[!UICONTROL Cartella]** per scegliere la cartella **[!UICONTROL Programma]**.

![](assets/campaign_folder.png){zoomable="yes"}

Seleziona la cartella **[!UICONTROL Programma]** e fai clic sul pulsante **[!UICONTROL Conferma]**, quindi sul pulsante **[!UICONTROL Salva e chiudi]**.

![](assets/campaign_linked.png){zoomable="yes"}

La campagna è ora elencata nel programma:

![](assets/campaign_in_program.png){zoomable="yes"}
