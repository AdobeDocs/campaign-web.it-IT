---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 7%

---

# Configurare le impostazioni del flusso di lavoro {#workflow-settings}

contenuto TBD

definire le impostazioni disponibili dal pulsante nell’area di lavoro del flusso di lavoro
<!--à reformuler-->

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="TBD"

(= come per la creazione del flusso di lavoro ? da controllare)

* Etichetta
* Opzioni aggiuntive
* Nome interno
* Cartella
* Campagna collegata > può modificarla. In tal caso, il flusso di lavoro scompare dalla campagna corrente e viene visualizzato nel nuovo flusso di lavoro collegato
* Fuso orario: definisci un fuso orario specifico da utilizzare per impostazione predefinita in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
* Supervisore: Quando un flusso di lavoro è errato, gli operatori appartenenti al gruppo di supervisione del flusso di lavoro ricevono una notifica tramite e-mail, purché il loro indirizzo e-mail sia elencato nel loro profilo. Questo gruppo è selezionato nella **[!UICONTROL Garante(i)]** campo delle proprietà del flusso di lavoro.
* descrizione

## Impostazioni di segmentazione

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="TBD"

* dimensione di targeting:

   Durante le operazioni di segmentazione dei dati, la chiave di targeting è mappata su una dimensione di filtro. La dimensione di targeting ti consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati, ecc. La dimensione di filtro consente di selezionare la popolazione in base a determinati criteri: titolari di contratti, abbonati a newsletter, ecc.

* mantieni risultati: La **Mantenere il risultato delle popolazioni intermedie tra due esecuzioni** consente di mantenere tabelle temporanee tra due esecuzioni di un flusso di lavoro.  È disponibile nelle proprietà del flusso di lavoro **[!UICONTROL Generale]** e può essere utilizzato a scopo di sviluppo e test per monitorare i dati e controllare i risultati. Puoi utilizzare questa opzione negli ambienti di sviluppo ma non mai negli ambienti di produzione. Mantenere tabelle temporanee potrebbe comportare un aumento significativo delle dimensioni del database e, in ultima analisi, il raggiungimento del limite di dimensione. Inoltre, rallenterà il backup.

   Vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate dal **[!UICONTROL pulizia]** , che viene eseguito su base giornaliera.

   >[!CAUTION]
   >
   >Questa opzione deve essere **mai** essere controllati in un **produzione** workflow. Questa opzione viene utilizzata per analizzare i risultati ed è progettata solo a scopo di test e quindi deve essere utilizzata solo negli ambienti di sviluppo o di staging.

## Impostazioni di esecuzione del flusso di lavoro

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Impostazioni di esecuzione"
>abstract="TBD"

* Storia in giorni: Le tabelle di lavoro del database conservano una cronologia delle esecuzioni (attività, eventi, log). Qui puoi definire il numero di giorni da archiviare per questo flusso di lavoro: il processo di pulizia eliminerà gli archivi più vecchi una volta al giorno. Se il valore in questo campo è zero, l’archivio non verrà mai eliminato.

   specifica il numero di giorni dopo i quali la cronologia deve essere eliminata. La cronologia contiene gli elementi relativi al flusso di lavoro: registri, attività, eventi (oggetti tecnici collegati all’operazione del flusso di lavoro), nonché file scaricati dal **[!UICONTROL Transfer file]** attività. Il valore predefinito è 30 giorni per i modelli di flusso di lavoro predefiniti.

   L&#39;eliminazione della cronologia viene eseguita dal flusso di lavoro tecnico Database cleanup , che viene eseguito quotidianamente per impostazione predefinita

   >[!IMPORTANT]
   >
   >Se la **[!UICONTROL Storia nei giorni]** Il campo è lasciato vuoto, il suo valore sarà considerato come &quot;1&quot;, il che significa che la cronologia verrà eliminata dopo 1 giorno.

* affinità predefinita: questo campo ti consente di forzare l’esecuzione di un flusso di lavoro o di un’attività del flusso di lavoro su un determinato computer.   Se l’installazione include diversi server del flusso di lavoro, utilizza questo campo per scegliere il computer su cui verrà eseguito il flusso di lavoro. Se il valore definito in questo campo non esiste su alcun server, il flusso di lavoro rimarrà in sospeso.

* salva query sql nel registro: consente di salvare le query SQL dal flusso di lavoro nei registri. (dove accedere ai log sql?)

   Questa funzionalità è riservata agli utenti avanzati. Riguarda flussi di lavoro che contengono attività di targeting (query, unione, intersezione, ecc.). Quando questa opzione è selezionata, le query SQL inviate al database durante l’esecuzione del flusso di lavoro vengono visualizzate in Adobe Campaign: questo significa che puoi analizzarli per ottimizzare le query o diagnosticare i problemi.

   Le query vengono visualizzate in un **[!UICONTROL Registri SQL]** , che viene aggiunta al flusso di lavoro (ad eccezione dei flussi di lavoro della campagna) e al **[!UICONTROL Proprietà]** quando l’opzione è abilitata. La **[!UICONTROL Audit]** La scheda include anche le query SQL.

## Impostazioni di gestione degli errori

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Impostazioni di gestione degli errori"
>abstract="TBD"

* Questo campo ti consente di definire le azioni da eseguire in caso di errori in un’attività del flusso di lavoro. Sono disponibili due opzioni possibili:

   Interrompi il processo: il flusso di lavoro viene messo in pausa automaticamente. lo stato del flusso di lavoro diventa Non riuscito. Una volta risolto il problema, riavvia il flusso di lavoro utilizzando i pulsanti Start o Restart.

   Ignora: lo stato dell&#39;attività che ha attivato l&#39;errore diventa Non riuscito, ma il flusso di lavoro mantiene lo stato Avviato . Questa configurazione è pertinente per le attività ricorrenti: se il ramo include una pianificazione, si avvia normalmente alla successiva esecuzione del flusso di lavoro.

* Errori consecutivi: Questo campo diventa disponibile quando il valore Ignora è selezionato nel campo In caso di errori. È possibile specificare il numero di errori che possono essere ignorati prima dell&#39;arresto del processo. Una volta raggiunto questo numero, lo stato del flusso di lavoro diventa Non riuscito. Se il valore di questo campo è 0, il flusso di lavoro non verrà mai interrotto indipendentemente dal numero di errori.
