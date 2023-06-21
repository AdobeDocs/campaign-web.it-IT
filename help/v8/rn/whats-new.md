---
audience: end-user
title: Novità di Campaign Web v8
description: Scopri la nuova funzione in arrivo con Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha"
source-git-commit: 4a439abca9c7b1f2cc5d82214efb0aae033a996c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 97%

---


# Novità {#new}

## Versione Alpha 2.0{#alpha-release}

Questa nuova interfaccia web di Campaign è attualmente disponibile solo per i **professionisti alfa** con le seguenti funzionalità:

**Esperienza moderna, intuitiva e unificata**

La nuova interfaccia Web di Campaign offre una nuova esperienza utente, allineata con tutte le soluzioni e le app Adobe Experience Cloud. Offre le seguenti funzionalità:

* Accesso alla nuova interfaccia e ad altre soluzioni Adobe con una sessione utente singola e condivisa
* Nuova esperienza di navigazione, con tutti i menu e le cartelle disponibili nella barra a sinistra
* Possibilità di passare a un’altra soluzione o organizzazione, mediante l’apposito controllo nella barra superiore
* Integrazione Unified Shell, con accesso diretto alla community, al centro assistenza e al supporto

**Nuove potenti funzionalità e processi fluidi**

* Interfaccia dell’area di lavoro del flusso di lavoro riprogettata per progettare e gestire i processi
* Contenuti dinamici per consegnare al pubblico esperienze altamente mirate e personalizzate
* Integrazione nativa con i tipi di pubblico di Adobe Experience Platform
* Gestione dei modelli per flussi di lavoro, consegne, campagne e contenuti

Per ulteriori informazioni sulla nuova interfaccia, visita [questa pagina](../get-started/user-interface.md).

**Creare, avviare e misurare le campagne**

Utilizza la nuova interfaccia di Campaign Web per:

* Progettare contenuti e-mail personalizzati con l&#39;e-mail designer - [Ulteriori informazioni](../content/edit-content.md)
* Invia campagne cross-channel, inclusi SMS e notifiche push.
* Definire i tipi di pubblico target con il generatore di regole - [Ulteriori informazioni](../audience/about-audiences.md)
* Visualizzare l‘anteprima, testare e inviare i messaggi e-mail - [Ulteriori informazioni](../monitor/prepare-send.md)
* Monitorare i risultati di invio e misurazione con i rapporti incorporati - [Ulteriori informazioni](../reporting/delivery-reports.md)


## Passaggio all’interfaccia utente di Campaign Web

In qualità di utente di Campaign, puoi comunque accedere alla console client per generare e gestire le risorse e i componenti di Campaign. I dati e le impostazioni vengono sincronizzati da un ambiente all’altro. Per ulteriori informazioni, consulta [questa sezione](../get-started/get-started.md#about-campaign-client-consoleac-client).

Inoltre, tutti i dati e le impostazioni già disponibili nella console client sono visibili nell’interfaccia utente di Campaign Web, dal menu di navigazione a sinistra di Explorer. Per ulteriori informazioni sulla vista di Explorer, consulta [questa sezione](../get-started/user-interface.md#explorer-user-interface-explorer).


## Aggiornamenti terminologici {#terminology-updates}

Se sei già utente di Campaign, tieni presente che alcuni concetti sono stati rinominati per aderire a nuovi standard terminologici. Queste modifiche si applicano solo all’interfaccia utente di Campaign Web e non vengono riportate nella console client. Tali modifiche sono riepilogate di seguito.

* Le “bozze” sono ora **e-mail di test**: per inviare una bozza, utilizza il pulsante **Test** nell’interfaccia per la consegna delle e-mail. Il target delle bozze ora è indicato come **Profili di test**. [Ulteriori informazioni](../preview-test/test-deliveries.md).
* Gli indirizzi seed vengono ora utilizzati come **Profili di test**: invia l’e-mail di test agli indirizzi seed, che sono destinatari aggiuntivi e fittizi nel database.
* L’analisi della consegna ora si chiama **preparazione della consegna**. Per avviare l’analisi, fai clic sul pulsante **Prepara**..
* L’anteprima e-mail è ora disponibile tramite il pulsante **Simula contenuto**.
* Gli elenchi ora sono **Tipi di pubblico**.

## Limitazioni{#limitations-alpha}

Alla presente versione alfa si applicano le seguenti limitazioni:

* Gli unici oggetti modificabili sono Consegne, Campagne, Flussi di lavoro, Tipi di pubblico e Modelli. Gli altri sono di sola lettura. Utilizza i filtri per sfogliarle tutti.
* I tipi di pubblico non possono essere salvati per utilizzi futuri.
* L&#39;interfaccia utente di amministrazione non è disponibile.
* Le metriche di reporting (come le aperture e i dati di tracciamento) vengono aggiornate ogni ora.
* I KPI del dashboard delle consegne vengono aggiornati ogni 5 minuti. - ma la preparazione della consegna avviene in tempo reale.
* Le notifiche Adobe Experience Cloud e la Guida unificata disponibili nella barra superiore finora non sono state integrate.

