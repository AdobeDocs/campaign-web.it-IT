---
title: Creare e pubblicare schemi
description: Scopri come creare, estendere e pubblicare schemi.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Creare e pubblicare schemi {#create-publish}

## Creare e gestire gli schemi {#create-schemas}

È possibile creare nuovi schemi, estendere gli schemi esistenti e accedere a database esterni.

### Creare o estendere uno schema {#create-new}

Per creare o estendere uno schema:

1. Passa a **[!UICONTROL Amministrazione]** > **[!UICONTROL Schemi]**.
1. Fare clic su **[!UICONTROL Crea schema]**.

   ![Finestra di dialogo per creazione schema](assets/schemas-create1.png)

1. Immettere uno spazio dei nomi per lo schema, ad esempio `cus` per gli schemi personalizzati.
1. Immetti un nome e un’etichetta univoci e scegli se desideri creare un nuovo schema o estenderne uno esistente.

1. Fai clic su **[!UICONTROL Crea]**.
   ![Finestra di dialogo per creazione schema](assets/schemas-create2.png)

Lo schema viene creato e viene visualizzata la struttura dello schema generata.

Per impostazione predefinita, lo schema è vuoto. Ora devi aggiungere i campi da includere nello schema utilizzando l’editor schema:

1. Fai clic sull&#39;icona della matita nella sezione **[!UICONTROL Contenuto]** della schermata dei dettagli dello schema.
2. Aggiungi gli elementi necessari e salva. Di seguito è riportato un esempio di struttura di schema personalizzata:

   ![Finestra di dialogo per creazione schema](assets/schemas-create3.png)

Il sistema convalida automaticamente la struttura XML e genera lo schema.

### Definire l’edizione dello schermo {#define-attributes}

Dopo aver creato lo schema, è necessario definire l’edizione dello schermo.

Per ulteriori informazioni sulla schermata di definizione dello schermo e su come accedervi, fare riferimento alla sezione [Accedere alla definizione dello schermo](schemas-browse-access.md#screen-def).

Nel nostro esempio, aggiungiamo semplicemente due campi personalizzati:

1. Fare clic sul pulsante **[!UICONTROL Screen edition]** nella visualizzazione dei dettagli dello schema per accedere alla definizione dello schermo.

1. Fai clic sull&#39;icona con i puntini di sospensione sopra la tabella **[!UICONTROL Elenco campi personalizzati]** e scegli **[!UICONTROL Seleziona attributi]**.
1. Seleziona i campi personalizzati da aggiungere e confermare.

   ![Finestra di dialogo per creazione schema](assets/schemas-create4.png)

## Pubblicare e sincronizzare gli schemi {#publish}

Dopo aver creato o modificato uno schema, è necessario pubblicarlo per sincronizzarlo con la struttura fisica del database.

### Pubblica modifiche schema {#publish-changes}

>[!CAUTION]
>
>La pubblicazione delle modifiche allo schema modifica la struttura del database. Assicurati di comprendere l’impatto di queste modifiche prima di confermare la pubblicazione.

Per pubblicare le modifiche allo schema:

1. Passa a **[!UICONTROL Amministrazione]** > **[!UICONTROL Schemi]** per accedere all&#39;elenco degli schemi.
1. Fai clic su **[!UICONTROL Pubblicazione]** e conferma.

   ![Finestra di dialogo per la pubblicazione dello schema che mostra le modifiche da applicare](assets/schemas-publish1.png)

1. Selezionare nell&#39;elenco lo schema da sincronizzare.

   ![Finestra di dialogo per la pubblicazione dello schema che mostra le modifiche da applicare](assets/schemas-publish2.png)

1. Verificare lo script SQL che verrà eseguito per aggiornare la struttura del database.
1. Fai clic su **[!UICONTROL Pubblica]** e conferma per continuare con la pubblicazione.

>[!NOTE]
>
>Il processo può richiedere un po’ di tempo a seconda delle dimensioni del database e della complessità delle modifiche.

### Creare una voce di navigazione {#navigation}

Dopo aver pubblicato uno schema personalizzato, puoi creare una voce di navigazione in Esplora risorse per accedere ai dati personalizzati:

1. Passa al menu **[!UICONTROL Explorer]** e seleziona la cartella in cui vuoi inserire lo schema personalizzato.
1. Fai clic sull&#39;icona con i puntini di sospensione e fai clic su **[!UICONTROL Crea nuova cartella]**.
   ![Creazione voce di navigazione per schema personalizzato](assets/schemas-publish3.png)
1. Aggiungi un&#39;etichetta e scegli lo schema nel campo **[!UICONTROL Tipo cartella]**.
   ![Creazione voce di navigazione per schema personalizzato](assets/schemas-publish5.png)
1. Lo schema personalizzato sarà ora accessibile dalla visualizzazione **[!UICONTROL Explorer]**.

Dalla nuova cartella, puoi:

* Visualizza l’elenco dei record nello schema personalizzato.
* Crea nuovi record.
* Modifica ed elimina i record esistenti.
* Personalizzare le colonne da visualizzare per impostazione predefinita nella vista a elenco.
