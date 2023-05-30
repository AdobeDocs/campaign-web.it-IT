---
audience: end-user
title: Note sulla versione di Campaign Web v8
description: Note sulla versione di Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: 0703b872bb8f452773e76f2524d47bf774c687e0
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 81%

---


# Note sulla versione {#release-notes}

In questa pagina sono elencate tutte le funzioni e i miglioramenti più recenti per Campaign Web v8.

## Versione alfa{#alpha-release}

Questa nuova interfaccia web di Campaign è attualmente disponibile solo per i **professionisti alfa** con le seguenti funzionalità:

**Esperienza moderna, intuitiva e unificata**

La nuova interfaccia Web di Campaign offre una nuova esperienza utente, allineata con tutte le soluzioni e le app Adobe Experience Cloud. Offre le seguenti funzionalità:

* Accedi alla nuova interfaccia e alle altre soluzioni di Adobe con una sessione utente singola e condivisa
* Nuova esperienza di navigazione, con tutti i menu e le cartelle disponibili nella barra a sinistra
* Possibilità di passare a un’altra soluzione o organizzazione, mediante l’apposito controllo nella barra superiore
* Integrazione Unified Shell, con accesso diretto alla community, al centro assistenza e al supporto

**Nuove potenti funzionalità e processi senza soluzione di continuità**

* Interfaccia dell’area di lavoro del flusso di lavoro riprogettata per progettare e gestire i processi
* Contenuti dinamici per fornire al pubblico esperienze altamente mirate e personalizzate
* Integrazione nativa con il pubblico di Adobe Experience Platform
* Gestione dei modelli per flussi di lavoro, consegne, campagne e contenuti

Per ulteriori informazioni sulla nuova interfaccia, visita [questa pagina](../get-started/user-interface.md).

**Creare, avviare e misurare le campagne**

Utilizza la nuova interfaccia di Campaign Web per:

* Progettare contenuti e-mail personalizzati con l&#39;e-mail designer - [Ulteriori informazioni](../content/edit-content.md)
* Invia campagne cross-channel, incluse notifiche SMS e push.
* Definire i tipi di pubblico target con il generatore di regole - [Ulteriori informazioni](../audience/about-audiences.md)
* Visualizzare l‘anteprima, testare e inviare i messaggi e-mail - [Ulteriori informazioni](../monitor/prepare-send.md)
* Monitorare i risultati di invio e misurazione con i rapporti incorporati - [Ulteriori informazioni](../reporting/delivery-reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Aggiornamenti terminologici{#terminology-updates}

Se sei già utente di Campaign, tieni presente che alcuni concetti sono stati rinominati per aderire a nuovi standard terminologici. Queste modifiche si applicano solo all’interfaccia utente di Campaign Web e non vengono riportate nella console client. Tali modifiche sono riepilogate di seguito.

* Le “bozze” sono ora **e-mail di test**: per inviare una bozza, utilizza il pulsante **Test** nell’interfaccia per la consegna delle e-mail. Il target della destinazione delle bozze ora è indicato come **Profili di test**.
* Gli indirizzi seed vengono ora utilizzati come **Profili di test**: invia l’e-mail di test agli indirizzi seed, che sono destinatari aggiuntivi e fittizi nel database.
* L’analisi della consegna ora si chiama **preparazione della consegna**. Per avviare l’analisi, fai clic sul pulsante **Prepara**.
* L’anteprima e-mail è ora disponibile tramite il pulsante **Simula contenuto**.
* Gli elenchi ora sono **Tipi di pubblico**.

## Limitazioni{#limitations-alpha}

Alla presente versione alfa si applicano le seguenti limitazioni:

* Gli unici oggetti modificabili sono Consegne, Campagne, Flussi di lavoro, Pubblico e Modelli. Gli altri sono di sola lettura. Utilizza i filtri per sfogliarle tutti.
* L&#39;interfaccia utente di amministrazione non è disponibile.
* Le metriche di reporting (come le aperture e i dati di tracciamento) vengono aggiornate ogni ora.
* I KPI del dashboard delle consegne vengono aggiornati ogni 5 minuti. - ma la preparazione della consegna avviene in tempo reale.
* Le notifiche Adobe Experience Cloud e la Guida unificata disponibili nella barra superiore finora non sono state integrate.

