---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Load file
description: Scopri come utilizzare l’attività del flusso di lavoro Load file
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 31%

---

# Carica file {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Attività di caricamento file"
>abstract="Il **Carica file** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per lavorare con i dati memorizzati in un file esterno."

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

Il **Carica file** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per lavorare con profili e dati memorizzati in un file esterno. I profili e i dati non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per [personalizzazione](../../personalization/gs-personalization.md), o per aggiornare profili o qualsiasi altra tabella.

>[!NOTE]
>Sono supportati i formati di file di testo (TXT) e i valori separati da virgole (CSV).

Questa attività può essere utilizzata con [Reconciliation](reconciliation.md) attività per collegare dati non identificati a risorse esistenti. Ad esempio, il **Carica file** l&#39;attività può essere inserita prima di un **Reconciliation** se importi dati non standard nel database.

## Configurare l’attività Load file {#load-configuration}

Per configurare il **Carica file** attività:

1. Trascina una **Carica file** attività nel flusso di lavoro. Fai clic su **Seleziona da file** pulsante.

1. Seleziona il file locale da usare. Il formato deve essere allineato con questo [file di esempio](../../audience/file-audience.md#sample-file).

1. Visualizza in anteprima e verifica la modalità di mappatura dei dati nella sezione centrale dello schermo.

   ![](../assets/load-file.png)

1. Utilizza il **Colonne** nel riquadro sinistro per regolare il tipo di dati e la larghezza di ogni colonna.

1. In **Formattazione** nella configurazione delle colonne, specifica come viene formattato il file esterno per garantire che i dati vengano importati correttamente.

1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

## Esempio{#load-example}

Esempio di caricamento di un file esterno utilizzato con **Reconciliation** l&#39;attività è disponibile in [questa sezione](reconciliation.md#reconciliation-example).
