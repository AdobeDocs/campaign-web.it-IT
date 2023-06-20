---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 99%

---

# Configurare le impostazioni del flusso di lavoro {#workflow-settings}

Durante l’orchestrazione delle attività del flusso di lavoro nell’area di lavoro, puoi accedere alle impostazioni avanzate relative al flusso di lavoro. Ad esempio, puoi impostare un fuso orario specifico per il flusso di lavoro, gestirne il comportamento in caso di errore oppure gestire il ritardo dopo il quale la cronologia del flusso di lavoro deve essere eliminata.

Queste impostazioni sono preconfigurate nel modello selezionato durante la creazione del flusso di lavoro, ma possono essere modificate in base alle esigenze per il flusso di lavoro specifico.

A questo scopo, fai clic sull’icona **[!UICONTROL Impostazioni del flusso di lavoro]** nell’angolo in alto a sinistra dell’area di lavoro, accanto all’etichetta del flusso di lavoro.

![](assets/workflow-settings.png)

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="In questa sezione sono illustrate le proprietà generiche del flusso di lavoro accessibili anche durante la relativa creazione. Puoi scegliere il modello da utilizzare per creare il flusso di lavoro e specificare un’etichetta. Espandi la sezione Opzioni aggiuntive per configurare impostazioni specifiche, ad esempio la cartella di archiviazione del flusso di lavoro o il fuso orario."

La sezione **[!UICONTROL Proprietà]** offre impostazioni generiche accessibili anche durante la creazione del flusso di lavoro.

* **[!UICONTROL Etichetta]**: l’etichetta del flusso di lavoro che viene visualizzata nell’elenco.
* **[!UICONTROL Nome]**: il nome interno del flusso di lavoro.
* **[!UICONTROL Cartella]**: la cartella in cui deve essere salvato il flusso di lavoro.
* **[!UICONTROL Campagna collegata]**: questo campo viene visualizzato se il flusso di lavoro è stato creato all’interno di una campagna. Ti consente di aprire la campagna associata.
* **[!UICONTROL Fuso orario]**: definisci un fuso orario specifico da utilizzare per impostazione predefinita in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
* **[!UICONTROL Supervisore/i]**: quando un flusso di lavoro genera un errore, gli operatori appartenenti al gruppo di supervisione del flusso di lavoro ricevono una notifica tramite e-mail, purché il loro indirizzo e-mail sia elencato nel loro profilo.
* **[!UICONTROL Descrizione]**: utilizza questo campo per fornire una descrizione del flusso di lavoro.

## Impostazioni di segmentazione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="In questa sezione, puoi selezionare la dimensione di targeting per eseguire il targeting dei profili nel flusso di lavoro e scegliere di mantenere i risultati del flusso di lavoro tra due esecuzioni. Questa opzione deve essere utilizzata solo a scopo di test e non deve mai essere abilitata in un flusso di lavoro di produzione."

* **[!UICONTROL Dimensione targeting]**: seleziona la dimensione di targeting da utilizzare per eseguire il targeting dei profili, tra cui destinatari, beneficiari del contratto, operatore, abbonati, ecc.
* **[!UICONTROL Mantieni il risultato delle popolazioni provvisorie tra due esecuzioni]**: per impostazione predefinita, vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate dal flusso di lavoro di pulizia, che viene eseguito su base giornaliera.

  Se questa opzione è abilitata, le tabelle di lavoro verranno mantenute anche dopo l’esecuzione del flusso di lavoro. Puoi utilizzarlo a scopo di test e quindi solo in ambienti di sviluppo o di staging. Questa opzione non deve mai essere selezionata in un flusso di lavoro di produzione.

## Impostazioni di esecuzione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Impostazioni di esecuzione"
>abstract="In questa sezione, puoi configurare le impostazioni relative all’esecuzione del flusso di lavoro, ad esempio il numero di giorni in cui viene mantenuta la cronologia del flusso di lavoro."

* **[!UICONTROL Cronologia in giorni]**: specifica il numero di giorni dopo i quali la cronologia deve essere eliminata. La cronologia contiene elementi correlati al flusso di lavoro: registri, attività, eventi (oggetti tecnici collegati all’operazione del flusso di lavoro). Per i modelli di flusso di lavoro preconfigurati, il valore predefinito è 30 giorni. L’eliminazione della cronologia viene eseguita dal flusso di lavoro tecnico per la pulizia del database, che viene eseguito quotidianamente per impostazione predefinita

  >[!IMPORTANT]
  >
  >Se il campo della **[!UICONTROL Cronologia in giorni]** è lasciato vuoto, il suo valore sarà considerato come “1”, il che significa che la cronologia verrà eliminata dopo 1 giorno.

* **[!UICONTROL Affinità predefinita]**: se l’installazione include diversi server per il flusso di lavoro, utilizza questo campo per scegliere il computer su cui verrà eseguito il flusso di lavoro. Se il valore definito in questo campo non esiste su alcun server, il flusso di lavoro rimarrà in sospeso.

* **[!UICONTROL Salva le query SQL nel registro]**: consente di salvare le query SQL dal flusso di lavoro nei registri. Questa funzionalità è riservata agli utenti avanzati. Si applica ai flussi di lavoro che contengono attività di targeting come **[!UICONTROL Creazione del pubblico]**. Quando questa opzione è selezionata, le query SQL inviate al database durante l’esecuzione del flusso di lavoro vengono visualizzate nei registri del flusso di lavoro, consentendoti di analizzarle per ottimizzare le query o diagnosticare eventuali problemi.

## Impostazioni di gestione degli errori

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Impostazioni di gestione degli errori"
>abstract="In questa sezione, puoi gestire il comportamento del flusso di lavoro quando si verifica un errore durante l’esecuzione (sospendi/interrompi l’esecuzione o ignora gli errori)."

* **[!UICONTROL Gestione degli errori]**: questo campo consente di definire le azioni da eseguire in caso di errori in un’attività del flusso di lavoro. Sono disponibili due opzioni possibili:

   * **[!UICONTROL Sospendi il processo]**: il flusso di lavoro viene messo automaticamente in pausa e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riprendi il flusso di lavoro utilizzando il pulsante **[!UICONTROL Riprendi]**.
   * **[!UICONTROL Ignora]**: lo stato dell’attività che ha attivato l’errore diventa **[!UICONTROL Non riuscito]**, ma il flusso di lavoro mantiene lo stato **[!UICONTROL Avviato]**.<!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Interrompi il processo]**: il flusso di lavoro viene interrotto automaticamente e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riavvia il flusso di lavoro utilizzando il pulsante **[!UICONTROL Avvia]**.

* **[!UICONTROL Errori consecutivi]**: questo campo diventa disponibile quando il valore **[!UICONTROL Ignora]** è selezionato nel campo **[!UICONTROL In caso di errori]**. È possibile specificare il numero di errori che possono essere ignorati prima dell’interruzione del processo. Una volta raggiunto questo numero, lo stato del flusso di lavoro diventa **[!UICONTROL Non riuscito]**. Se il valore di questo campo è 0, il flusso di lavoro non verrà mai interrotto indipendentemente dal numero di errori.
