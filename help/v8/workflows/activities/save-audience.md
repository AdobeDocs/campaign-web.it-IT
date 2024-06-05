---
audience: end-user
title: Utilizzare l’attività Salva pubblico nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: 75c612d50d2d4a675829a412e2c4f55ed1cb817c
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 97%

---

# Salvare il pubblico {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Salva un pubblico"
>abstract="Utilizza questa attività per aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro. I tipi di pubblico creati vengono aggiunti all’elenco dei tipi di pubblico e sono disponibili tramite il menu **Tipi di pubblico**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Genera transizione in uscita"
>abstract="Utilizza questa opzione se desideri aggiungere una transizione dopo l’attività **Salva pubblico**."

L’attività **Salva pubblico** è un’attività di **targeting**. Questa attività consente di aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro. I tipi di pubblico creati vengono aggiunti all’elenco dei tipi di pubblico delle applicazioni e sono disponibili tramite il menu **Tipi di pubblico**.

Questa attività è essenzialmente utilizzata per mantenere i gruppi di popolazione calcolati nello stesso flusso di lavoro, convertendoli in tipi di pubblico riutilizzabili. Connettila ad altre attività di targeting, come a un’attività **Crea pubblico** o **Combina**.

## Configurare l’attività Salva pubblico{#save-audience-configuration}

Per configurare l’attività **Salva pubblico**, segui questi passaggi:

![](../assets/workflow-save-audience.png)

1. Aggiungi un’attività **Salva pubblico** al flusso di lavoro.

1. Nell’elenco a discesa **Modalità**, seleziona l’azione da eseguire:

   * **Crea o aggiorna un pubblico esistente**: definisci un’**etichetta del pubblico**. Se il pubblico esiste già, verrà aggiornato; altrimenti verrà creato un nuovo pubblico.

   * **Aggiorna un pubblico esistente**: scegli il **Pubblico** che desideri aggiornare dall’elenco dei tipi di pubblico esistenti.

1. Seleziona la **Modalità di aggiornamento** che verrà applicata ai tipi di pubblico esistenti:

   * **Sostituisci il contenuto del pubblico con nuovi dati**: viene sostituito tutto il contenuto del pubblico. I vecchi dati vanno perduti. Vengono conservati solo i dati della transizione in entrata dell’attività Salva pubblico. Questa opzione elimina il tipo di pubblico e la dimensione di targeting del pubblico aggiornato.

   * **Completa il pubblico con i nuovi dati**: il vecchio contenuto del pubblico viene conservato e vi vengono aggiunti i dati della transizione in entrata dell’attività Salva pubblico.

1. Seleziona l’opzione **Genera una transizione in uscita** se desideri aggiungere una transizione dopo l’attività **Salva pubblico**.

Il contenuto del pubblico salvato è quindi disponibile nella relativa visualizzazione dettagliata, accessibile dal menu **Tipi di pubblico**. Le colonne disponibili in questa vista corrispondono alle colonne della transizione in entrata dell’attività **Salva pubblico** del flusso di lavoro.


## Esempio{#save-audience-example}

L’esempio seguente illustra un semplice aggiornamento del pubblico dal targeting. Viene aggiunto un modulo di pianificazione per eseguire il flusso di lavoro una volta al mese. Una query recupera tutti i profili abbonati alle diverse applicazioni disponibili. L’attività **Salva pubblico** aggiorna il pubblico eliminando i profili per i quali è stata annullata l’iscrizione al servizio dall’ultima esecuzione del flusso di lavoro e aggiungendo i nuovi profili iscritti.
