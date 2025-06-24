---
audience: end-user
title: Utilizzo del query modeler
description: Scopri come funziona il query modeler di Adobe Campaign Web.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: dfe670447ed3f1e09191460e8ac6aceee9035bb2
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 24%

---

# Utilizzo del query modeler {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Nuovo generatore di regole"
>abstract="È ora disponibile un nuovo generatore di regole che consente di definire condizioni complesse in un’interfaccia utente migliorata. Se necessario, puoi passare dal generatore di regole precedente a quello nuovo."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Nuovo query modeler"
>abstract="Adobe Campaign Web dispone di un query modeler che semplifica il processo di filtraggio dei database per selezionare destinazioni specifiche in base a vari criteri. Tra i criteri figurano l’utilizzo di espressioni avanzate e operatori. Il query modeler è disponibile in ogni contesto in cui è necessario definire regole per filtrare i dati."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Query modeler"
>abstract="Definisci i criteri di filtro per i destinatari o qualsiasi altra dimensione targeting dal database. Approfitta del pubblico di Adobe Experience Platform per migliorare ulteriormente il pubblico target e massimizzare l’impatto della campagna."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Perfezionare la destinazione"
>abstract="Questi regole possono essere modificate solo nella console client."

L’interfaccia utente web di Adobe Campaign dispone di un modellatore di query che semplifica il processo di filtraggio del database in base a vari criteri. Garantisce la piena compatibilità con le query create nella console client, semplificando la transizione all’interfaccia utente web.

Inoltre, Query Modeler gestisce in modo efficiente query molto complesse e lunghe, offrendo maggiore flessibilità e precisione. Inoltre, supporta filtri predefiniti all’interno di condizioni, consentendo agli utenti di perfezionare le query con facilità e allo stesso tempo utilizzare espressioni avanzate e operatori per strategie complete di targeting del pubblico e segmentazione.

## Accedere al query modeler

Il query modeler è disponibile in ogni contesto in cui è necessario definire regole per filtrare i dati.

| Utilizzo | Esempio |
|  ---  |  ---  |
| **Definisci i tipi di pubblico**: specifica la popolazione di cui desideri eseguire il targeting nei messaggi o nei flussi di lavoro e crea facilmente nuovi tipi di pubblico personalizzati in base alle tue esigenze. [Scopri come creare tipi di pubblico](../audience/one-time-audience.md) | ![Immagine che mostra come accedere all&#39;interfaccia di creazione del pubblico](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Personalizza attività flusso di lavoro**: applica regole all&#39;interno delle attività del flusso di lavoro, ad esempio **Dividi** e **Riconciliazione**, per allinearle ai requisiti specifici. [Ulteriori informazioni sulle attività del flusso di lavoro](../workflows/activities/about-activities.md) | ![Immagine che mostra come accedere alle opzioni di personalizzazione del flusso di lavoro](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Filtri predefiniti**: crea filtri predefiniti da usare come scelte rapide durante varie operazioni di filtro, sia che si utilizzino elenchi di dati che che si formi il pubblico per una consegna. [Scopri come utilizzare i filtri preimpostati](../get-started/predefined-filters.md) | ![Immagine che mostra come accedere ai filtri predefiniti](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Filtrare i dati dei report**: aggiungere regole per filtrare i dati visualizzati nei report. [Scopri come utilizzare i report](../reporting/gs-reports.md) | ![Immagine che mostra come filtrare i dati nei report](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Personalizza elenchi**: crea regole personalizzate per filtrare i dati visualizzati in elenchi quali destinatari o elenchi di consegne. [Scopri come filtrare gli elenchi](../get-started/list-filters.md#list-built-in-filters) | ![Immagine che mostra come personalizzare i filtri elenco](assets/access-lists.png){width="200" align="center" zoomable="yes"} |
| **Crea contenuto condizionale**: rendi dinamico il contenuto delle e-mail creando condizioni che definiscono quale contenuto deve essere visualizzato a destinatari diversi, garantendo messaggi personalizzati e pertinenti. [Scopri come creare contenuti condizionali](../personalization/conditions.md) | ![Immagine che mostra come creare il contenuto condizionale](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

>[!NOTE]
>
>Quando si accede a un oggetto creato nella console client in cui sono state applicate le regole, ad esempio un pubblico o un filtro predefinito, è possibile che venga visualizzata la sezione **[!UICONTROL Perfeziona destinazione]**. Ciò significa che sono stati configurati parametri aggiuntivi per perfezionare il target della regola. Questi parametri possono essere modificati solo nella console.
>
>![Immagine che mostra un avviso relativo all&#39;ottimizzazione delle destinazioni](assets/target-warning.png){zoomable="yes"}

## Interfaccia del query modeler {#interface}

Il modellatore di query fornisce un’area di lavoro centrale in cui creare la query e un riquadro a destra che fornisce informazioni sulla query.

>[!IMPORTANT]
>
>È disponibile una nuova interfaccia per Query Modeler. Il nuovo generatore di regole consente di creare la query con maggiore facilità grazie alla sua interfaccia semplificata. Per passare a questa esperienza, premi il pulsante di attivazione nell’angolo in alto a destra. Per tornare al modellatore di query classico in qualsiasi momento, è sufficiente premere nuovamente il pulsante per disattivare la nuova interfaccia. In questa nuova interfaccia è possibile applicare gli stessi principi del modellatore di query.
>&#x200B;>![Immagine che mostra l&#39;interruttore per la nuova interfaccia del generatore di regole](assets/query-modeler-toggle.png){zoomable="yes"}


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Nuova esperienza del generatore di regole"
>abstract="Utilizza questa opzione per passare dal query modeler classico alla nuova esperienza del generatore di regole. Il nuovo generatore di regole ti consente di creare la query più facilmente, grazie all’interfaccia semplificata e intuitiva."

![Immagine che mostra l&#39;interfaccia di Query Modeler](assets/query-interface.png){zoomable="yes"}

### Area di lavoro centrale {#canvas}

Nell’area di lavoro centrale di Query Modeler puoi aggiungere e combinare i diversi componenti per creare la query. [Scopri come creare una query](build-query.md)

>[!BEGINTABS]

>[!TAB Modellatore di query classico]

La barra degli strumenti situata nell’angolo inferiore destro dell’area di lavoro offre opzioni per manipolare facilmente i componenti della query e navigare nell’area di lavoro:

* **Modalità di selezione multipla**: selezionare più componenti filtro per copiarli e incollarli nel percorso desiderato.
* **Ruota**: cambia l&#39;area di lavoro verticalmente.
* **Adatta allo schermo**: adatta il livello di zoom dell&#39;area di lavoro allo schermo.
* **Zoom indietro** / **Zoom avanti**: Zoom indietro o indietro nell&#39;area di lavoro.
* **Mappa di visualizzazione**: apri uno snapshot dell&#39;area di lavoro che mostra la posizione corrente.

>[!TAB Nuova esperienza con il generatore di regole]

La barra degli strumenti situata nell’angolo superiore destro dell’area di lavoro offre opzioni per manipolare facilmente i componenti della query e navigare nell’area di lavoro:

* **Sposta la selezione verso l&#39;alto**: sposta il componente di una riga verso l&#39;alto.
* **Sposta selezione in basso**: sposta il componente in basso di una riga.
* **Selezione gruppo**: inserire due componenti in un gruppo.
* **Separa la selezione**: separa i componenti di un singolo gruppo.
* **Espandi tutto**: espandi tutti i gruppi.
* **Comprimi tutto**: comprimi tutti i gruppi.
* **Rimuovi tutto**: rimuovi tutti i gruppi e i componenti.

>[!ENDTABS]

### Riquadro delle proprietà della regola {#rule-properties}

Sul lato destro, il riquadro **[!UICONTROL Proprietà regola]** fornisce informazioni sulla query. Consente di eseguire varie operazioni per verificare la query e assicurarsi che sia adatta alle tue esigenze. Questo riquadro viene visualizzato quando si crea una query per creare un pubblico. [Scopri come controllare e convalidare la query](build-query.md#check-and-validate-your-query)
