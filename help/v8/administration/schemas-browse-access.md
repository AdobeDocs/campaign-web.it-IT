---
title: Sfogliare e accedere agli schemi
description: Scopri come sfogliare e accedere agli schemi nell’interfaccia.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 3%

---

# Accedere e configurare gli schemi {#access}

Gli schemi sono accessibili dal menu **[!UICONTROL Amministrazione]** > **[!UICONTROL Schemi]**.

![Schemi con la schermata dell&#39;elenco che mostra gli schemi e i filtri disponibili](assets/schemas-list.png)

Da questa schermata puoi visualizzare tutti gli schemi esistenti. I filtri sono disponibili per aiutarti a perfezionare l’elenco, ad esempio per visualizzare solo gli schemi modificabili.

Per aprire uno schema, selezionarne il nome. Viene visualizzata una vista di schema dettagliata.

![Schermata dei dettagli dello schema che mostra le proprietà e il contenuto dello schema](assets/schema-details.png)

## Panoramica dello schema {#overview}

La scheda **[!UICONTROL Panoramica]** fornisce una visualizzazione generale dello schema:

* Nella sezione **[!UICONTROL Proprietà]** vengono visualizzate informazioni chiave, ad esempio il nome dello schema, lo spazio dei nomi e il nome della tabella associata.

* La sezione **[!UICONTROL Definizione schema]** mostra i dettagli sulla definizione dello schema, inclusa la chiave primaria utilizzata per la riconciliazione dei dati e i relativi collegamenti ad altre tabelle.

  Fai clic sul pulsante **[!UICONTROL Anteprima schema]** per visualizzare i diversi campi e collegamenti che compongono lo schema. Questo consente di controllare la struttura completa di uno schema. Se lo schema è stato esteso con campi personalizzati, puoi visualizzarne tutte le estensioni.

* La sezione **[!UICONTROL Content]** visualizza il contenuto XML dello schema, consentendo di passare dall&#39;origine alla sintassi generata.

## Dati schema {#data}

La scheda **[!UICONTROL Dati]** fornisce informazioni sui dati dello schema.

![Scheda dati dello schema che mostra la struttura dati e gli attributi](assets/schemas-data.png)

## Personalizzare la visualizzazione dello schermo {#screen-def}

La definizione della schermata ti consente di configurare il modo in cui i campi dello schema vengono visualizzati e modificati nell’interfaccia. È possibile configurare le colonne predefinite per le visualizzazioni elenco, personalizzare i campi personalizzati da visualizzare nelle schermate di dettaglio, aggiungere elenchi di raccolta per visualizzare i dati correlati e organizzare i campi in sezioni con separatori e criteri di visibilità.

Per accedere alla definizione della schermata:

1. Accedi al menu **[!UICONTROL Schemi]** e individua gli schemi modificabili utilizzando i filtri.

   ![Schemi con la schermata dell&#39;elenco che mostra gli schemi e i filtri disponibili](assets/schemas-list2.png)

1. Selezionare il nome dello schema nell&#39;elenco per aprirlo e fare clic sul pulsante **[!UICONTROL Screen edition]** nella visualizzazione dei dettagli dello schema per accedere alla definizione dello schermo.

   ![Schemi con la schermata dell&#39;elenco che mostra gli schemi e i filtri disponibili](assets/schemas-list3.png)

   I diversi elenchi consentono di riordinare gli elementi utilizzando le icone freccia su e freccia giù o trascinarli e rilasciarli. Per rimuovere gli elementi, fare clic sull&#39;icona del cestino su una riga specifica oppure selezionare **[!UICONTROL Elimina tutto]** dall&#39;icona con i puntini di sospensione.

   ![Sezione Generale definizione schermo](assets/schemas-general.png)

Dalla definizione della schermata, puoi effettuare le seguenti operazioni:

* [Configura colonne elenco predefinite](schemas-list-columns.md) - Configura quali colonne vengono visualizzate per impostazione predefinita nelle visualizzazioni elenco.
* [Modifica campi personalizzati](schemas-custom-fields.md) - Configura i campi personalizzati da visualizzare nelle schermate di dettaglio e organizzali in sezioni.
* [Aggiungi elenchi raccolta](schemas-collection-lists.md) - Aggiungi elenchi raccolta per visualizzare i dati correlati nelle schermate del profilo.
