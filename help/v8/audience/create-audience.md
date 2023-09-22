---
audience: end-user
title: Creare e gestire i tipi di pubblico
description: Scopri come creare e gestire i tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---


# Creare tipi di pubblico {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Da questa schermata, puoi accedere all’elenco di tutti i tipi di pubblico a cui è possibile indirizzare le consegne. Clic **Crea** per creare nuovi tipi di pubblico in un’area di lavoro visiva utilizzando varie attività del flusso di lavoro, ad esempio **Dividi** o **Escludi**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Impostazioni pubblico"
>abstract="Immetti il nome del pubblico e altre opzioni, quindi fai clic sul pulsante **Crea pubblico** pulsante."

Campaign Web consente di creare nuovi tipi di pubblico in un’area di lavoro del flusso di lavoro visiva. Oltre a iniziare da zero per creare un pubblico semplice, puoi anche sfruttare le attività del flusso di lavoro per perfezionare il pubblico. Ad esempio, puoi combinare più tipi di pubblico in un unico pubblico, arricchire il pubblico con attributi esterni o suddividerlo in più tipi di pubblico in base alle regole scelte.

Dopo aver creato il flusso di lavoro, i tipi di pubblico risultanti vengono automaticamente memorizzati nel database di Campaign insieme a quelli esistenti. Questi tipi di pubblico possono quindi essere oggetto di targeting in campagne o consegne autonome.

## Creare il primo pubblico {#create}

Per creare un pubblico, segui questi passaggi:

1. Accedi a **[!UICONTROL Tipi di pubblico]** e fai clic sul pulsante **[!UICONTROL Crea pubblico]** nell&#39;angolo superiore destro.
1. Fornisci un’etichetta per il pubblico.
1. Espandi **[!UICONTROL Opzioni aggiuntive]** per configurare parametri di pubblico avanzati.

   Per impostazione predefinita, i tipi di pubblico vengono creati in **[!UICONTROL Profili e destinazioni]** / **[!UICONTROL Elenchi]** menu di esplora risorse. È possibile modificare il percorso di archiviazione predefinito utilizzando **[!UICONTROL Cartella]** campo.

   ![](assets/audiences-settings.png)

1. Dopo aver configurato le impostazioni per il pubblico, fai clic su **[!UICONTROL Crea pubblico]** pulsante. Viene visualizzata un’area di lavoro del flusso di lavoro con due attività predefinite:

   * **[!UICONTROL Creare un pubblico]**: questo è il punto di partenza del flusso di lavoro, che consente di creare un pubblico e utilizzarlo come base per il flusso di lavoro.

   * **[!UICONTROL Salva pubblico]**: questo rappresenta il passaggio finale nel flusso di lavoro, che consente di salvare i risultati del flusso di lavoro come un nuovo pubblico.

1. Apri **[!UICONTROL Creare un pubblico]** e utilizza il generatore di regole per definire la popolazione da includere nel pubblico filtrando i dati contenuti nel database. [Scopri come configurare un’attività Genera pubblico](../workflows/activities/build-audience.md)

1. Se desideri eseguire operazioni aggiuntive sulla popolazione di destinazione nel flusso di lavoro, aggiungi tutte le attività necessarie e collegale tra loro. Per ulteriori informazioni su come configurare le attività del flusso di lavoro, consulta [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro del pubblico.

   ![](assets/audience-creation-canvas.png)

1. Configurare **[!UICONTROL Salva pubblico]** per specificare come salvare la popolazione calcolata a monte nel flusso di lavoro. [Scopri come configurare un’attività Save audience](../workflows/activities/save-audience.md)

1. Quando il workflow è pronto, fai clic su **[!UICONTROL Inizio]** per eseguirlo.

Il flusso di lavoro viene salvato in **[!UICONTROL Flussi di lavoro]** , mentre i tipi di pubblico risultanti sono accessibili nel **[!UICONTROL Tipi di pubblico]** elenco.

## Esempio di flusso di lavoro per il pubblico {#example}

L’esempio seguente mostra un flusso di lavoro del pubblico configurato per rivolgersi alle clienti di sesso femminile che vivono a New York e creare due nuovi tipi di pubblico in base al loro ultimo acquisto (Yoga o Running gear).

![](assets/audiences-example.png)

1. Il **[!UICONTROL Creare un pubblico]** L’attività è indirizzata a tutti i profili femminili che vivono a New York.
1. Il **[!UICONTROL Arricchimento]** L’attività arricchisce il pubblico con le informazioni contenute nella tabella Purchases per identificare quale tipo di prodotto hanno acquistato i clienti.
1. Il **[!UICONTROL Dividi]** L’attività divide il flusso di lavoro in due percorsi in base all’ultimo acquisto effettuato dal cliente.
1. Il **[!UICONTROL Salva pubblico]** Le attività alla fine di ciascun percorso creano due nuovi tipi di pubblico nel database, inclusa la popolazione calcolata in ciascun percorso.

## Monitorare e gestire i tipi di pubblico {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Errore di pubblico"
>abstract="I dati sul pubblico non sono disponibili. Attendi la fine dell&#39;esecuzione del flusso di lavoro."

L’elenco dei tipi di pubblico disponibili per l’utilizzo in Campaign Web è accessibile dalla pagina **[!UICONTROL Tipi di pubblico]** menu.

![](assets/audiences-list.png)

I tipi di pubblico possono provenire da più sorgenti. Il **[!UICONTROL Origine]** Le colonne indicano dove è stato creato un determinato pubblico:

* **[!UICONTROL Adobe Campaign]**: questi tipi di pubblico vengono creati nella console di Adobe Campaign V8. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=it){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Questi tipi di pubblico vengono creati all’interno di Adobe Experience Platform e sono integrati in Campaign Web utilizzando l’integrazione Adobe Sources and Destinations. Scopri come impostare questa integrazione in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Interfaccia web di Adobe Campaign]**: questi tipi di pubblico vengono creati utilizzando i flussi di lavoro Pubblico web di Campaign. [Scopri come creare tipi di pubblico](create-audience.md)

Per ottenere ulteriori informazioni su un pubblico, aprilo dall’elenco. Vengono visualizzate le proprietà del pubblico e il numero di profili inclusi nel pubblico. Puoi aggiornare il conteggio del pubblico in qualsiasi momento utilizzando **[!UICONTROL Calcola]** pulsante.

Il **[!UICONTROL Dati]** Questa scheda ti consente di visualizzare i profili che fanno parte del pubblico. Puoi personalizzare questa visualizzazione aggiungendo più colonne o sfruttando filtri avanzati per perfezionare i dati visualizzati.

![](assets/audiences-details.png)

Per duplicare o eliminare un pubblico, fai clic su **[!UICONTROL Altre azioni]** disponibile nell’elenco dei tipi di pubblico accanto al nome del pubblico o all’interno della schermata dei dettagli del pubblico.
