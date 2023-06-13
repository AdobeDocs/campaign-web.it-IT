---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 17%

---

# Configurare le impostazioni del flusso di lavoro {#workflow-settings}

Durante l’orchestrazione delle attività del flusso di lavoro nell’area di lavoro, puoi accedere alle impostazioni avanzate relative al flusso di lavoro. Ad esempio, puoi impostare un fuso orario specifico per il flusso di lavoro, gestire il comportamento del flusso di lavoro in caso di errore o gestire il ritardo dopo il quale la cronologia del flusso di lavoro deve essere eliminata.

Queste impostazioni sono preconfigurate nel modello selezionato durante la creazione del flusso di lavoro, ma possono essere modificate in base alle esigenze per questo flusso di lavoro specifico.

A questo scopo, fai clic su **[!UICONTROL Impostazioni del flusso di lavoro]** nell’angolo in alto a sinistra dell’area di lavoro, accanto all’etichetta del flusso di lavoro.

![](assets/workflow-settings.png)

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="In questa sezione vengono fornite proprietà di flusso di lavoro generiche accessibili anche durante la creazione del flusso di lavoro. Puoi scegliere il modello da utilizzare per creare il flusso di lavoro e specificare un’etichetta. Espandi la sezione Opzioni aggiuntive per configurare impostazioni specifiche, ad esempio la cartella di archiviazione del flusso di lavoro o il fuso orario."

Il **[!UICONTROL Proprietà]** fornisce impostazioni generiche accessibili anche durante la creazione del flusso di lavoro.

* **[!UICONTROL Etichetta]**: l’etichetta del flusso di lavoro che viene visualizzata nell’elenco.
* **[!UICONTROL Nome]**: nome interno del flusso di lavoro.
* **[!UICONTROL Cartella]**: cartella in cui deve essere salvato il flusso di lavoro.
* **[!UICONTROL Campagna collegata]**: questo campo viene visualizzato se il flusso di lavoro è stato creato all’interno di una campagna. Ti consente di aprire la campagna associata.
* **[!UICONTROL Fuso orario]**: definisci un fuso orario specifico da utilizzare per impostazione predefinita in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
* **[!UICONTROL Supervisori]**: quando un flusso di lavoro è in errore, gli operatori appartenenti al gruppo di supervisione del flusso di lavoro ricevono una notifica via e-mail, purché il loro indirizzo e-mail sia elencato nel profilo.
* **[!UICONTROL Descrizione]**: utilizza questo campo per fornire una descrizione del flusso di lavoro.

## Impostazioni di segmentazione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="In questa sezione, puoi selezionare la dimensione di targeting per eseguire il targeting dei profili nel flusso di lavoro e scegliere di mantenere i risultati del flusso di lavoro tra due esecuzioni. Questa opzione deve essere utilizzata solo a scopo di test e non deve mai essere abilitata in un flusso di lavoro di produzione."

* **[!UICONTROL Dimensione targeting]**: seleziona la dimensione di targeting da utilizzare per eseguire il targeting dei profili: destinatari, beneficiari del contratto, operatore, abbonati, ecc.
* **[!UICONTROL Mantieni il risultato delle popolazioni provvisorie tra due esecuzioni]**: per impostazione predefinita, vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate da un flusso di lavoro tecnico che viene eseguito su base giornaliera.

  Se questa opzione è abilitata, le tabelle di lavoro verranno mantenute anche dopo l’esecuzione del flusso di lavoro. Puoi utilizzarlo a scopo di test e quindi deve essere utilizzato solo in ambienti di sviluppo o di staging. Non deve mai essere archiviato in un flusso di lavoro di produzione.

## Impostazioni di esecuzione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Impostazioni di esecuzione"
>abstract="In questa sezione puoi configurare le impostazioni relative all’esecuzione del flusso di lavoro, ad esempio il numero di giorni in cui viene mantenuta la cronologia del flusso di lavoro."

* **[!UICONTROL Cronologia in giorni]**: specifica quanti giorni devono trascorrere prima che la cronologia venga eliminata. La cronologia contiene elementi correlati al flusso di lavoro: registri, attività, eventi (oggetti tecnici collegati all’operazione del flusso di lavoro). Per i modelli di flusso di lavoro preconfigurati, il valore predefinito è 30 giorni. L’eliminazione della cronologia viene eseguita dal flusso di lavoro tecnico per la pulizia del database, che viene eseguito quotidianamente per impostazione predefinita

  >[!IMPORTANT]
  >
  >Se il campo della **[!UICONTROL Cronologia in giorni]** è lasciato vuoto, il suo valore sarà considerato come “1”, il che significa che la cronologia verrà eliminata dopo 1 giorno.

* **[!UICONTROL Affinità predefinita]**: se l’installazione include diversi server del flusso di lavoro, utilizza questo campo per scegliere il computer in cui verrà eseguito il flusso di lavoro. Se il valore definito in questo campo non esiste in alcun server, il flusso di lavoro rimarrà in sospeso.

* **[!UICONTROL Salvare le query SQL nel registro]**: consente di salvare le query SQL dal flusso di lavoro nei registri. Questa funzionalità è riservata agli utenti avanzati. Si applica ai flussi di lavoro che contengono attività di targeting come **[!UICONTROL Creare un pubblico]**. Quando questa opzione è abilitata, le query SQL inviate al database durante l&#39;esecuzione del flusso di lavoro vengono visualizzate nei registri del flusso di lavoro, consentendo di analizzarle per ottimizzare le query o diagnosticare i problemi.

## Impostazioni di gestione degli errori

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Impostazioni di gestione degli errori"
>abstract="In questa sezione puoi gestire il comportamento del flusso di lavoro quando si verifica un errore durante l’esecuzione (sospendine/interrompine l’esecuzione o ignora gli errori)."

* **[!UICONTROL Gestione degli errori]**: questo campo ti consente di definire le azioni da intraprendere in caso di errori in un’attività del flusso di lavoro. Sono disponibili due opzioni possibili:

   * **[!UICONTROL Sospendi il processo]**: il flusso di lavoro viene messo automaticamente in pausa e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riprendere il flusso di lavoro utilizzando **[!UICONTROL Riprendi]** pulsanti.
   * **[!UICONTROL Ignora]**: lo stato dell’attività che ha attivato l’errore cambia in **[!UICONTROL Non riuscito]**, ma il flusso di lavoro mantiene **[!UICONTROL Avviato]** stato. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Interrompi il processo]**: il flusso di lavoro viene arrestato automaticamente e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riavvia il flusso di lavoro utilizzando **[!UICONTROL Inizio]** pulsanti.

* **[!UICONTROL Errori consecutivi]**: questo campo diventa disponibile quando **[!UICONTROL Ignora]** è selezionato in **[!UICONTROL In caso di errori]** campo. È possibile specificare il numero di errori che possono essere ignorati prima dell’arresto del processo. Una volta raggiunto questo numero, lo stato del flusso di lavoro cambia in **[!UICONTROL Non riuscito]**. Se il valore di questo campo è 0, il flusso di lavoro non verrà mai interrotto indipendentemente dal numero di errori.
