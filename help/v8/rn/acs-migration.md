---
audience: end-user
title: Passaggio da Campaign Standard ad Adobe Campaign Web
description: Interfaccia utente di Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 99%

---

# Passaggio da Campaign Standard a Campaign v8 {#acs-to-ac}

Chi utilizza Adobe Campaign Standard ora può passare ad Adobe Campaign Managed Cloud Services v8. Questa transizione offre diversi vantaggi:

* **Solida infrastruttura IT**: Managed Cloud Service v8 offre un’infrastruttura IT più solida per migliorare le prestazioni, l’affidabilità e la scalabilità delle campagne.
* **Supporto avanzato**: il team Managed Cloud Services offre assistenza di alto livello per garantire una transizione fluida e il monitoraggio continuo della piattaforma. Il supporto include la risoluzione dei problemi e la manutenzione proattiva.
* **Integrazione con Adobe Experience Platform**: Managed Cloud Service v8 si connette direttamente con Adobe Experience Platform e permette agli utenti di sfruttare pienamente i propri dati e fornire campagne personalizzate e di impatto su tutti i canali.
* **Interfaccia utente ed esperienza coerenti**: la transizione a Managed Cloud Services v8 non interferisce con i flussi di lavoro. L’utente ritrova la stessa interfaccia ed esperienza utente che conosce già e la curva di apprendimento per i team è davvero minima.

**Se usi già Campaign Standard e stai passando a Campaign v8, [questo documento](../../adoption/home.md) spiega come iniziare.**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funzionalità principali {#key-features}

Gli utenti di Campaign v8, hanno accesso sia alla nuova interfaccia di Campaign Web che alla console v8. I dati e le impostazioni vengono sincronizzati tra i due ambienti. Tutti i dati e le impostazioni disponibili nella console client sono visibili nell’interfaccia utente di Campaign Web, accessibile dal menu di navigazione a sinistra di Explorer. [Ulteriori informazioni](../get-started/user-interface.md#user-interface-explorer)

L’interfaccia utente di Campaign Web è progettata per consentire ai marketer di creare e orchestrare facilmente le campagne. Le funzionalità principali dell’interfaccia utente di Campaign v8 Web includono:

* **Esperienza moderna, intuitiva e unificata**. [Ulteriori informazioni](../get-started/connect-to-campaign.md).
* **Nuove potenti funzionalità e processi fluidi**. [Ulteriori informazioni](../get-started/user-interface.md).
* **Query modeler semplificato e intuitivo**. [Ulteriori informazioni](../query/query-modeler-overview.md).
* **Funzionalità incorporate per la gestione delle campagne cross-channel**. [Ulteriori informazioni](../msg/gs-messages.md).
* **Attività riprogettate per i flussi di lavoro delle campagne**. [Ulteriori informazioni](../workflows/gs-workflows.md).
* **Facile creazione e gestione dei profili**. [Ulteriori informazioni](../audience/about-recipients.md).
* **Filtri preimpostati**. [Ulteriori informazioni](../get-started/predefined-filters.md).
* **Convertitore HTML per la progettazione delle e-mail**. [Ulteriori informazioni](../email/existing-content.md).
* **SMS con offerte**. [Ulteriori informazioni](../msg/offers.md).

La console client di Campaign è progettata per consentire ad amministratori e sviluppatori di configurare e personalizzare il proprio ambiente. Le funzionalità chiave disponibili nella console client di Campaign sono descritte in dettaglio in [questa documentazione](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Per ulteriori informazioni sulle funzionalità supportate e non supportate e sull’interoperabilità tra l’interfaccia utente di Campaign Web e la console client di Campaign, consulta [questa pagina](../get-started/capability-matrix.md).

## Terminologia {#terminology}

Tra Campaign v8 e Campaign Standard la maggior parte dei concetti è simile. Tuttavia, ci sono alcune differenze di terminologia. Alcuni esempi:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Funzionalità specifiche {#new-features}

Per garantire una transizione fluida a Campaign v8, le principali funzionalità di Campaign Standard sono state aggiunte a Campaign v8. Queste funzioni sono descritte nei dettagli in [questa documentazione](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it){target=_blank} e sono disponibili solo per gli utenti che stanno effettuando la transizione da Campaign Standard.

* **Reporting dinamico**: il reporting dinamico fornisce rapporti personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Include l’accesso ai dati di profilo per l’analisi demografica in base alle dimensioni, come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. [Ulteriori informazioni](../reporting/dynamic-reporting/get-started-reporting.md).

* **Branding centralizzato**: Adobe Campaign consente alle aziende di definire linee guida visive e tecniche per il brand. Gli utenti possono presentare alla clientela un brand coerente, dai loghi agli aspetti tecnici come il mittente dell’e-mail, l’URL o i domini. [Ulteriori informazioni](../administration/branding/branding-gs.md).

* **API REST**: gli utenti che hanno effettuato la migrazione a Campaign Standard possono utilizzare le API REST per creare integrazioni per Adobe Campaign e creare ecosistemi integrando Adobe Campaign con altre tecnologie. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.

* **Pagine di destinazione**: le pagine di destinazione di Campaign v8 includono miglioramenti per garantire la parità delle funzioni con Campaign Standard. Per ulteriori informazioni, consulta le [note sulla versione](../rn/release-notes.md#new-24-4) e la pagina di destinazione della [documentazione](../landing-pages/get-started-lp.md).

* **Frammenti visivi**: i frammenti visivi sono componenti visivi riutilizzabili a cui è possibile fare riferimento in una o più consegne e-mail o in modelli di contenuto. Modificando un frammento, viene aggiornato tutto il contenuto che lo utilizza. Questa funzionalità consente agli utenti di marketing di precreare più blocchi di contenuto personalizzati per l’assemblaggio rapido dei messaggi in un processo di progettazione migliorato. [Ulteriori informazioni](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->