---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Aggiorna dati
description: Scopri come utilizzare l’attività del flusso di lavoro Aggiorna dati
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 18%

---

# Aggiornare i dati {#update-data}

Il **Aggiorna dati** l&#39;attività è un **Gestione dati** attività. Consente di eseguire un aggiornamento di massa sui campi del database. Diverse opzioni consentono di personalizzare l’aggiornamento dei dati.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Configurare l’attività Update data{#update-data-configuration}

Per configurare **Aggiorna dati** attività, inizia aggiungendo l’attività al flusso di lavoro e definisci un’etichetta.

![](../assets/workflow-update-data.png)

### Tipo di operazione

Il **Tipo di operazione** consente di scegliere il processo da eseguire sui dati del database:

* **Inserisci o aggiorna**: inserire dati o aggiornarli, se i record sono già presenti nel database.
* **Inserisci**: inserire solo i dati. I record già esistenti non vengono aggiornati. Se vengono definiti i criteri di riconciliazione, verranno aggiunti solo i record non riconciliati.
* **Aggiorna**: aggiorna i dati dei record già presenti solo nel database.
* **Elimina**: elimina i dati.

Il **Dimensione batch** Questo campo consente di selezionare il numero di elementi di transizione in entrata da aggiornare. Se ad esempio si specifica 500, verranno aggiornati i primi 500 record trattati.

### Identificazione record

Questa sezione consente di specificare come identificare i record nel database:

* Se le voci di dati si riferiscono a una dimensione di targeting esistente, seleziona la **Utilizzo della dimensione di targeting** e selezionarla da nel **Dimensione targeting da aggiornare** campo.
* È inoltre possibile selezionare **Utilizzo di collegamenti personalizzati** e specificare uno o più collegamenti che consentano l&#39;identificazione dei dati nel database
* Se il tipo di operazione selezionato richiede un aggiornamento, è necessario utilizzare **Utilizzo delle regole di riconciliazione** opzione.

### Campi da aggiornare

In **Campi da aggiornare** , aggiungi i campi in cui verrà applicato l’aggiornamento e, se necessario, aggiungi le condizioni per l’esecuzione. A tale scopo, utilizza **Considerato se** campo. Le condizioni vengono applicate in sequenza, secondo l’ordine dell’elenco. Utilizza le frecce a destra per cambiare l’ordine degli aggiornamenti. Puoi usare più volte lo stesso campo di destinazione.

Puoi collegare automaticamente i campi utilizzando **Mappatura automatica** pulsante. Il collegamento automatico rileva i campi con il medesimo nome.

Durante un **Inserisci o aggiorna** tipo di operazione, puoi selezionare singolarmente l’operazione da applicare a ciascun campo. A questo scopo, seleziona il valore desiderato nella **Tipo di operazione** campo.

### Opzioni avanzate

Il **Opzioni avanzate** consente di specificare opzioni aggiuntive per l’aggiornamento dei dati e la gestione dei duplicati.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Le ultime due opzioni consentono di eseguire azioni specifiche:

* **Generare una transizione in uscita**: crea una transizione in uscita che verrà attivata alla fine dell’esecuzione. L’aggiornamento in genere segnala la fine di un flusso di lavoro di targeting e l’opzione non viene quindi attivata per impostazione predefinita.

* **Genera una transizione in uscita per i rifiuti**: crea una transizione in uscita contenente record che non sono stati elaborati correttamente dopo l’aggiornamento (ad esempio se è presente un duplicato). L’aggiornamento in genere segna la fine di un flusso di lavoro di targeting e pertanto l’opzione non è attivata per impostazione predefinita.
