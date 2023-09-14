---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Save audience
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
badge: label="Beta"
source-git-commit: 058327a9beaca30a2d5ac84d71a8fef2333732ab
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 9%

---


# Salvare tipi di pubblico {#save-audience}

>[!CONTEXTUALHELP]
>id="???"
>title="Salvare l’attività del pubblico"
>abstract="L’attività Save audience ti consente di:"

Il **Salva pubblico** l&#39;attività è un **Targeting** attività. Questa attività ti consente di aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro. I tipi di pubblico creati vengono aggiunti all’elenco dei tipi di pubblico delle applicazioni e sono disponibili tramite **Tipi di pubblico** menu.

Questa attività viene essenzialmente utilizzata per mantenere i gruppi di popolazione calcolati nello stesso flusso di lavoro, convertendoli in tipi di pubblico riutilizzabili. Connettila ad altre attività di targeting come **Creare un pubblico** o un **Combina** attività.

## Configurazione

Per configurare il **Salva pubblico** attività:

1. Aggiungi un **Salva pubblico** al flusso di lavoro.

   ![](../assets/workflow-save-audience.png)

1. In **Modalità** a discesa, seleziona l’azione da eseguire:

   * **Creare o aggiornare un pubblico esistente**: definisci un **Etichetta del pubblico**. Se il pubblico esiste già, verrà aggiornato, altrimenti verrà creato un nuovo pubblico.

   * **Aggiornare un pubblico esistente**: scegli il **Pubblico** desideri effettuare l’aggiornamento tra i tipi di pubblico esistenti.

1. Seleziona la **Modalità di aggiornamento** che si applicheranno ai tipi di pubblico esistenti:

   * **Sostituire il contenuto del pubblico con nuovi dati**: viene sostituito tutto il contenuto del pubblico. I vecchi dati sono persi. Vengono conservati solo i dati della transizione in entrata dell’attività Save audience. Questa opzione cancella il tipo di pubblico e la dimensione di targeting del pubblico aggiornato.

   * **Completare il pubblico con nuovi dati**: il contenuto del pubblico precedente viene mantenuto e i dati della transizione in entrata dell’attività Save audience vengono aggiunti a esso.

1. Controlla la **Genera complemento** se desideri sfruttare il gruppo rimanente. Verrà quindi aggiunta una transizione aggiuntiva all’attività.

Il contenuto del pubblico salvato è quindi disponibile nella relativa visualizzazione dettagliata, accessibile dalla **Tipi di pubblico** menu. Le colonne disponibili in questa visualizzazione corrispondono a quelle della transizione in entrata del **Crea pubblico** attività.


## Esempio



