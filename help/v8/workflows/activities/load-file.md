---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Load file
description: Scopri come utilizzare l’attività del flusso di lavoro Load file
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 49%

---

# Carica file {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Attività di caricamento file"
>abstract="L’attività **Carica file** è un’attività di **gestione dati**. Utilizza questa attività per utilizzare i dati memorizzati in un file esterno."

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

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="File target per l’attività di caricamento file"
>abstract="File target per l’attività di caricamento file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Rimappatura del valore per l’attività di caricamento file"
>abstract="Rimappatura del valore per l’attività di caricamento file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Comando Load File"
>abstract="Consentire un comando arbitrario per la pre-elaborazione è un problema di sicurezza, disabilita l’opzione di sicurezza XtkSecurity_Disable_Preproc per forzare l’uso di un elenco predefinito di comandi."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Elimina file dopo l’importazione"
>abstract="TBC"

L’attività **Carica file** è un’attività di **gestione dati**. Utilizza questa attività per lavorare con profili e dati memorizzati in un file esterno. I profili e i dati non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per [personalizzazione](../../personalization/gs-personalization.md), o per aggiornare profili o qualsiasi altra tabella.

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
