---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Load file
description: Scopri come utilizzare l’attività del flusso di lavoro Load file
badge: label="Disponibilità limitata"
source-git-commit: 6068e3695ebed22a94a75b9aded59d1e5fb6b47a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 40%

---

# Attività Load file {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Attività di caricamento file"
>abstract="Il **Carica file** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per lavorare con i profili memorizzati in un file esterno."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="File di esempio"
>abstract="File di esempio"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nome del file"
>abstract="Nome del file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Database di destinazione"
>abstract="Database di destinazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Rifiuta la gestione per l’attività di caricamento file"
>abstract="Rifiuta la gestione per l’attività di caricamento file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Rifiuta la gestione della transizione in uscita"
>abstract="Rifiuta la gestione della transizione in uscita"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Rifiuta la gestione della transizione in uscita per i valori rifiutati"
>abstract="Rifiuta la gestione della transizione in uscita per i valori rifiutati"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formattazione per l’attività di caricamento file"
>abstract="Formattazione per l’attività di caricamento file"


Il **Carica file** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per lavorare con i profili memorizzati in un file esterno. I profili non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per [personalizzazione](../../personalization/gs-personalization.md), o per aggiornare i profili.


>[!NOTE]
>Sono supportati i formati di file di testo (TXT) e i valori separati da virgole (CSV).


Questa attività può essere utilizzata con [Reconciliation](reconciliation.md) attività per collegare dati non identificati a risorse esistenti. Ad esempio, il **Carica file** l&#39;attività può essere inserita prima di un **Reconciliation** se importi dati non standard nel database.


## Configurare l’attività Load file {#load-configuration}

Per configurare il **Carica file** attività:


1. Trascina una **Carica file** attività nel flusso di lavoro. Fai clic su **Seleziona da file** pulsante.
1. Seleziona il file locale da usare. Il formato deve essere allineato con [file di esempio](../../audience/file-audience.md#sample-file).
1. Visualizza in anteprima e verifica la modalità di mappatura dei dati nella sezione centrale dello schermo.
1. Regola le impostazioni delle colonne e il formato dei dati dalle opzioni disponibili.
1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

## Esempio{#load-example}

Un esempio di caricamento di un file esterno è disponibile con **Reconciliation** attività in [questa sezione](reconciliation.md#example).