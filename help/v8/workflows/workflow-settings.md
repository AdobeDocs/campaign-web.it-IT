---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 63%

---

# Configurare le impostazioni avanzate del flusso di lavoro {#workflow-settings}

Durante l’orchestrazione delle attività del flusso di lavoro nell’area di lavoro, puoi accedere alle impostazioni avanzate relative al flusso di lavoro. Ad esempio, puoi impostare un fuso orario specifico per il flusso di lavoro, gestire il comportamento del flusso di lavoro in caso di errore o gestire il ritardo dopo il quale la cronologia del flusso di lavoro deve essere eliminata.

A questo scopo, fai clic su **[!UICONTROL Impostazioni del flusso di lavoro]** nell’angolo in alto a sinistra dell’area di lavoro, accanto all’etichetta del flusso di lavoro.

![](assets/workflow-settings.png)

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="TBD"

La sezione delle proprietà del flusso di lavoro fornisce proprietà generiche accessibili anche durante la creazione del flusso di lavoro.

* **[!UICONTROL Etichetta]**: l’etichetta del flusso di lavoro che viene visualizzata nell’elenco.
* **[!UICONTROL Nome interno]**: nome interno del flusso di lavoro.
* **[!UICONTROL Cartella]**: cartella in cui deve essere salvato il flusso di lavoro.
* **[!UICONTROL Campagna collegata]**: questo campo viene visualizzato se il flusso di lavoro è stato creato all’interno di una campagna. Ti consente di aprire la campagna associata.
* **[!UICONTROL Fuso orario]**: definisci un fuso orario specifico da utilizzare per impostazione predefinita in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
* **[!UICONTROL Supervisore]**: quando un flusso di lavoro è in errore, gli operatori appartenenti al gruppo di supervisione del flusso di lavoro ricevono una notifica via e-mail, purché il loro indirizzo e-mail sia elencato nel profilo.
* **[!UICONTROL Descrizione]**: utilizza questo campo per fornire una descrizione del flusso di lavoro.

## Impostazioni di segmentazione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="TBD"

* **[!UICONTROL Dimensione targeting]**: seleziona la dimensione di targeting da utilizzare per eseguire il targeting dei profili: destinatari, beneficiari del contratto, operatore, abbonati, ecc.
* **[!UICONTROL Mantieni il risultato delle popolazioni provvisorie tra due esecuzioni]**: per impostazione predefinita, vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate da un flusso di lavoro tecnico che viene eseguito su base giornaliera.

   Se questa opzione è abilitata, le tabelle di lavoro verranno mantenute anche dopo l’esecuzione del flusso di lavoro. Puoi utilizzarlo a scopo di test e quindi deve essere utilizzato solo in ambienti di sviluppo o di staging. Non deve mai essere sottoposto a check-in in un flusso di lavoro di produzione,

## Impostazioni di esecuzione del flusso di lavoro

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Impostazioni di esecuzione"
>abstract="TBD"

* Cronologia in giorni: le tabelle di lavoro del database conservano una cronologia delle esecuzioni (attività, eventi, registro). Qui puoi definire il numero di giorni da archiviare per questo flusso di lavoro: il processo di pulizia eliminerà gli archivi più vecchi una volta al giorno. Se il valore in questo campo è zero, l’archivio non verrà mai eliminato.

   Specifica il numero di giorni dopo i quali la cronologia deve essere eliminata. La cronologia contiene gli elementi relativi al flusso di lavoro: registri, attività, eventi (oggetti tecnici collegati all’operazione del flusso di lavoro), nonché file scaricati dall’attività **[!UICONTROL Trasferisci file]**. Per i modelli di flusso di lavoro preconfigurati, il valore predefinito è 30 giorni.

   L’eliminazione della cronologia viene eseguita dal flusso di lavoro tecnico per la pulizia del database, che viene eseguito quotidianamente per impostazione predefinita

   >[!IMPORTANT]
   >
   >Se il campo della **[!UICONTROL Cronologia in giorni]** è lasciato vuoto, il suo valore sarà considerato come “1”, il che significa che la cronologia verrà eliminata dopo 1 giorno.

* Affinità predefinita: questo campo consente di forzare l’esecuzione di un flusso di lavoro o di un’attività del flusso di lavoro su un determinato computer.   Se l’installazione include diversi server per il flusso di lavoro, utilizza questo campo per scegliere il computer su cui verrà eseguito il flusso di lavoro. Se il valore definito in questo campo non esiste su alcun server, il flusso di lavoro rimarrà in sospeso.

* Salva le query SQL nel registro: consente di salvare le query SQL dal flusso di lavoro nei registri. (dove è possibile accedere ai registri sql?)

   Questa funzionalità è riservata agli utenti avanzati. Riguarda i flussi di lavoro che contengono attività di targeting (query, unione, intersezione, ecc.). Quando questa opzione è selezionata, le query SQL inviate al database durante l’esecuzione del flusso di lavoro vengono visualizzate in Adobe Campaign: potrai quindi analizzarle per ottimizzare le query o diagnosticare eventuali problemi.

   Le query vengono visualizzate nella scheda **[!UICONTROL Registri SQL]**, che viene aggiunta al flusso di lavoro (ad eccezione dei flussi di lavoro della campagna) e all’attività **[!UICONTROL Proprietà]** quando l’opzione è abilitata. La scheda **[!UICONTROL Audit]** include anche le query SQL.

## Impostazioni di gestione degli errori

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Impostazioni di gestione degli errori"
>abstract="TBD"

* Questo campo consente di definire le azioni da eseguire in caso di errori in un’attività del flusso di lavoro. Sono disponibili due opzioni possibili:

   Interrompi il processo: il flusso di lavoro viene messo in pausa automaticamente. Lo stato del flusso di lavoro diventa Non riuscito. Una volta risolto il problema, riavvia il flusso di lavoro utilizzando i pulsanti Avvia o Riavvia.

   Ignora: lo stato dell’attività che ha attivato l’errore diventa Non riuscito, ma il flusso di lavoro mantiene lo stato Avviato. Questa configurazione è pertinente per le attività ricorrenti: se il ramo include un modulo di pianificazione, si avvia normalmente alla successiva esecuzione del flusso di lavoro.

* Errori consecutivi: questo campo diventa disponibile quando il valore Ignora è selezionato nel campo In caso di errori. È possibile specificare il numero di errori che possono essere ignorati prima dell’arresto del processo. Una volta raggiunto questo numero, lo stato del flusso di lavoro diventa Non riuscito. Se il valore di questo campo è 0, il flusso di lavoro non verrà mai interrotto indipendentemente dal numero di errori.
