---
audience: end-user
title: Creare tipi di pubblico
description: Scopri come creare tipi di pubblico in Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 29%

---

# Creare tipi di pubblico {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Da questa schermata, puoi accedere all’elenco di tutti i tipi di pubblico a cui è possibile indirizzare i flussi di lavoro e le consegne. Fai clic su **Crea** per creare un nuovo pubblico in un’area di lavoro visiva.<br/><br/>Oltre a iniziare da zero per creare un pubblico semplice, puoi anche perfezionare il pubblico sfruttando le attività del flusso di lavoro. Ad istanza, puoi combinare più tipi di pubblico in uno solo, arricchire il pubblico con attributi esterni o suddividerlo in più tipi di pubblico in base a regole di tua scelta."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Campaign Web consente di creare nuovi tipi di pubblico in un&#39;area di lavoro visiva workflow. Oltre a iniziare da zero per creare un pubblico semplice, puoi anche perfezionare il pubblico sfruttando le attività del flusso di lavoro. Ad istanza, puoi combinare più tipi di pubblico in uno solo, arricchire il pubblico con attributi esterni o suddividerlo in più tipi di pubblico in base a regole di tua scelta.

Una volta creato il workflow, i tipi di pubblico risultanti vengono automaticamente archiviati nel database Campaign insieme a quelli esistenti. Questi tipi di pubblico possono quindi essere utilizzati come target nei flussi di lavoro o nelle consegne autonome.

La **[!UICONTROL colonna Origine]** indica le origini dei tipi di pubblico: **[!UICONTROL Adobe Campaign]** tipi di pubblico vengono creati nella console Adobe Campaign v8 o nell&#39;interfaccia utente Web, mentre **[!UICONTROL Adobe Experience Platform:]** i tipi di pubblico vengono creati all&#39;interno di Adobe Experience Platform e integrati nella Campaign utilizzando l&#39;integrazione di Adobe Systems Origini e destinazioni.

➡️ [Scopri questa funzione nel video](#video)

## Creare il primo pubblico {#create}

Per creare un pubblico, segui questi passaggi:

1. Passa al menu **[!UICONTROL Tipi di pubblico]** e fai clic sul pulsante **[!UICONTROL Crea pubblico]** nell&#39;angolo in alto a destra.

1. Viene creato automaticamente un nuovo flusso di lavoro, che consente di combinare le attività per generare il pubblico. Per impostazione predefinita, il canvas contiene due attività principali:

   * L&#39;attività &quot;Query&quot; **[!UICONTROL Build audience]** è il punto di partenza del tuo workflow. Ti consente di creare un pubblico e utilizzarlo come base per il tuo workflow.

   * L&#39;attività &quot;Nuovo audience&quot; **[!UICONTROL Salva audience]** rappresenta il passaggio finale della tua workflow. Consente di salvare i risultati come nuovo pubblico.

   ![Un&#39;area di lavoro vuota per la creazione di audience con due attività predefinite: Creare audience e Salva audience.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >I flussi di lavoro del pubblico vengono archiviati nel menu Flussi di **lavoro, insieme agli** altri flussi di lavoro Campaign. Sono progettati specificamente per versione pubblico e sono identificabili dalla loro tela verticale.

1. Per una migliore leggibilità, modifica il nome del workflow nel campo Etichetta delle impostazioni **workflow** . [Scopri come configurare le impostazioni di workflow](../workflows/workflow-settings.md)

1. Apri l&#39;attività **[!UICONTROL Genera pubblico]** e utilizza il modellatore di query per definire la popolazione da includere nel pubblico filtrando i dati contenuti nel database. [Scopri come configurare un’attività Crea pubblico](../workflows/activities/build-audience.md)

1. Se desideri eseguire operazioni aggiuntive sulla popolazione di destinazione nel flusso di lavoro, aggiungi tutte le attività necessarie e collegale tra loro. Per ulteriori informazioni su come configurare le attività del flusso di lavoro, consulta la [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro relativi al pubblico.

   ![Un&#39;area di lavoro per la creazione di audience con più attività collegate per perfezionare l&#39;audience.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configura l’attività **[!UICONTROL Salva pubblico]** per specificare come salvare la popolazione calcolata a monte nel flusso di lavoro. [Scopri come configurare un’attività Salva pubblico](../workflows/activities/save-audience.md)

1. Quando il flusso di lavoro è pronto, fai clic su **[!UICONTROL Avvia]** per eseguirlo.

Il workflow viene salvato nell&#39;elenco **[!UICONTROL Flussi di lavoro, mentre i tipi di]** pubblico risultanti sono accessibili nell&#39;elenco **[!UICONTROL Audiences]** con l&#39;etichetta definita nell&#39;attività **di Salva pubblico** . Scopri informazioni su come monitorare e gestire i tipi di pubblico in [questa sezione](manage-audience.md)

Ora puoi utilizzare questo pubblico come target principale di una consegna. [Ulteriori informazioni](add-audience.md)

## Esempio di flusso di lavoro del pubblico {#example}

L’esempio seguente mostra un flusso di lavoro del pubblico configurato per rivolgersi alle clienti di sesso femminile che vivono a New York e creare due nuovi tipi di pubblico in base al loro ultimo acquisto (articoli da yoga o da corsa).

![Esempio di flusso di lavoro del pubblico indirizzato a clienti di sesso femminile a New York e suddiviso in base al loro ultimo acquisto.](assets/audiences-example.png){zoomable="yes"}

1. L’attività **[!UICONTROL Crea pubblico]** è indirizzata a tutti i profili femminili che vivono a New York.
1. L’attività **[!UICONTROL Arricchimento]** arricchisce il pubblico con le informazioni contenute nella tabella Acquisti per identificare quale tipo di prodotto hanno acquistato le clienti.
1. L’attività **[!UICONTROL Dividi]** separa il flusso di lavoro in due percorsi in base all’ultimo acquisto effettuato dalla cliente.
1. Le **[!UICONTROL attività di audience]** Salva alla fine di ogni percorso creano due nuove audience nel database, inclusa la popolazione calcolata in ogni percorso.

## Modifica un pubblico {#edit}

Puoi modificare un pubblico generato da un workflow ogni volta che è necessario eseguendo nuovamente il workflow corrispondente. Ciò consente di aggiornare i dati del pubblico o di perfezionare il pubblico modificando la query in base alle proprie esigenze.

1. Passa al **menu Audiences** e apri il pubblico da modificare.
1. Nella scheda **Panoramica**, la sezione **Ultimo flusso di lavoro** fornisce un collegamento al flusso di lavoro utilizzato per generare il pubblico. Fai clic su di esso per accedere al flusso di lavoro.
1. Apportare le modifiche desiderate e fare clic sul pulsante **Avvia** per eseguire nuovamente il flusso di lavoro. Al termine, il pubblico risultante dal flusso di lavoro viene aggiornato automaticamente con i risultati del flusso di lavoro più recenti.

Per impostazione predefinita, l’esecuzione ripetuta di un flusso di lavoro per un pubblico sostituisce l’intero contenuto del pubblico con nuovi dati, causando la perdita di dati precedenti.

Se preferisci non sostituire i risultati del pubblico esistente, configura le attività del **pubblico** Salva in modo che siano allineate alle tue esigenze. Ad esempio, puoi modificare il campo dell&#39;etichetta **Pubblico** per store i nuovi risultati in un nuovo pubblico o aggiungere i nuovi risultati al contenuto di pubblico esistente senza cancellare i dati precedenti. [Scopri come configurare un’attività Salva pubblico](../workflows/activities/save-audience.md)

![Schermata di configurazione dell&#39;attività Save audience con opzioni per regolare il comportamento di salvataggio del pubblico.](assets/edit-audience-save.png){zoomable="yes"}

## Video dimostrativo {#video}

Scopri come creare e gestire i tipi di pubblico, come selezionare i tipi di pubblico per una consegna e definire gruppi di controllo.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)