---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Riconciliazione
description: Scopri come utilizzare l’attività del flusso di lavoro Riconciliazione
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 44%

---

# Riconciliazione {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Attività di riconciliazione"
>abstract="L’attività di **riconciliazione** è un’attività di **targeting** che consente di definire il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro. Ad esempio, l’attività di **riconciliazione** può essere inserita dopo un’attività **Carica file** per importare dati non standard nel database. In questo caso, l’attività di **riconciliazione** consente di definire il collegamento tra i dati nel database di Adobe Campaign e i dati nella tabella esterna."

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

Il **Reconciliation** l&#39;attività è un **Targeting** attività che ti consente di definire il collegamento tra i dati nel database di Adobe Campaign e i dati in una tabella di lavoro, ad esempio i dati caricati da un file esterno.

Ad esempio, l’attività di **riconciliazione** può essere inserita dopo un’attività **Carica file** per importare dati non standard nel database. In questo caso, il **Reconciliation** attività consente di definire il collegamento tra i dati nel database di Adobe Campaign e i dati nella tabella di lavoro.

## Best practice {#reconciliation-best-practices}

Mentre il **Arricchimento** attività ti consente di definire i dati aggiuntivi da elaborare nel flusso di lavoro (puoi utilizzare un’ **Arricchimento** attività (per combinare dati provenienti da più set o per creare collegamenti a una risorsa temporanea), **Reconciliation** L’attività ti consente di collegare dati non identificati a risorse esistenti.

>[!NOTE]
>L&#39;operazione Reconciliation implica che i dati delle dimensioni collegate siano già presenti nel database.  Ad esempio, se importi un file di acquisti che mostra quale prodotto è stato acquistato in un determinato momento da uno specifico cliente, ecc., il prodotto e il cliente devono già esistere nel database.

## Configurare l’attività di riconciliazione {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensione targeting"
>abstract="Seleziona la nuova dimensione targeting. Una dimensione consente di definire la popolazione target: destinatari, abbonati all’app, operatori, iscritti, ecc. Per impostazione predefinita, è selezionata la dimensione targeting corrente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regole di riconciliazione"
>abstract="Seleziona le regole di riconciliazione da utilizzare per la deduplica. Per utilizzare gli attributi, seleziona l’opzione **Attributi semplici** e scegli i campi di origine e di destinazione. Per creare una condizione di riconciliazione personalizzata utilizzando query modeler, seleziona l’opzione **Condizioni di riconciliazione avanzate**."
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

Per configurare il **Reconciliation** attività:

1. Trascina una **Reconciliation** attività nel flusso di lavoro. Questa attività deve essere aggiunta dopo una transizione contenente un gruppo la cui dimensione di targeting non proviene direttamente da Adobe Campaign.

1. Seleziona la nuova dimensione targeting. Una dimensione consente di definire la popolazione target: destinatari, abbonati all’app, operatori, iscritti, ecc. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions).

1. Seleziona i campi da utilizzare per la riconciliazione. Puoi utilizzare uno o più criteri di riconciliazione.

   1. Per utilizzare gli attributi per riconciliare i dati, selezionare **Attributi semplici** opzione. Il **Sorgente** campo elenca i campi disponibili nella transizione di input, che devono essere riconciliati. Il **Destinazione** corrisponde ai campi della dimensione di targeting selezionata. I dati vengono riconciliati quando l’origine e la destinazione sono uguali. Ad esempio, seleziona la **E-mail** per deduplicare i profili in base al loro indirizzo e-mail.

      Per aggiungere un altro criterio di riconciliazione, fai clic su **Aggiungi regola** pulsante. Se sono specificate più condizioni di unione, è necessario verificarle TUTTE in modo che i dati possano essere collegati tra loro.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Per utilizzare altri attributi per riconciliare i dati, selezionare **Condizioni di riconciliazione avanzate** opzione. Puoi quindi creare una condizione di riconciliazione personalizzata utilizzando Query Modeler. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md).

1. È possibile filtrare i dati da riconciliare utilizzando **Crea filtro** pulsante. Questo consente di creare una condizione personalizzata utilizzando il modellatore di query. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

Per impostazione predefinita, i dati non riconciliati vengono conservati nella transizione in uscita e sono disponibili nella tabella di lavoro per utilizzi futuri. Per rimuovere i dati non riconciliati, disattiva l’opzione **Mantieni i dati non riconciliati**.

## Esempio {#reconciliation-example}

L’esempio seguente illustra un flusso di lavoro che crea un pubblico di profili direttamente da un file importato contenente nuovi clienti. È costituito dalle seguenti attività:

Il flusso di lavoro è progettato come segue:

![](../assets/workflow-reconciliation-sample-1.0.png)


Viene generato con le seguenti attività:

* L’attività [Load file](load-file.md) carica un file contenente i dati di profili estratti da uno strumento esterno.

  Ad esempio:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **Reconciliation** attività che identifica i dati in arrivo come profili, utilizzando **email** e **Data di nascita** come criteri di riconciliazione.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [Salva pubblico](save-audience.md) per creare un nuovo pubblico in base a questi aggiornamenti. È inoltre possibile sostituire il **Salva pubblico** attività di un **Fine** attività se non è necessario creare o aggiornare un pubblico specifico. I profili dei destinatari vengono aggiornati in ogni caso quando esegui il flusso di lavoro.


## Compatibilità {#reconciliation-compat}

Il **Reconciliation** L&#39;attività non esiste nella console Client. Tutti **Arricchimenti** Le attività create nella console client con le opzioni di riconciliazione abilitate vengono visualizzate come **Reconciliation** attività nell’interfaccia utente di Campaign Web.
