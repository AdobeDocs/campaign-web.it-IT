---
title: Guardrail e limitazioni nell’interfaccia utente web di Campaign
description: Guardrail e limitazioni nell’interfaccia utente web di Campaign
badge: label="Beta"
source-git-commit: 4b01e31edeadfa76546da1f906f5e3d2eb74ec13
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 4%

---


# Guardrail e limitazioni {#guardrails-limitations}

Quando lavori nell’interfaccia utente web di Campaign con componenti creati o modificati nella console client di Campaign, si applicano le protezioni e le limitazioni elencate di seguito.

## Flussi di lavoro {#wf-guardrails-limitations}

È possibile accedere allo stesso flusso di lavoro sia nella console che nell’interfaccia utente web. Tuttavia, tieni presente che si applicano alcune limitazioni.

**Edizione attività**

* Quando accedi a un flusso di lavoro della console nell’interfaccia utente web, puoi modificare solo le attività compatibili.

**Edizione Canvas**

* Se un flusso di lavoro della console dispone di più nodi/rami iniziali o attività mobili, è necessario aggiungere un’attività iniziale e un fork per collegare i nodi iniziali al nodo principale. È inoltre necessario rimuovere le attività mobili.

**Posizionamento attività**

* Il posizionamento dei nodi verrà ricalcolato (il posizionamento iniziale delle attività verrà quindi modificato) solo quando un’attività è stata aggiunta o rimossa (non sempre).

**Opzioni non esposte**

* Le opzioni non compatibili non vengono visualizzate nell’interfaccia utente web.

**Loop**

* I flussi di lavoro che includono i loop non vengono visualizzati nell’interfaccia utente web. Viene visualizzato un messaggio di errore.

**riconciliazione e arricchimento**

Nella console del client Campaign, il **Arricchimento** L’attività può eseguire sia la riconciliazione che l’arricchimento. Nell’interfaccia utente web di Campaign, le funzionalità di riconciliazione non sono ancora disponibili. Se hai impostato la riconciliazione nell’attività della console, questa verrà visualizzata come un’attività non compatibile nell’interfaccia utente web.

* Se il **Arricchimento** nella console esegue solo un arricchimento, il **Arricchimento** L&#39;attività viene visualizzata nel Web.
* Se il **Arricchimento** l’attività nella console esegue solo una riconciliazione, viene visualizzata un’attività non compatibile.

## Filtri preimpostati {#filters-guardrails-limitations}

Durante la selezione del pubblico di una consegna o la creazione di un pubblico in un flusso di lavoro, alcuni filtri predefiniti non sono disponibili nell’interfaccia utente, in tale versione del prodotto.

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