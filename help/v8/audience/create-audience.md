---
audience: end-user
title: Creare tipi di pubblico
description: Scopri come creare tipi di pubblico in Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# Creare tipi di pubblico {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Tipi di pubblico"
>abstract="Da questa schermata, puoi creare e combinare i tipi di pubblico in un’area di lavoro visiva. Aggiungi varie attività del flusso di lavoro, ad esempio **Dividi** o **Escludi** per generare un pubblico nuovo e perfezionato."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Impostazioni pubblico"
>abstract="Immetti il nome del pubblico e altre opzioni, quindi fai clic sul pulsante **Crea pubblico** pulsante."

Campaign Web consente di creare nuovi tipi di pubblico in un’area di lavoro del flusso di lavoro visiva. Oltre a iniziare da zero per creare un pubblico semplice, puoi anche sfruttare le attività del flusso di lavoro per perfezionare i tipi di pubblico. Ad esempio, puoi creare più tipi di pubblico in un unico pubblico, arricchire i tipi di pubblico con attributi esterni o dividere un determinato pubblico in più tipi di pubblico.

Dopo aver creato il flusso di lavoro, i tipi di pubblico risultanti vengono automaticamente memorizzati nel database di Campaign insieme a quelli esistenti. Questi tipi di pubblico possono quindi essere oggetto di targeting in campagne o consegne autonome.

I passaggi principali per creare un pubblico sono i seguenti:

1. Crea un flusso di lavoro per il pubblico.
1. Configura un’attività Genera pubblico per eseguire query sul database in base alle tue esigenze.
1. Aggiungi attività del flusso di lavoro per perfezionare il pubblico (facoltativo).
1. Configurare un’attività Save audience.
1. Esegui il flusso di lavoro per salvare nel database i tipi di pubblico risultanti.


## Creare il primo pubblico {#create}

Per creare un pubblico, segui questi passaggi:

1. Accedi a **[!UICONTROL Tipi di pubblico]** e fai clic sul pulsante **[!UICONTROL Crea pubblico]** nell&#39;angolo superiore destro.
1. Fornisci un’etichetta per il pubblico.
1. Espandi **[!UICONTROL Opzioni aggiuntive]** per configurare parametri di pubblico avanzati.

   Per impostazione predefinita, i tipi di pubblico vengono creati in **[!UICONTROL Profili e destinazioni]** / **[!UICONTROL Elenchi]** menu di esplora risorse. È possibile modificare il percorso di archiviazione predefinito utilizzando **[!UICONTROL Cartella]** campo.

   ![](assets/audiences-settings.png)

1. Dopo aver configurato le impostazioni per il pubblico, fai clic su **[!UICONTROL Crea pubblico]** pulsante.

1. Viene visualizzata un’area di lavoro del flusso di lavoro con due attività predefinite:

   * **[!UICONTROL Creare un pubblico]**: questo è il punto di partenza del flusso di lavoro, che consente di creare un pubblico e utilizzarlo come base per il flusso di lavoro. [Scopri come configurare un’attività Genera pubblico](../workflows/activities/build-audience.md)

   * **[!UICONTROL Salva pubblico]**: questo rappresenta il passaggio finale nel flusso di lavoro, che consente di salvare i risultati come un nuovo pubblico. [Scopri come configurare un’attività Save audience](../workflows/activities/save-audience.md)

1. Se si desidera eseguire un&#39;operazione aggiuntiva dopo **[!UICONTROL Creare un pubblico]** , aggiungi nel flusso di lavoro tutte le attività necessarie. Per ulteriori informazioni su come configurare le attività del flusso di lavoro, consulta [documentazione sui flussi di lavoro](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Le attività del canale non sono disponibili per l’utilizzo nei flussi di lavoro del pubblico.

   ![](assets/audience-creation-canvas.png)

1. Quando il workflow è pronto, fai clic su **[!UICONTROL Inizio]** per eseguirlo.

1. Il flusso di lavoro viene salvato in **[!UICONTROL Flussi di lavoro]** , mentre i tipi di pubblico risultanti sono accessibili nel **[!UICONTROL Tipi di pubblico]** elenco. [Scopri come monitorare e gestire i tipi di pubblico](access-audiences.md)

## Esempio di flusso di lavoro per il pubblico {#example}

L’esempio seguente mostra un flusso di lavoro del pubblico configurato per rivolgersi alle clienti di sesso femminile che vivono a New York e creare due nuovi tipi di pubblico in base al loro centro di interesse in Yoga o in Attrezzatura da corsa. I due tipi di pubblico sono arricchiti da informazioni aggiuntive relative agli acquisti dei clienti.

AGGIUNGI SCHERMATA

1. L’attività Build audience esegue il targeting di tutti i profili di sesso femminile che vivono a New York.
1. L’attività Enrichment arricchisce il pubblico con gli attributi della tabella Purchases.
1. L’attività Split divide il flusso di lavoro in due percorsi in base ai centri di interesse dei clienti.
1. Le attività Save audience alla fine di ogni percorso per salvare ogni pubblico nel database.
