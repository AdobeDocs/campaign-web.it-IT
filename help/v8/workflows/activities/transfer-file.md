---
audience: end-user
title: Utilizzare l’attività Transfer file
description: Scopri come utilizzare l’attività del flusso di lavoro Trasferisci file
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 160ae5704601d1f8de41ebadde353a7097d9606c
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 13%

---

# Trasferimento file {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Trasferimento file"
>abstract="L’attività **Trasferimento file** consente di ricevere o inviare file, verificare la presenza di file o elencarli su un server. Il protocollo utilizzato può essere un protocollo da server a server o HTTP."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Opzioni di trasferimento file"
>abstract="Opzioni di trasferimento file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Attività Estrarre file"
>abstract="Attività Estrarre file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Trasferimento file su server remoto"
>abstract="Specificare il server da connettere."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Trasferimento origine file"
>abstract="Trasferimento origine file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Elimina i file di origine dopo il trasferimento"
>abstract="Cancella i file di origine dopo un trasferimento riuscito."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Visualizzare i registri di sessione"
>abstract="Le informazioni relative all’operazione di trasferimento vengono visualizzate nei registri del flusso di lavoro."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Elenca tutti i file"
>abstract="Questa opzione indicizza tutti i file presenti sul server in **vars.filenames** variabile evento."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Storicizzazione del file"
>abstract="Storicizzazione del file"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Elabora file mancanti"
>abstract="Questa opzione ti consente di attivare una transizione in uscita &quot;No file&quot; dopo l’attività."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Errori del processo"
>abstract="Questa opzione consente di attivare una transizione in uscita di tipo &quot;Errore&quot; dopo l’attività."

Il **Trasferisci file** l&#39;attività è un **Gestione dati** attività. Consente di ricevere o inviare file, verificare la presenza di file o elencarli su un server. Il protocollo utilizzato può essere un protocollo da server a server o HTTP.

>[!NOTE]
>
>Con l’interfaccia utente di Campaign Web, abbiamo consolidato due attività in una unendo entrambe **Trasferimento file** e **Download web** funzionalità. Questo consolidamento non influisce in alcun modo sulla funzionalità dell’attività.

Segui i passaggi descritti di seguito per configurare **Trasferisci file** attività.

## Scegliere il protocollo e l&#39;operazione di trasferimento {#protocol}

1. Aggiungi un **Trasferisci file** attività nel flusso di lavoro, quindi specifica il tipo di trasferimento da eseguire a seconda del protocollo che desideri utilizzare:

   * Per il protocollo HTTP, seleziona **[!UICONTROL Download Web]**. Questo consente di eseguire il download di un file GET o POST su un URL esplicito, un account esterno o un’istanza di Adobe Campaign.
   * Per altri protocolli server-to-server e azioni correlate, selezionare **[!UICONTROL Trasferimento file]**.

1. Seleziona l’azione da eseguire con l’attività. Le azioni disponibili dipendono dal tipo di trasferimento selezionato. Per ulteriori informazioni, espandi le sezioni seguenti.

   +++Azioni disponibili con **Trasferimento file** attività di tipo

   * **[!UICONTROL Download dei file]**: scarica un file dal server.
   * **[!UICONTROL Caricamento di file]**: carica un file sul server.
   * **[!UICONTROL Test per verificare se il file esiste]**: controlla se un determinato file è presente sul server. Genera due transizioni in uscita dopo l’attività: &quot;Il file esiste&quot; e &quot;Il file non esiste&quot;.
   * **[!UICONTROL Elenco dei file]**: elenca tutti i file disponibili sul server.

+++

   +++Azioni disponibili con **Download web** attività di tipo

   * **[!UICONTROL Trasferimento semplice (GET)]**: recupera un file.
   * **[!UICONTROL Trasferimento tramite un modulo (POST)]**: carica un file e parametri aggiuntivi.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. Per impostazione predefinita, per le azioni di caricamento file, l’attività utilizza il file specificato nell’attività precedente. Per utilizzare un file diverso, attiva/disattiva **[!UICONTROL Usa file da attività precedente]** e fare clic sul pulsante **[!UICONTROL Aggiungi file]** pulsante.

   In **[!UICONTROL Sorgente]** immettere il nome di file desiderato oppure utilizzare l&#39;editor di espressioni per calcolare il nome di file utilizzando le variabili evento. [Scopri come utilizzare le variabili evento e l’editor di espressioni](../event-variables.md). Ripetere l&#39;operazione per aggiungere tutti i file necessari.

## Definire la destinazione del trasferimento {#destination}

1. In **[!UICONTROL Server remoto]** , specificare il server da connettere utilizzando uno dei seguenti metodi:

   * **[!UICONTROL Utilizzare i parametri di connessione definiti in un account esterno]**: connettiti a un server utilizzando i parametri di connessione di un account esterno. In **[!UICONTROL Cartella server]** , specificare il percorso del file (o della cartella per l&#39;elenco delle azioni).
   * **[!UICONTROL Configurazione rapida]**: immetti l’URL del file (o della cartella per le azioni di elenco dei file).
   * **[!UICONTROL istanza Adobe Campaign]** (attività di tipo download web): scarica un file da un server di istanze di Adobe Campaign.

   ![](../assets/workflow-transfer-file-server.png)

1. Per le azioni POST di download web, con l’operazione puoi trasmettere parametri aggiuntivi. A questo scopo, fai clic su **[!UICONTROL Aggiungi parametro]** quindi specificare il nome e il valore dei parametri. Puoi aggiungere tutti i parametri necessari.

1. Per impostazione predefinita, per il caricamento di file, i file caricati su un server vengono salvati automaticamente. Se non desideri conservare questa cronologia, attiva/disattiva la **[!UICONTROL Mantieni la cronologia dei file inviati]** opzione disattivata.

## Impostazioni di storicizzazione {#historization}

Ogni volta che **[!UICONTROL Trasferisci file]** Quando l&#39;attività viene eseguita, i file caricati o scaricati vengono memorizzati in una cartella dedicata. Viene creata una cartella per ogni attività Transfer file di un flusso di lavoro. Per impostazione predefinita, i file vengono salvati nella directory di archiviazione predefinita della cartella di installazione di Adobe Campaign (`/vars`) prima dell&#39;elaborazione. Per utilizzare una cartella specifica, attiva/disattiva **[!UICONTROL Utilizza una directory di archiviazione predefinita]** disattivata e immettete il percorso della directory.

![](../assets/workflow-transfer-file-historization.png)

È importante essere in grado di limitare le dimensioni di questa cartella per preservare lo spazio fisico sul server. A questo scopo, puoi definire un numero massimo di file o una dimensione totale per la cartella dell’attività. Per impostazione predefinita sono autorizzati 100 file e 50 MB.

Tutte le volte che l’attività viene eseguita, la cartella viene controllata come segue:

* Vengono presi in considerazione solo file creati più di 24 ore prima dell’esecuzione dell’attività.
* Se il numero di file considerati è maggiore del valore del **[!UICONTROL Numero di file]** , i file meno recenti vengono eliminati finché non viene raggiunto il numero massimo di file consentiti.
* Se la dimensione totale dei file considerati è maggiore del valore del **[!UICONTROL Dimensione massima (in MB)]** , i file meno recenti vengono eliminati finché non viene raggiunta la dimensione massima (in MB) consentita.

>[!CAUTION]
>
>Se l’attività non viene eseguita nuovamente, la relativa cartella non viene né controllata né eliminata. In quest’ottica, fai attenzione durante il trasferimento di file di grandi dimensioni.

## Opzioni avanzate e di gestione degli errori {#advanced}

1. In **[!UICONTROL Opzioni avanzate]**, sono disponibili opzioni aggiuntive in base al tipo di attività che si sta configurando. Per ulteriori informazioni, espandi le sezioni seguenti.

   +++Opzioni aggiuntive per **[!UICONTROL Trasferimento file]** attività di tipo

   * **[!UICONTROL Elimina i file di origine dopo il trasferimento]**: cancella i file sorgente dopo un trasferimento riuscito.
   * **[!UICONTROL Visualizzare i registri di sessione]**: quando questa opzione viene attivata, le informazioni relative all’operazione di trasferimento vengono visualizzate nei registri del flusso di lavoro una volta eseguito il flusso di lavoro.
   * **[!UICONTROL Elenca tutti i file]** (azioni di elenco file): questa opzione indicizza tutti i file presenti sul server in `vars.filenames` variabile di evento, in cui i nomi dei file sono separati da `n` caratteri. [Scopri come utilizzare le variabili evento](../event-variables.md)

+++

   +++Opzioni aggiuntive per **[!UICONTROL Download web]** attività di tipo

   * **[!UICONTROL Segui i reindirizzamenti]**: il reindirizzamento dei file consente di utilizzare gli override per indirizzare l’input o l’output di dati a un dispositivo di tipo diverso.
   * **[!UICONTROL Aggiungi le intestazioni HTTP al file]**: in alcuni casi, potrebbe essere utile aggiungere ulteriori intestazioni HTTP a un file. Nella maggior parte dei casi, queste intestazioni vengono utilizzate per fornire informazioni aggiuntive a scopo di risoluzione dei problemi, per [Condivisione delle risorse tra diverse origini (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS), o per impostare specifiche direttive di caching.
   * **[!UICONTROL Ignora il codice di ritorno HTTP]**: i codici di ritorno HTTP, o codici di stato HTTP, indicano il risultato di una richiesta HTTP.

1. Il **[!UICONTROL Errori di processo]** consente di attivare una transizione in uscita &quot;Error&quot; dopo l’attività, se si verifica un errore durante il trasferimento.

   Inoltre, per **Trasferimento file** attività di tipo, il **[!UICONTROL Elabora file mancante]** L’opzione ti consente di attivare una transizione in uscita &quot;No file&quot; dopo l’attività, se il file non è disponibile nel percorso specificato.
