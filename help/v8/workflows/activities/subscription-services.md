---
audience: end-user
title: Utilizzare l’attività Subscription services
description: Scopri come utilizzare l’attività del flusso di lavoro Subscription services
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 24%

---

# Servizi di iscrizione {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Attività Servizi di iscrizione"
>abstract="L’attività Servizi di iscrizione consente a più profili di effettuare l’iscrizione a un servizio o annullarla in un’unica azione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parametri generali dei servizi di iscrizione"
>abstract="Scegli il servizio desiderato e scegli l’azione da eseguire (iscrizione o annullamento dell’iscrizione). Attiva l’opzione **Invia messaggio di conferma** per inviare una notifica sull’iscrizione o sull’annullamento dell’iscrizione al servizio selezionato alla popolazione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Genera una transizione in uscita"
>abstract="Attiva o disattiva l’opzione **Genera una transizione in uscita** per aggiungere una transizione dopo l’attività."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Informazioni aggiuntive"
>abstract="Specifica i dati e l’origine dell’iscrizione per ciascun record. Puoi lasciare vuota questa sezione, nel qual caso non verrà impostata alcuna data o origine durante l’esecuzione del flusso di lavoro. Se i dati in entrata contengono una colonna che indica la data di iscrizione del profilo al servizio, puoi selezionarla nel campo **[!UICONTROL Data]**. Nel campo **[!UICONTROL Percorso origine]**, definisci l’origine dell’iscrizione. Puoi impostarla su uno dei campi dei dati in entrata o su un valore costante desiderato selezionando l’opzione **[!UICONTROL Imposta una costante come origine]**."

L&#39;attività **Subscription services** è un&#39;attività **Data Management**. Consente di creare o eliminare un abbonamento a un servizio di informazioni per la popolazione specificata nella transizione.

## Configurare l’attività Subscription services {#subscription-services-configuration}

Segui questi passaggi per configurare l&#39;attività **Subscription services**:

1. Aggiungi un&#39;attività **Subscription services** al flusso di lavoro. Puoi utilizzare questa attività dopo il targeting dei profili o l’importazione di un file con dati identificati.

1. Seleziona il servizio per il quale desideri gestire gli abbonamenti utilizzando una delle seguenti opzioni:

   * **[!UICONTROL Seleziona un servizio specifico]**: seleziona manualmente un servizio utilizzando il campo **[!UICONTROL Servizio]**.

   * **[!UICONTROL Da transizione in entrata]**: utilizzare il servizio specificato nella transizione in entrata. Ad esempio, puoi importare un file che specifica il servizio da gestire per ogni riga. Il servizio su cui eseguire l’operazione viene quindi selezionato dinamicamente per ciascun profilo.

   ![Schermata dell&#39;interfaccia del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service.png)

1. Selezionare l&#39;operazione da eseguire: **Sottoscrivi** o **Annulla sottoscrizione**.

   Se il servizio è definito nella transizione in entrata, scegliere come recuperare questa operazione:

   * **Selezionare un tipo di operazione specifico**: selezionare manualmente l&#39;operazione da eseguire (**Sottoscrivi** o **Annulla sottoscrizione**).

   * **Selezionare un tipo di operazione da un percorso di transizione in entrata**: selezionare la colonna dei dati in entrata che specifica l&#39;operazione da eseguire per ogni record. Ad esempio, è possibile importare un file che specifica l&#39;operazione da eseguire per ogni riga di una colonna &quot;operazione&quot;.

     Qui è possibile selezionare solo campi booleani o interi. Assicurati che i dati contenenti l’operazione da eseguire corrispondano a questo formato. Ad esempio, se carichi dati da un&#39;attività Load file, verifica di aver impostato correttamente il formato della colonna contenente l&#39;operazione nell&#39;attività **[!UICONTROL Load file]**. Un esempio è presentato in [questa sezione](#uc2).

     >[!CAUTION]
     >
     >Per impostazione predefinita, se si seleziona questa opzione, l&#39;attività **Subscription services** prevede di avere una definizione di collegamento alla tabella **Services (nms)** impostata nel flusso di lavoro. A questo scopo, assicurati di aver configurato un collegamento di riconciliazione in un&#39;attività di **arricchimento** precedente nel flusso di lavoro. Un esempio che mostra come utilizzare questa opzione è disponibile [qui](#uc2).

   ![Schermata dell&#39;interfaccia in entrata del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service-inbound.png)

1. Per notificare ai destinatari l&#39;abbonamento o l&#39;annullamento dell&#39;abbonamento al servizio selezionato, attivare l&#39;opzione **[!UICONTROL Invia un messaggio di conferma]**. Il contenuto di questa notifica è definito in un modello di consegna associato al servizio informazioni.

1. Se utilizzi dati da una transizione in entrata, viene visualizzata una sezione **[!UICONTROL Ulteriori informazioni]** che ti consente di specificare i dati e l&#39;origine della sottoscrizione per ogni record. Puoi lasciare vuota questa sezione, nel qual caso non verrà impostata alcuna data o origine durante l’esecuzione del flusso di lavoro.

   * Se i dati in entrata contengono una colonna che indica la data di abbonamento del profilo al servizio, puoi selezionarla nel campo **[!UICONTROL Data]**.

   * Nel campo **[!UICONTROL Percorso origine]**, definisci l’origine dell’iscrizione. Puoi impostarla su uno dei campi dei dati in entrata o su un valore costante desiderato selezionando l’opzione **[!UICONTROL Imposta una costante come origine]**.

   ![Schermata dell&#39;interfaccia delle informazioni aggiuntive del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service-additional.png)

1. Per aggiungere una transizione in uscita dopo l&#39;attività, attivare l&#39;opzione **[!UICONTROL Genera una transizione in uscita]**.

## Esempi {#example}

### Iscrizione di un pubblico a un servizio specifico {#uc1}

Questo flusso di lavoro seguente mostra come abbonare un pubblico a un servizio esistente.

![Schermata del flusso di lavoro per l&#39;abbonamento di un pubblico a un servizio specifico.](../assets/workflow-subscription-service-uc1.png)

* Un&#39;attività **[!UICONTROL Build audience]** esegue il targeting di un pubblico esistente.

* Un&#39;attività **[!UICONTROL Subscription Services]** consente di selezionare il servizio a cui i profili devono essere abbonati.

### Aggiornamento di più stati di abbonamento da un file {#uc2}

Il flusso di lavoro seguente mostra come importare un file contenente profili e aggiornarne l’abbonamento a diversi servizi specificati nel file.

![Schermata del flusso di lavoro che aggiorna più stati di abbonamento da un file.](../assets/workflow-subscription-service-uc2.png)

* Un&#39;attività **[!UICONTROL Load file]** carica un file CSV contenente i dati e definisce la struttura delle colonne importate. Le colonne &quot;servizio&quot; e &quot;operazione&quot; specificano il servizio da aggiornare e l’operazione da eseguire (abbonamento o annullamento dell’abbonamento).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Come avrai notato, l’operazione è specificata nel file come &quot;sub&quot; o &quot;unsub&quot;. Il sistema richiede un **valore booleano** o un **numero intero** per riconoscere l’operazione da eseguire: &quot;0&quot; per annullare l’abbonamento e &quot;1&quot; per effettuare l’abbonamento. Per soddisfare questo requisito:
   * Il **tipo di dati** per la colonna &quot;operazione&quot; è impostato su un numero intero.
   * È necessario eseguire una **Modifica del valore** per far corrispondere i valori &quot;sub&quot; e &quot;unsub&quot; con i valori &quot;1&quot; e &quot;0&quot;.

  ![Schermata dell&#39;interfaccia di mappatura del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service-uc2-mapping.png)

  Se il file utilizza già &quot;0&quot; e &quot;1&quot; per identificare l’operazione, non devi ripetere la mappatura di tali valori. Assicurati solo che la colonna sia elaborata come **Boolean** o **Integer** nelle colonne del file di esempio.

* Un&#39;attività **[!UICONTROL Reconciliation]** identifica i dati del file come appartenenti alla dimensione di profilo del database di Adobe Campaign. Il campo **email** del file corrisponde al campo **email** della risorsa profilo.

  ![Schermata dell&#39;interfaccia di riconciliazione del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service-uc2-reconciliation.png)

* Un&#39;attività **[!UICONTROL Enrichment]** crea un collegamento di riconciliazione alla tabella &quot;Services (nms)&quot;, con un semplice join tra la colonna &quot;service&quot; del file caricato e il campo &quot;internal name&quot; dei servizi nel database.

  ![Schermata dell&#39;interfaccia di arricchimento del servizio di abbonamento al flusso di lavoro.](../assets/workflow-subscription-service-uc2-enrichment.png)

* Un **[!UICONTROL Subscription Services]** identifica i servizi da aggiornare come provenienti dalla transizione.

  Il tipo di operazione **** è identificato come proveniente dal campo **operation** del file. Qui è possibile selezionare solo campi con un valore booleano o un numero intero. Se la colonna del file che contiene l&#39;operazione da eseguire non viene visualizzata nell&#39;elenco, verificare di aver impostato correttamente il formato della colonna nell&#39;attività **[!UICONTROL Carica file]**, come spiegato in precedenza in questo esempio.

  ![Schermata dell&#39;interfaccia di sottoscrizione del servizio di sottoscrizione del flusso di lavoro.](../assets/workflow-subscription-service-uc2-subscription.png)