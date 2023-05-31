---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 696fa6192c16f8fd1d2dd77ad533203277f8a2dd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configurare le impostazioni del flusso di lavoro {#workflow-settings}

contenuto da definire

Definisci le impostazioni disponibili dal pulsante nell’area di lavoro del flusso di lavoro
<!--à reformuler-->

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="TBD"

(= come per la creazione del flusso di lavoro? da controllare)

* Etichetta
* Opzioni aggiuntive
* Nome interno
* Cartella
* Campagna collegata > può essere modificata. In tal caso, il flusso di lavoro scompare dalla campagna corrente e viene visualizzato nella nuova campagna collegata

   Quando crei un flusso di lavoro all’interno di una campagna, troverai un campo Campagna aggiuntivo, che ti consente di identificare e accedere facilmente alla campagna associata al flusso di lavoro.

* Ad esempio, puoi definire un fuso orario specifico da utilizzare per impostazione predefinita in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
* Supervisore: quando un flusso di lavoro genera un errore, gli operatori appartenenti al gruppo di supervisione del flusso di lavoro ricevono una notifica tramite e-mail, purché il loro indirizzo e-mail sia elencato nel loro profilo. Questo gruppo è selezionato nel campo **[!UICONTROL Supevisore(i)]** delle proprietà del flusso di lavoro.
* descrizione

## Impostazioni di segmentazione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="TBD"

* Dimensione targeting:

   Durante le operazioni di segmentazione dei dati, la chiave di targeting è mappata su una dimensione filtro. La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati, ecc. La dimensione filtro consente di selezionare la popolazione in base a determinati criteri: titolari di contratti, abbonati a newsletter, ecc.

* Mantenere i risultati: l’opzione **Mantieni il risultato delle popolazioni provvisorie tra due esecuzioni** consente di mantenere tabelle temporanee tra due esecuzioni di un flusso di lavoro.  È disponibile nella scheda delle proprietà del flusso di lavoro **[!UICONTROL Generale]** e può essere utilizzata a scopo di sviluppo e test per monitorare i dati e controllare i risultati. Puoi utilizzare questa opzione negli ambienti di sviluppo ma mai negli ambienti di produzione. Mantenere tabelle temporanee potrebbe comportare un aumento significativo delle dimensioni del database e, in ultima analisi, il raggiungimento del limite consentito. Inoltre, rallenterà il backup.

   Vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate dal flusso di lavoro di **[!UICONTROL pulizia]**, che viene eseguito su base giornaliera.

   >[!CAUTION]
   >
   >Questa opzione non deve **mai** essere selezionata in un flusso di lavoro di **produzione**. Viene utilizzata per analizzare i risultati ed è progettata solo a scopo di test e quindi deve essere utilizzata solo in ambienti di sviluppo o di staging.

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
