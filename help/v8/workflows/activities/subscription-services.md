---
audience: end-user
title: Utilizzare l’attività Subscription services
description: Scopri come utilizzare l’attività del flusso di lavoro Subscription services
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 13%

---

# Servizi di abbonamento {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Attività dei servizi di abbonamento"
>abstract="L’attività Subscription services consente a più profili di effettuare o annullare l’abbonamento a un servizio in un’unica azione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parametri generali del servizio di abbonamento"
>abstract="Scegli il servizio desiderato e scegli l’azione da eseguire (abbonamento o annullamento dell’abbonamento). Attiva **Invia messaggio di conferma** opzione su per notificare alla popolazione l’abbonamento o l’annullamento dell’abbonamento al servizio selezionato."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Genera una transizione in uscita"
>abstract="Attiva/disattiva l’opzione **Genera una transizione in uscita** per aggiungere una transizione dopo l’attività."

Il **Servizi di abbonamento** l&#39;attività è un **Gestione dati** attività. Consente di creare o eliminare un abbonamento a un servizio di informazioni per la popolazione specificata nella transizione.

## Configurare l’attività Subscription services {#subscription-services-configuration}

Per configurare il **Servizi di abbonamento** attività:

1. Aggiungi un **Servizi di abbonamento** attività nel flusso di lavoro. Puoi utilizzare questa attività dopo il targeting dei profili o l’importazione di un file con dati identificati.

1. Seleziona il servizio per il quale desideri gestire gli abbonamenti utilizzando una delle seguenti opzioni:

   * **[!UICONTROL Seleziona un servizio specifico]**: seleziona manualmente un servizio utilizzando **[!UICONTROL Servizio]** campo.

   * **[!UICONTROL Da transizione in entrata]**: utilizza il servizio specificato nella transizione in entrata. Ad esempio, puoi importare un file che specifica il servizio da gestire per ogni riga. Il servizio su cui eseguire l’operazione viene quindi selezionato dinamicamente per ciascun profilo.

   ![](../assets/workflow-subscription-service.png)

1. Selezionare l&#39;operazione da eseguire: **Abbonati** o **Annulla iscrizione**.

   Se il servizio è definito nella transizione in entrata, puoi scegliere come recuperare questa operazione:

   * **Seleziona un tipo di operazione specifico**: seleziona manualmente l’operazione da eseguire (**Abbonati** o **Annulla iscrizione**)

   * **Seleziona un tipo di operazione da un percorso di transizione in entrata**: seleziona la colonna dei dati in entrata che specifica l’operazione da eseguire per ogni record. Ad esempio, è possibile importare un file che specifica l&#39;operazione da eseguire per ogni riga di una colonna &quot;operazione&quot;.

     >[!NOTE]
     >
     >Qui è possibile selezionare solo campi booleani o interi. Assicurati che i dati contenenti l’operazione da eseguire corrispondano a questo formato. Ad esempio, se carichi i dati da un’attività Load file, verifica di aver impostato correttamente il formato della colonna contenente l’operazione nell’ **[!UICONTROL Carica file]** attività. Un esempio è presentato in [questa sezione](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Per notificare ai destinatari l’abbonamento o il suo annullamento al servizio selezionato, attiva/disattiva **[!UICONTROL Invia un messaggio di conferma]** opzione attivata. Il contenuto di questa notifica è definito in un modello di consegna associato al servizio informazioni.

1. Se utilizzi dati da una transizione in entrata, un’ **[!UICONTROL Informazioni aggiuntive]** viene visualizzata la sezione, che consente di specificare i dati e l’origine dell’abbonamento per ciascun record. Puoi lasciare vuota questa sezione, nel qual caso non verrà impostata alcuna data o origine durante l’esecuzione del flusso di lavoro.

   * Se i dati in entrata contengono una colonna che indica la data di abbonamento del profilo al servizio, puoi selezionarla in **[!UICONTROL Data]** campo.

   * In **[!UICONTROL Percorso origine]** , definisci l’origine dell’abbonamento. Puoi impostarlo su uno dei campi dei dati in entrata o su un valore costante desiderato selezionando la **[!UICONTROL Imposta una costante come origine]** opzione.

   ![](../assets/workflow-subscription-service-additional.png)

1. Per aggiungere una transizione in uscita dopo l’attività, imposta il **[!UICONTROL Generare una transizione in uscita]** opzione attivata.

## Esempi {#example}

### Iscrizione di un pubblico a un servizio specifico {#uc1}

Questo flusso di lavoro seguente mostra come abbonare un pubblico a un servizio esistente.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Creare un pubblico]** l’attività esegue il targeting di un pubblico esistente.

* A **[!UICONTROL Subscription Services]** attività ti consente di selezionare il servizio a cui i profili devono effettuare l’abbonamento.

### Aggiornamento di più stati di abbonamento da un file {#uc2}

Il flusso di lavoro seguente mostra come importare un file contenente profili e aggiornarne l’abbonamento a diversi servizi specificati nel file.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Carica file]** L’attività carica un file CSV contenente i dati e definisce la struttura delle colonne importate. Le colonne &quot;servizio&quot; e &quot;operazione&quot; specificano il servizio da aggiornare e l’operazione da eseguire (abbonamento o annullamento dell’abbonamento).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Come avrai notato, l’operazione è specificata nel file come &quot;sub&quot; o &quot;non sub&quot;. Il sistema richiede un **valore booleano** o un **numero intero** per riconoscere l’operazione da eseguire: &quot;0&quot; per annullare l’abbonamento e &quot;1&quot; per effettuare l’abbonamento. Per soddisfare questo requisito, è necessario eseguire una nuova mappatura dei valori nei dettagli della colonna &quot;operazione&quot; nella schermata di configurazione del file di esempio.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Se il file utilizza già &quot;0&quot; e &quot;1&quot; per identificare l’operazione, non devi ripetere la mappatura di tali valori. Assicurati solo che la colonna venga elaborata come **Booleano** o **Intero** nelle colonne del file di esempio.

* A **[!UICONTROL Reconciliation]** l’attività identifica i dati del file come appartenenti alla dimensione di profilo del database di Adobe Campaign. Il **email** del file corrisponde al campo **email** della risorsa profilo.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* Un **[!UICONTROL Arricchimento]** l’attività crea un collegamento alla tabella &quot;Services (nms)&quot; e un semplice join tra la colonna &quot;service&quot; del file caricato e il campo &quot;internal name&quot; dei servizi nel database.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplicazione]** in base al **email** Questo campo identifica i duplicati. È importante eliminare i duplicati poiché l’abbonamento a un servizio non riuscirà per tutti i dati in caso di duplicati.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* A **[!UICONTROL Subscription Services]** identifica i servizi da aggiornare come provenienti dalla transizione, attraverso il collegamento creato in **[!UICONTROL Reconciliation]** attività.

  Il **[!UICONTROL Tipo di operazione]** è identificato come proveniente da **operazione** del file. Qui è possibile selezionare solo campi con un valore booleano o un numero intero. Se la colonna del file che contiene l&#39;operazione da eseguire non viene visualizzata nell&#39;elenco, verificare di aver impostato correttamente il formato della colonna nel **[!UICONTROL Carica file]** come spiegato in precedenza in questo esempio.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
