---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Load file
description: Scopri come utilizzare l’attività del flusso di lavoro Load file
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 4518f7a2f280eca70f799b941c5d28bdc39c1def
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 14%

---

# Carica file {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Attività di caricamento file"
>abstract="L’attività **Carica file** è un’attività di **gestione dati**. Utilizza questa attività per lavorare con i dati memorizzati in un file esterno. I profili e i dati non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per la personalizzazione, per l’aggiornamento dei profili o di qualsiasi altra tabella. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Rifiuta la gestione della transizione in uscita"
>abstract="Rifiuta la gestione della transizione in uscita"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Rifiuta la gestione della transizione in uscita per i valori rifiutati"
>abstract="Rifiuta la gestione della transizione in uscita per i valori rifiutati"


L’attività **Carica file** è un’attività di **gestione dati**. Utilizza questa attività per lavorare con profili e dati memorizzati in un file esterno. I profili e i dati non vengono aggiunti al database, ma tutti i campi nel file di input sono disponibili per [personalizzazione](../../personalization/gs-personalization.md), o per aggiornare profili o qualsiasi altra tabella.

>[!NOTE]
>Sono supportati i formati di file di testo (TXT) e i valori separati da virgole (CSV). È possibile caricare file con una dimensione massima di 50 MB.

Questa attività può essere utilizzata con [Reconciliation](reconciliation.md) attività per collegare dati non identificati a risorse esistenti. Ad esempio, il **Carica file** l&#39;attività può essere inserita prima di un **Reconciliation** se importi dati non standard nel database.

## Configurare l’attività Load file {#load-configuration}

Il **Carica file** la configurazione dell’attività prevede due passaggi. Innanzitutto, devi definire la struttura del file prevista effettuando il caricamento di un file di esempio. Al termine, puoi specificare l’origine del file di cui verranno importati i dati. Segui i passaggi seguenti per configurare l’attività.

![](../assets/workflow-load-file.png)

### Configurare il file di esempio {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="File di esempio"
>abstract="Seleziona la struttura di file prevista caricando un file di esempio."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formattazione per l’attività di caricamento file"
>abstract="In **Formattazione** , specificare la formattazione del file per garantire che i dati vengano importati correttamente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Rimappatura del valore per l’attività di caricamento file"
>abstract="Utilizza questa opzione per mappare valori specifici dai file caricati con nuovi valori. Ad esempio, se la colonna contiene i valori &quot;True&quot;/&quot;False&quot;, puoi aggiungere una mappatura per sostituire automaticamente tali valori con i caratteri &quot;0&quot;/&quot;1&quot;."

Segui questi passaggi per configurare il file di esempio utilizzato per definire la struttura di file prevista:

1. Aggiungi un **Carica file** attività nel flusso di lavoro.

1. Seleziona il file di esempio da utilizzare per definire la struttura di file prevista. A questo scopo, fai clic su **Seleziona file** pulsante in **[!UICONTROL File di esempio]** e selezionare il file locale da utilizzare.

   >[!NOTE]
   >
   >I dati del file di esempio sono utilizzati per la configurazione dell’attività, ma non vengono importati. È consigliabile utilizzare un file di esempio contenente pochi dati. Il formato del file deve essere allineato con questo [file di esempio](../../audience/file-audience.md#sample-file).

1. Viene visualizzata un&#39;anteprima del file di esempio, con un massimo di 30 righe.

1. In **[!UICONTROL Tipo di file]** , specificare se il file utilizza colonne delimitate o colonne a larghezza fissa.

   ![](../assets/workflow-load-file-sample.png)

1. Per i tipi di file di colonne delimitate, utilizza **Colonne** per configurare le proprietà di ciascuna colonna.

   +++Opzioni disponibili per le colonne di file

   * **[!UICONTROL Etichetta]**: etichetta da visualizzare per la colonna.
   * **[!UICONTROL Tipo di dati]**: tipo di dati contenuti nella colonna.
   * **[!UICONTROL Larghezza]** (tipo di dati stringa): numero massimo di caratteri da visualizzare nella colonna.
   * **[!UICONTROL Trasformazione dei dati]** (tipo di dati stringa): applica la trasformazione ai valori contenuti nella colonna.
   * **[!UICONTROL Gestione degli spazi vuoti]** (tipo di dati string): specifica come gestire gli spazi contenuti nella colonna.
   * **[!UICONTROL Separatori]** (tipi di dati data, ora, numero intero e numero)*: specifica i caratteri da utilizzare come separatori.
   * **[!UICONTROL Consenti valori NULL]**: specifica come gestire i valori vuoti nella colonna. Se è presente un valore vuoto, l’opzione &quot;Adobe Campaign default&quot; genera un errore.
   * **[!UICONTROL Errore di elaborazione]** (tipo di dati stringa): specifica il comportamento in caso di errori in una delle righe.
   * **[!UICONTROL Modifica del valore]**: questa opzione consente di mappare valori specifici con valori nuovi. Ad esempio, se la colonna contiene i valori &quot;True&quot;/&quot;False&quot;, puoi aggiungere una mappatura per sostituire automaticamente tali valori con i caratteri &quot;0&quot;/&quot;1&quot;.

+++

1. In **Formattazione** , specificare la formattazione del file per garantire che i dati vengano importati correttamente.

### Definisci il file di destinazione da caricare {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="File target per l’attività di caricamento file"
>abstract="In **[!UICONTROL File di destinazione]** , specifica come recuperare il file da caricare sul server."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nome del file"
>abstract="Specifica il nome del campo da caricare sul server. Fai clic su **[!UICONTROL Apri finestra di dialogo per personalizzazione]** per utilizzare l’editor di espressioni, incluse le variabili evento, per calcolare il nome del file."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Database di destinazione"
>abstract="Se stai accedendo a un **[!UICONTROL Carica file]** che è già stata configurata nella console client, un&#39;ulteriore **[!UICONTROL Database di destinazione]** Questa sezione è disponibile se hai configurato l’attività per caricare il file in un database esterno."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Comando Load File"
>abstract="Consentire un comando arbitrario per la pre-elaborazione è un problema di sicurezza, disabilita l’opzione di sicurezza XtkSecurity_Disable_Preproc per forzare l’uso di un elenco predefinito di comandi."

>[!CAUTION]
>
>Prima di caricare il file di destinazione, accertati che sia conforme alla formattazione del file di esempio. Eventuali discrepanze nel formato del file, nella struttura delle colonne o nel numero di colonne possono causare errori durante l’esecuzione del flusso di lavoro.

Per definire il file di destinazione da caricare, effettua le seguenti operazioni:

1. In **[!UICONTROL File di destinazione]** , specificare l&#39;azione da eseguire durante il recupero del file da caricare sul server.

   * **[!UICONTROL Carica file dal computer locale]**: seleziona il file da caricare dal computer.

   * **[!UICONTROL Specificato nella transizione]**: carica il file specificato nella transizione in entrata in arrivo da un’attività precedente, ad esempio **[!UICONTROL Trasferisci file]**.

   * **[!UICONTROL Pre-elabora il file]**: carica il file specificato nella transizione precedente e applica a tale file un comando di pre-elaborazione, ad esempio **[!UICONTROL Decompressione]** o **[!UICONTROL Decrittografa]**.

   * **[!UICONTROL Calcolato]**: carica il file il cui nome è specificato nella **[!UICONTROL Nome file]** campo. Fai clic su **[!UICONTROL Apri finestra di dialogo per personalizzazione]** per utilizzare l’editor di espressioni, incluse le variabili evento, per calcolare il nome del file.

   ![](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Se stai accedendo a un **[!UICONTROL Carica file]** che è già stata configurata nella console client, un&#39;ulteriore **[!UICONTROL Database di destinazione]** Questa sezione mostra se hai configurato l’attività per caricare il file in un database esterno. Ti consente di specificare se desideri caricare il file sul server Campaign o sul database esterno.

### Opzioni aggiuntive {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Rifiuta la gestione per l’attività di caricamento file"
>abstract="In **Gestione dei rifiuti** , specifica il comportamento dell&#39;attività in caso di errori. Puoi definire il numero massimo di errori da consentire e attivare/disattivare la **[!UICONTROL Mantieni i rifiuti in un file]** per scaricare sul server un file contenente gli errori verificatisi durante l’importazione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Elimina file dopo l’importazione"
>abstract="Attiva/disattiva **Elimina file dopo l’importazione** per eliminare il file originale dal server dopo averlo importato."


1. In **Gestione dei rifiuti** , specifica il comportamento dell&#39;attività in caso di errori:

   * In **[!UICONTROL Dele]** specificare il numero massimo di errori autorizzati durante l&#39;elaborazione del file da caricare. Ad esempio, se il valore è impostato su &quot;20&quot;, l’esecuzione del flusso di lavoro avrà esito negativo se si verificano più di 20 errori durante il caricamento del file.

   * Per mantenere gli errori che si sono verificati durante il caricamento del file, attiva/disattiva **[!UICONTROL Mantieni i rifiuti in un file]** e specificare il nome desiderato per il file nella **[!UICONTROL File di rifiuto]** campo.

     Dopo aver attivato questa opzione, dopo l’attività viene aggiunta una transizione di output aggiuntiva denominata &quot;Complemento&quot;. Qualsiasi errore che si verificherà durante l&#39;importazione verrà memorizzato nel file specificato sul server.

1. Per eliminare il file caricato dal server dopo l’esecuzione del flusso di lavoro, attiva/disattiva **[!UICONTROL Elimina file dopo l’importazione]** opzione.

   ![](../assets/workflow-load-file-options.png)

1. Fai clic su **Conferma** una volta che le impostazioni sono corrette.

## Esempio {#load-example}

Esempio di caricamento di un file esterno utilizzato con **Reconciliation** l&#39;attività è disponibile in [questa sezione](reconciliation.md#reconciliation-example).
