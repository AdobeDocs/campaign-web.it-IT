---
audience: end-user
title: Configurare le impostazioni del flusso di lavoro
description: Scopri come configurare le impostazioni del flusso di lavoro con Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 0250ab3bd05023bddbf3a0104631cc7bb40acadc
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 69%

---


# Configurare le impostazioni del flusso di lavoro {#workflow-settings}


>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Proprietà del flusso di lavoro"
>abstract="In questa schermata, scegli il modello da utilizzare per creare il flusso di lavoro e specifica un’etichetta. Espandi **Opzioni aggiuntive** per configurare altre impostazioni, ad esempio il nome interno del flusso di lavoro, la cartella, il fuso orario e il gruppo di supervisori. Si consiglia vivamente di selezionare un gruppo di supervisori in modo che gli operatori vengano avvisati in caso di errore."

Durante la creazione di un flusso di lavoro o l’orchestrazione delle attività del flusso di lavoro nell’area di lavoro, puoi accedere alle impostazioni avanzate relative al flusso di lavoro. Ad esempio, puoi impostare un fuso orario specifico per il flusso di lavoro, gestirne il comportamento in caso di errore oppure gestire il ritardo dopo il quale la cronologia del flusso di lavoro deve essere eliminata.

Queste impostazioni sono preconfigurate nel modello selezionato durante la creazione del flusso di lavoro, ma possono essere modificate in base alle esigenze per il flusso di lavoro specifico.


![](assets/workflow-settings-button.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

## Proprietà del flusso di lavoro {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Proprietà del flusso di lavoro"
>abstract="In questa sezione sono illustrate le proprietà generiche del flusso di lavoro accessibili anche durante la relativa creazione. Puoi scegliere il modello da utilizzare per creare il flusso di lavoro e specificare un’etichetta. Espandi la sezione Opzioni aggiuntive per configurare impostazioni specifiche, ad esempio la cartella di archiviazione del flusso di lavoro o il fuso orario."

Il **[!UICONTROL Proprietà]** fornisce impostazioni generiche che possono essere configurate durante la creazione di un flusso di lavoro. Per accedere alle proprietà di un flusso di lavoro esistente, fai clic su **[!UICONTROL Impostazioni]** disponibile nella barra delle azioni sopra l’area di lavoro del flusso di lavoro.


![](assets/workflow-settings.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}


Queste proprietà sono:

* Il **[!UICONTROL Etichetta]** del flusso di lavoro visualizzato nell’elenco.
* Il **[!UICONTROL Nome interno]** del workflow.
* Il **[!UICONTROL Cartella]** dove salvare il flusso di lavoro.
* Il valore predefinito **[!UICONTROL Fuso orario]** da utilizzare in tutte le attività del flusso di lavoro. Per impostazione predefinita, il fuso orario del flusso di lavoro è quello definito per l’operatore corrente di Campaign.
I valori possibili sono:
   * **Fuso orario del server** per utilizzare il fuso orario del server dell’applicazione Adobe Campaign
   * **Fuso orario dell’operatore** per utilizzare il fuso orario dell’operatore di Adobe Campaign che esegue il flusso di lavoro, come definito nel profilo dell’operatore, nella console client
   * **Fuso orario del database** per utilizzare il fuso orario del server del database
   * Un fuso orario specifico
* Quando un flusso di lavoro non riesce, gli operatori appartenenti al gruppo di operatori selezionato nel **[!UICONTROL Supervisori]** vengono notificati tramite e-mail.
* È inoltre possibile immettere un **[!UICONTROL Descrizione]** del workflow.

Quando il flusso di lavoro è [associato a una campagna](create-workflow.md), viene visualizzato nel **[!UICONTROL Campagna collegata]** campo. Puoi aprire la campagna associata da quel campo.


## Impostazioni di segmentazione  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Impostazioni di segmentazione"
>abstract="In questa sezione, puoi selezionare la dimensione di targeting per eseguire il targeting dei profili nel flusso di lavoro e scegliere di mantenere i risultati del flusso di lavoro tra due esecuzioni. Questa opzione deve essere utilizzata solo a scopo di test e non deve mai essere abilitata in un flusso di lavoro di produzione."

* **[!UICONTROL Dimensione targeting]**: seleziona la dimensione di targeting da utilizzare per eseguire il targeting dei profili: destinatari, beneficiari del contratto, operatore, abbonati, ecc. [Ulteriori informazioni sulle dimensioni di targeting](../audience/targeting-dimensions.md)

* **[!UICONTROL Mantieni il risultato delle popolazioni provvisorie tra due esecuzioni]**: per impostazione predefinita, vengono mantenute solo le tabelle di lavoro dell’ultima esecuzione del flusso di lavoro. Le tabelle di lavoro delle esecuzioni precedenti vengono eliminate dal flusso di lavoro di pulizia, che viene eseguito su base giornaliera.

  Se questa opzione è abilitata, le tabelle di lavoro verranno mantenute anche dopo l’esecuzione del flusso di lavoro. Puoi utilizzarlo a scopo di test e quindi deve essere utilizzato **solo** in ambienti di sviluppo o di staging. Questa opzione non deve mai essere selezionata in un flusso di lavoro di produzione.

## Impostazioni di esecuzione  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Impostazioni di esecuzione"
>abstract="In questa sezione, puoi configurare le impostazioni relative all’esecuzione del flusso di lavoro, ad esempio il numero di giorni in cui viene mantenuta la cronologia del flusso di lavoro."

* **[!UICONTROL Cronologia in giorni]**: specifica il numero di giorni dopo i quali la cronologia deve essere eliminata. La cronologia contiene elementi correlati al flusso di lavoro: registri, attività, eventi (oggetti tecnici collegati all’operazione del flusso di lavoro). Per i modelli di flusso di lavoro preconfigurati, il valore predefinito è 30 giorni. L’eliminazione della cronologia viene eseguita dal flusso di lavoro tecnico per la pulizia del database, che viene eseguito quotidianamente per impostazione predefinita

  >[!IMPORTANT]
  >
  >Se il campo della **[!UICONTROL Cronologia in giorni]** è lasciato vuoto, il suo valore sarà considerato come “1”, il che significa che la cronologia verrà eliminata dopo 1 giorno.

* **[!UICONTROL Affinità predefinita]**: se l’installazione include diversi server del flusso di lavoro, utilizza questo campo per specificare il server su cui verrà eseguito il flusso di lavoro. Questo forza l’esecuzione di quel flusso di lavoro su un server particolare. Puoi scegliere un nome di affinità esistente, ma assicurati di non utilizzare spazi o segni di punteggiatura. Se si utilizzano server diversi, specificare nomi diversi, separati da virgole.

  >[!IMPORTANT]
  >
  >Se il valore definito in questo campo non esiste su alcun server, il flusso di lavoro rimarrà in sospeso.


* **[!UICONTROL Salvare le query SQL nel registro]**: seleziona questa opzione per salvare le query SQL dal flusso di lavoro nei registri. Questa funzionalità è riservata agli utenti avanzati. Si applica ai flussi di lavoro che contengono attività di targeting come **[!UICONTROL Creazione del pubblico]**. Quando questa opzione è selezionata, le query SQL inviate al database durante l’esecuzione del flusso di lavoro vengono visualizzate nei registri del flusso di lavoro, consentendoti di analizzarle per ottimizzare le query o diagnosticare eventuali problemi.

## Impostazioni di gestione degli errori  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Impostazioni di gestione degli errori"
>abstract="In questa sezione puoi definire come il flusso di lavoro deve gestire gli errori durante l’esecuzione. Puoi scegliere di sospendere il processo, ignorare un certo numero di errori o interrompere l’esecuzione del flusso di lavoro."

* **[!UICONTROL Gestione degli errori]**: questo campo consente di definire le azioni da eseguire in caso di errori in un’attività del flusso di lavoro. Sono disponibili tre opzioni:

   * **[!UICONTROL Sospendi il processo]**: il flusso di lavoro viene messo automaticamente in pausa e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riprendi il flusso di lavoro utilizzando il pulsante **[!UICONTROL Riprendi]**.
   * **[!UICONTROL Ignora]**: lo stato dell’attività che ha attivato l’errore diventa **[!UICONTROL Non riuscito]**, ma il flusso di lavoro mantiene lo stato **[!UICONTROL Avviato]**.<!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Interrompi il processo]**: il flusso di lavoro viene interrotto automaticamente e il suo stato cambia in **[!UICONTROL Non riuscito]**. Una volta risolto il problema, riavvia il flusso di lavoro utilizzando il pulsante **[!UICONTROL Avvia]**.

* **[!UICONTROL Errori consecutivi]**: questo campo diventa disponibile quando il valore **[!UICONTROL Ignora]** è selezionato nel campo **[!UICONTROL In caso di errori]**. È possibile specificare il numero di errori che possono essere ignorati prima dell’interruzione del processo. Una volta raggiunto questo numero, lo stato del flusso di lavoro diventa **[!UICONTROL Non riuscito]**. Se il valore di questo campo è 0, il flusso di lavoro non verrà mai interrotto indipendentemente dal numero di errori.
