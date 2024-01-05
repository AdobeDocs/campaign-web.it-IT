---
audience: end-user
title: Utilizzo del query modeler
description: Scopri come funziona il query modeler di Adobe Campaign Web.
badge: label="Disponibilità limitata"
source-git-commit: fd29d499bc84e381e7a8c016b468ce85837cac6a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 58%

---

# Utilizzo del query modeler {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Nuovo Query Modeler"
>abstract="Adobe Campaign Web dispone di un query modeler che semplifica il processo di filtraggio dei database per selezionare destinazioni specifiche in base a vari criteri. Ciò include l’utilizzo di espressioni e operatori avanzati. Il query modeler è disponibile in ogni contesto in cui è necessario definire regole per filtrare i dati."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Query modeler"
>abstract="Definisci i criteri di filtro per i destinatari o qualsiasi altra dimensione targeting dal database. Approfitta del pubblico di Adobe Experience Platform per migliorare ulteriormente il pubblico target e massimizzare l’impatto della campagna."

Adobe Campaign Web dispone di un query modeler che semplifica il processo di filtraggio dei database per selezionare destinazioni specifiche in base a vari criteri. Tra i criteri figurano l’utilizzo di espressioni e operatori avanzati.

## Accedere al query modeler

Il query modeler è disponibile in ogni contesto in cui è necessario definire regole per filtrare i dati.

| Utilizzo | Esempio |
|  ---  |  ---  |
| **Definire i tipi di pubblico**: specifica la popolazione per la quale desideri eseguire il targeting nei messaggi o nei flussi di lavoro e crea senza difficoltà nuovi tipi di pubblico in base alle tue esigenze. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Personalizzare le attività del flusso di lavoro**: applica regole all’interno delle attività del flusso di lavoro, come Suddivisione e Riconciliazione, in modo da allinearle ai requisiti specifici. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Filtri preimpostati**: crea filtri preimpostati che fungono da scelte rapide durante varie operazioni di filtraggio, sia nell’utilizzo di elenchi di dati che nella formazione del tipo di pubblico per una consegna. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Filtrare i dati dei rapporti**: aggiungi la regola per filtrare i dati visualizzati nei rapporti. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Personalizzare gli elenchi**: crea regole personalizzate per filtrare i dati visualizzati in elenchi come destinatari, elenchi di consegne, ecc. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->

## Interfaccia del query modeler {#interface}

Il modellatore di query fornisce un’area di lavoro centrale in cui creare la query e un riquadro a destra che fornisce informazioni sulla query.

![](assets/query-interface.png)

### Area di lavoro centrale {#canvas}

L’area di lavoro centrale di Query Modeler è il luogo in cui puoi aggiungere e combinare i diversi componenti che creano la query. [Scopri come creare una query](build-query.md)

La barra degli strumenti situata nell’angolo superiore destro dell’area di lavoro offre opzioni per manipolare facilmente i componenti della query e navigare nell’area di lavoro:

* **Modalità di selezione multipla**: seleziona più componenti filtro per copiarli e incollarli nella posizione desiderata.
* **Ruota**: cambia l’area di lavoro verticalmente.
* **Adatta allo schermo**: adatta il livello di zoom dell’area di lavoro allo schermo.
* **Zoom indietro** / **Zoom in**: zoom indietro o nell’area di lavoro.
* **Visualizza mappa**: apre un’istantanea dell’area di lavoro che mostra la tua posizione.

### Riquadro delle proprietà della regola {#rule-properties}

Sul lato destro, il **[!UICONTROL Proprietà delle regole]** fornisce informazioni sulla query. Consente di eseguire varie operazioni per verificare la query e assicurarsi che sia adatta alle tue esigenze. [Scopri come controllare e convalidare la query](build-query.md#check-and-validate-your-query)
