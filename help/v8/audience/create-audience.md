---
audience: end-user
title: Creare tipi di pubblico
description: Scopri come creare tipi di pubblico in Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 44c3cb9905850719e75bd5199b907c78d3cd7467
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 52%

---

# Creare tipi di pubblico {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Composizione del pubblico"
>abstract="Crea nuovi tipi di pubblico in nell’area di lavoro del flusso di lavoro. Oltre a iniziare da zero per creare un pubblico semplice, puoi anche perfezionare il pubblico sfruttando le attività del flusso di lavoro. Puoi combinare più tipi di pubblico in un unico pubblico, arricchirlo con attributi esterni o suddividerlo in più tipi di pubblico in base alle regole scelte."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Da questa schermata, puoi accedere all’elenco di tutti i tipi di pubblico a cui è possibile indirizzare i flussi di lavoro e le consegne. Fai clic su **Crea** per creare un nuovo pubblico in un’area di lavoro visiva.<br/><br/>Oltre a iniziare da zero per creare un pubblico semplice, puoi anche perfezionare il pubblico sfruttando le attività del flusso di lavoro. Ad esempio, puoi combinare più tipi di pubblico in un unico pubblico, arricchirlo con attributi esterni o suddividerlo in più tipi di pubblico in base alle regole scelte"

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Campaign Web consente di creare nuovi tipi di pubblico in un’area di lavoro visiva per i flussi di lavoro. Oltre a iniziare da zero per creare un pubblico semplice, puoi anche perfezionare il pubblico sfruttando le attività del flusso di lavoro. Ad esempio, puoi combinare più tipi di pubblico in un unico pubblico, arricchirlo con attributi esterni o suddividerlo in più tipi di pubblico in base alle regole scelte

Dopo aver creato il flusso di lavoro, i tipi di pubblico risultanti vengono automaticamente memorizzati nel database di Campaign insieme a quelli esistenti. Questi tipi di pubblico possono quindi essere utilizzati come target nei flussi di lavoro o nelle consegne autonome.

Il **[!UICONTROL Origine]** le colonne indicano le origini dei tipi di pubblico: **[!UICONTROL Adobe Campaign]** i tipi di pubblico sono stati creati nella console di Adobe Campaign v8 o nell’interfaccia utente web, mentre **[!UICONTROL Adobe Experience Platform:]** I tipi di pubblico sono stati creati all’interno di Adobe Experience Platform e integrati in Campaign utilizzando l’integrazione Adobe Sources and Destinations.

➡️ [Scopri questa funzione nel video](#video)

## Creare il primo pubblico {#create}

Per creare un pubblico, segui questi passaggi:

1. Passa al menu **[!UICONTROL Tipi di pubblico]** e fai clic sul pulsante **[!UICONTROL Crea pubblico]** in alto a destra.

1. Viene creato automaticamente un nuovo flusso di lavoro, che consente di combinare le attività per generare il pubblico. Per impostazione predefinita, l’area di lavoro contiene due attività principali:

   * La &quot;Query&quot; **[!UICONTROL Creare un pubblico]** l’attività è il punto di partenza del flusso di lavoro, che consente di creare un pubblico e utilizzarlo come base per il flusso di lavoro.

   * Il &quot;Nuovo pubblico&quot; **[!UICONTROL Salva pubblico]** l’attività rappresenta il passaggio finale nel flusso di lavoro, che consente di salvare i risultati come un nuovo pubblico.

   ![](assets/create-audience-blank.png){zoomable=&quot;yes&quot;}

   >[!IMPORTANT]
   >
   >I flussi di lavoro del pubblico sono memorizzati nella **Flussi di lavoro** , insieme agli altri flussi di lavoro di Campaign. Sono progettati specificamente per creare tipi di pubblico e sono identificabili dalla loro area di lavoro verticale.

1. Per una migliore leggibilità, si consiglia di modificare il nome del flusso di lavoro nelle relative impostazioni. **Etichetta** campo. [Scopri come configurare le impostazioni del flusso di lavoro](../workflows/workflow-settings.md)

1. Apri **[!UICONTROL Creare un pubblico]** e utilizza Query Modeler per definire la popolazione da includere nel pubblico filtrando i dati contenuti nel database. [Scopri come configurare un’attività Crea pubblico](../workflows/activities/build-audience.md)

1. Se desideri eseguire operazioni aggiuntive sulla popolazione target nel flusso di lavoro, aggiungi tutte le attività necessarie e collegale tra loro. Per ulteriori informazioni su come configurare le attività del flusso di lavoro, consulta la [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro relativi al pubblico.

   ![](assets/audience-creation-canvas.png){zoomable=&quot;yes&quot;}

1. Configura l’attività **[!UICONTROL Salva pubblico]** per specificare come salvare la popolazione calcolata a monte nel flusso di lavoro. [Scopri come configurare un’attività Salva pubblico](../workflows/activities/save-audience.md)

1. Quando il flusso di lavoro è pronto, fai clic su **[!UICONTROL Avvia]** per eseguirlo.

Il flusso di lavoro viene salvato in **[!UICONTROL Flussi di lavoro]** , mentre i tipi di pubblico risultanti sono accessibili nel **[!UICONTROL Tipi di pubblico]** con l’etichetta definita nella sezione **Salva pubblico** attività. Scopri come monitorare e gestire i tipi di pubblico in [questa sezione](manage-audience.md)

Ora puoi utilizzare questo pubblico come target principale di una consegna. [Ulteriori informazioni](add-audience.md)

## Esempio di flusso di lavoro del pubblico {#example}

L’esempio seguente mostra un flusso di lavoro del pubblico configurato per rivolgersi alle clienti di sesso femminile che vivono a New York e creare due nuovi tipi di pubblico in base al loro ultimo acquisto (articoli da yoga o da corsa).

![](assets/audiences-example.png){zoomable=&quot;yes&quot;}

1. L’attività **[!UICONTROL Crea pubblico]** è indirizzata a tutti i profili femminili che vivono a New York.
1. L’attività **[!UICONTROL Arricchimento]** arricchisce il pubblico con le informazioni contenute nella tabella Acquisti per identificare quale tipo di prodotto hanno acquistato le clienti.
1. L’attività **[!UICONTROL Dividi]** separa il flusso di lavoro in due percorsi in base all’ultimo acquisto effettuato dalla cliente.
1. Le attività **[!UICONTROL Salva pubblico]** alla fine di ciascun percorso creano due nuovi tipi di pubblico nel database, che includono la popolazione calcolata in ciascun percorso.

## Modificare un pubblico {#edit}

Puoi modificare un pubblico generato da un flusso di lavoro ogni volta che sia necessario rieseguendo il flusso di lavoro corrispondente. Questo consente di aggiornare facilmente i dati sul pubblico o di perfezionarlo regolando la query in base alle tue esigenze.

1. Accedi a **Tipi di pubblico** e aprire il pubblico da modificare.
1. In **Panoramica** , la scheda **Ultimo flusso di lavoro** fornisce un collegamento al flusso di lavoro utilizzato per generare il pubblico. Fai clic su di esso per accedere al flusso di lavoro.
1. Apportare le modifiche desiderate e fare clic su **Inizio** per eseguire nuovamente il flusso di lavoro. Al termine, il pubblico risultante dal flusso di lavoro viene aggiornato automaticamente con i risultati del flusso di lavoro più recenti.

Per impostazione predefinita, l’esecuzione ripetuta di un flusso di lavoro per un pubblico sostituisce l’intero contenuto del pubblico con nuovi dati, causando la perdita di dati precedenti.

Se preferisci non sostituire i risultati del pubblico esistenti, configura il **Salva pubblico** attività per allinearle alle tue esigenze. Ad esempio, puoi modificare il **Etichetta del pubblico** per memorizzare i nuovi risultati in un nuovo pubblico o aggiungere i nuovi risultati al contenuto del pubblico esistente senza cancellare i dati precedenti. [Scopri come configurare un’attività Save audience](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png){zoomable=&quot;yes&quot;}

## Video dimostrativo {#video}

Scopri come creare e gestire i tipi di pubblico, come selezionare i tipi di pubblico per una consegna e definire gruppi di controllo.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
