---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Riconciliazione
description: Scopri come utilizzare l’attività del flusso di lavoro Riconciliazione
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 40%

---

# Riconciliazione {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Attività di riconciliazione"
>abstract="L’attività di **riconciliazione** è un’attività di **targeting** che consente di definire il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro. Ad esempio, l’attività di **riconciliazione** può essere inserita dopo un’attività **Carica file** per importare dati non standard nel database. In questo caso, l’attività di **riconciliazione** definisce il collegamento tra i dati nel database di Adobe Campaign e i dati nella tabella esterna."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Campo di selezione riconciliazione"
>abstract="Campo di selezione riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condizione di creazione riconciliazione"
>abstract="Condizione di creazione riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Complemento generato da riconciliazione"
>abstract="Complemento generato da riconciliazione"

L&#39;attività **Reconciliation** è un&#39;attività **Targeting** che definisce il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro, ad esempio i dati caricati da un file esterno.

Ad esempio, l’attività di **riconciliazione** può essere inserita dopo un’attività **Carica file** per importare dati non standard nel database. In questo caso, l&#39;attività **Reconciliation** definisce il collegamento tra i dati nel database di Adobe Campaign e i dati nella tabella di lavoro.

## Best practice {#reconciliation-best-practices}

Mentre l&#39;attività **Enrichment** definisce i dati aggiuntivi da elaborare nel flusso di lavoro (ad esempio, la combinazione di dati da più set o la creazione di collegamenti a una risorsa temporanea), l&#39;attività **Reconciliation** collega i dati non identificati alle risorse esistenti.

>[!NOTE]
>Le operazioni di riconciliazione richiedono che i dati delle dimensioni collegate siano già presenti nel database. Ad esempio, se importi un file di acquisti che mostra quale prodotto è stato acquistato in un determinato momento e da quale client, il prodotto e il client devono già esistere nel database.

## Configurare l’attività di riconciliazione {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensione targeting"
>abstract="Seleziona la nuova dimensione targeting. Una dimensione consente di definire la popolazione target: destinatari, abbonati all’app, operatori, iscritti, ecc. Per impostazione predefinita, è selezionata la dimensione targeting corrente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regole di riconciliazione"
>abstract="Seleziona le regole di riconciliazione per la deduplica. Per utilizzare gli attributi, seleziona l’opzione **Attributi semplici** e scegli i campi di origine e di destinazione. Per creare una condizione di riconciliazione personalizzata utilizzando query modeler, seleziona l’opzione **Condizioni di riconciliazione avanzate**."
>additional-url="https://experienceleague.adobe.com/it/docs/campaign-web/v8/query-database/query-modeler-overview" text="Utilizzo del query modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Selezionare una dimensione targeting"
>abstract="Seleziona la dimensione targeting per i dati in entrata per cui eseguire la riconciliazione."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=it#targeting-dimensions" text="Dimensioni di targeting"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Mantenere i dati non riconciliati"
>abstract="Per impostazione predefinita, i dati non riconciliati vengono conservati nella transizione in uscita e sono disponibili nella tabella di lavoro per utilizzi futuri. Per rimuovere i dati non riconciliati, disattiva l’opzione **Mantieni i dati non riconciliati**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Attributo di riconciliazione"
>abstract="Seleziona l’attributo da utilizzare per riconciliare i dati e fai clic su Conferma."

Per configurare l&#39;attività **Reconciliation**, eseguire la procedura seguente:

1. Aggiungi un&#39;attività **Reconciliation** al flusso di lavoro. Questa attività deve seguire una transizione contenente un gruppo la cui dimensione di targeting non proviene direttamente da Adobe Campaign.

1. Seleziona la nuova dimensione targeting. Una dimensione consente di definire la popolazione target: destinatari, abbonati all’app, operatori, iscritti, ecc. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions).

1. Seleziona i campi da utilizzare per la riconciliazione. Puoi utilizzare uno o più criteri di riconciliazione.

   1. Per utilizzare gli attributi per riconciliare i dati, selezionare l&#39;opzione **Attributi semplici**. Nel campo **Source** sono elencati i campi disponibili nella transizione di input che devono essere riconciliati. Il campo **Destinazione** corrisponde ai campi della dimensione di targeting selezionata. I dati vengono riconciliati quando l’origine e la destinazione sono uguali. Ad esempio, seleziona i campi **E-mail** per deduplicare i profili in base al loro indirizzo e-mail.

      Per aggiungere un altro criterio di riconciliazione, fare clic sul pulsante **Aggiungi regola**. Se sono specificate più condizioni di unione, è necessario verificarle tutte affinché i dati siano collegati tra loro.

      ![Esempio di criteri di riconciliazione](../assets/workflow-reconciliation-criteria.png)

   1. Per utilizzare altri attributi per riconciliare i dati, selezionare l&#39;opzione **Condizioni di riconciliazione avanzate**. Puoi quindi creare una condizione di riconciliazione personalizzata utilizzando Query Modeler. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md).

1. Filtra i dati da riconciliare utilizzando il pulsante **Crea filtro**. Questo consente di creare una condizione personalizzata utilizzando il modellatore di query. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md).

Per impostazione predefinita, i dati non riconciliati vengono conservati nella transizione in uscita e sono disponibili nella tabella di lavoro per utilizzi futuri. Per rimuovere i dati non riconciliati, disattiva l’opzione **Mantieni i dati non riconciliati**.

## Esempio {#reconciliation-example}

L’esempio seguente illustra un flusso di lavoro che crea un pubblico di profili direttamente da un file importato contenente nuovi clienti. Include le seguenti attività:

Il flusso di lavoro è progettato come segue:

![Esempio di flusso di lavoro](../assets/workflow-reconciliation-sample-1.0.png)

Viene generato con le seguenti attività:

* Un&#39;attività [Load file](load-file.md) carica un file contenente dati di profilo estratti da uno strumento esterno.

  Ad esempio:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Un&#39;attività **Reconciliation** identifica i dati in arrivo come profili utilizzando i campi **E-mail** e **Data di nascita** come criteri di riconciliazione.

  ![Esempio di attività Reconciliation](../assets/workflow-reconciliation-sample-1.1.png)

* Un&#39;attività [Save audience](save-audience.md) crea un nuovo pubblico in base a questi aggiornamenti. È inoltre possibile sostituire l&#39;attività **Salva pubblico** con un&#39;attività **Fine** se non è necessario creare o aggiornare un pubblico specifico. I profili dei destinatari vengono aggiornati in ogni caso quando esegui il flusso di lavoro.

## Compatibilità {#reconciliation-compat}

L&#39;attività **Reconciliation** non esiste nella console client. Tutte le attività **Enrichment** create nella console client con le opzioni di riconciliazione abilitate vengono visualizzate come attività **Reconciliation** nell&#39;interfaccia utente Web di Campaign.