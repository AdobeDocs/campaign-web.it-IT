---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: b8cf1d45b1a69efbe8e055d57b430d0fa04f8494
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 93%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione di giugno 2026 {#26-6-release}

_16 giugno 2026_

### Miglioramenti {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Ora puoi esportare dati da qualsiasi schermata dell’elenco, inclusi i registri di tracciamento. Trova il tuo elenco e fai semplicemente clic sul pulsante di esportazione. L’esportazione include le righe attualmente caricate e tiene conto delle colonne visualizzate sullo schermo e di eventuali ricerche o filtri attivi. [Ulteriori informazioni](../get-started/list-filters.md)

* Le attività del flusso di lavoro **Deduplica** e **Termina** ora supportano più transizioni in entrata. Quando sono disponibili più transizioni in entrata, utilizza la sezione **Set per partecipare** nell&#39;attività
proprietà dell’attività per selezionare le transizioni da connettere. Ulteriori informazioni sono disponibili in queste pagine: [Deduplica](../workflows/activities/deduplication.md), [Fine](../workflows/activities/end.md)

* I parametri avanzati sono ora esposti nella sezione **Dati di arricchimento** delle attività del flusso di lavoro **Genera pubblico** (tipo di query) e **Arricchimento**. Questi parametri consentono di ottimizzare la creazione dei dati di arricchimento, inclusi il raggruppamento, la deduplica, la gestione delle chiavi primarie e i dati degli eventi in entrata. [Ulteriori informazioni](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
