---
title: Guardrail e limitazioni nell’interfaccia utente web di Campaign
description: Guardrail e limitazioni nell’interfaccia utente web di Campaign
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 4%

---


# Guardrail e limitazioni {#guardrails-limitations}

Quando lavori nell’interfaccia utente web di Campaign con componenti creati o modificati nella console client di Campaign, si applicano le protezioni e le limitazioni elencate di seguito.

## Flussi di lavoro {#wf-guardrails-limitations}

**Attività**

* Le attività del flusso di lavoro non ancora supportate nell’interfaccia utente web sono di sola lettura. Puoi comunque eseguire il flusso di lavoro, inviare messaggi, controllare i registri e così via. Le attività del flusso di lavoro disponibili sia nell’interfaccia utente web che nella console client sono modificabili.

| Console | Interfaccia web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**Area di lavoro**

* Quando crei un nuovo flusso di lavoro nell’interfaccia utente web, l’area di lavoro supporta un solo punto di ingresso. Tuttavia, se hai creato un flusso di lavoro nella console con più punti di ingresso,

Tuttavia, anche se il flusso di lavoro è stato creato nell’area di lavoro della console client con più punti di ingresso, sarà modificabile anche nell’interfaccia utente web. Puoi comunque aprire e modificare



Per provare questo scenario, crea un flusso di lavoro dalla console client con più punti di ingresso e aprilo dall’interfaccia web per visualizzare il risultato.



Naturalmente, puoi modificare le attività ed avviare ed eseguire normalmente il flusso di lavoro.



**Posizionamento attività**

* Il posizionamento dei nodi verrà ricalcolato (il posizionamento iniziale delle attività verrà quindi modificato) solo quando un’attività è stata aggiunta o rimossa (non sempre).

**Opzioni non esposte**

* Le opzioni non compatibili non vengono visualizzate nell’interfaccia utente web.

**Loop**

* I loop non sono ancora disponibili nell’interfaccia utente web. Se hai creato un flusso di lavoro che include un ciclo continuo utilizzando la console, non puoi accedervi dall’interfaccia utente web. Viene visualizzato un messaggio di errore.

| Console | Interfaccia web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**riconciliazione e arricchimento**

Nella console del client Campaign, il **Arricchimento** L’attività può eseguire sia la riconciliazione che l’arricchimento. Nell’interfaccia utente web di Campaign, le funzionalità di riconciliazione non sono ancora disponibili. Se hai impostato la riconciliazione nell’attività della console, questa verrà visualizzata come un’attività non compatibile nell’interfaccia utente web.

* Se il **Arricchimento** nella console esegue solo un arricchimento, il **Arricchimento** L&#39;attività viene visualizzata nel Web.
* Se il **Arricchimento** l’attività nella console esegue solo una riconciliazione, viene visualizzata un’attività non compatibile.

## Filtri preimpostati {#filters-guardrails-limitations}

In tale versione del prodotto, quando si seleziona il pubblico di una consegna o quando si crea un pubblico in un flusso di lavoro, alcuni filtri predefiniti non sono disponibili nell’interfaccia utente.

Viene visualizzato un messaggio di errore specifico. Anche se non è possibile visualizzare la rappresentazione grafica della query nel generatore di regole e non è possibile modificare il filtro, è comunque possibile utilizzarlo e visualizzare le condizioni di filtro e i risultati. È inoltre possibile accedere alla query SQL per verificare le impostazioni esatte.

![](assets/filter-unavailable.png){width="70%" align="left"}

Nota che se si crea un filtro nell’interfaccia Web e lo si modifica nella console con attributi non supportati, la rappresentazione grafica non può più essere disponibile nell’interfaccia Web. In ogni caso, puoi comunque utilizzare il filtro.

Gli attributi non supportati sono elencati di seguito.

### Tipi di dati non supportati {#unsupported-data-type}

I seguenti tipi di dati disponibili nella console client non sono supportati quando si visualizza un filtro o una regola nell’interfaccia Web:

* datetime
* orario
* intervallo di tempo
* doppio
* galleggiare

### Funzionalità di filtro non supportate {#unsupported-filtering-capabilities}

Quando un filtro viene creato con espressioni e funzioni complesse nella console client, non può essere modificato nell’interfaccia web.

Inoltre, i seguenti operatori non sono supportati:

* Tipo numerico
   * è incluso in
   * no in

* Tipo di stringa
   * maggiore di
   * minore di
   * maggiore o uguale a
   * minore o uguale a
   * mi piace
   * non simile a

* Tipo di data
   * il o dopo il
   * il o prima del
   * diverso da
   * è vuoto
   * non è vuoto
   * è incluso in
   * non in
   * nell’ultimo/a

* Collegamenti 1-N
   * CONTEGGIO, SOMMA, MEDIA, MIN, MAX