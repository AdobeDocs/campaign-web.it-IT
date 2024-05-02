---
audience: end-user
title: Transizione da Campaign Standard ad Adobe Campaign Web
description: Scopri l’interfaccia utente web di Campaign
source-git-commit: 4c1f68f0e89b2b84b8845b2759ef3b0dc9b12033
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 7%

---


# Transizione di Campaign Standard a Campaign v8{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Benvenuti in Adobe Campaign Managed Cloud Services v8!

Siamo entusiasti di annunciare che gli utenti di Adobe Campaign Standard ora possono effettuare la transizione a Adobe Campaign Managed Cloud Services v8. Questa transizione offre molti vantaggi:

* Solida infrastruttura IT: con Managed Cloud Service v8, i client possono sfruttare un&#39;infrastruttura IT più solida, garantendo prestazioni, affidabilità e scalabilità migliorate per le loro campagne.
* Supporto avanzato: il nostro team di Cloud Service gestiti si impegna a fornire assistenza di alto livello per garantire una transizione fluida e un monitoraggio continuo della piattaforma. Dalla risoluzione dei problemi alla manutenzione proattiva, tutto è a tua disposizione.
* Integrazione con Adobe Experience Platform: Managed Cloud Service v8 si connette direttamente con Adobe Experience Platform, consentendo ai client di sfruttare appieno il potenziale dei propri dati e di fornire campagne personalizzate e di impatto su tutti i canali.
* Interfaccia utente ed esperienza coerenti: la transizione a Cloud Service gestiti v8 non interrompe il flusso di lavoro. Continuerai a godere dell’interfaccia utente familiare e dell’esperienza utente, garantendo al tuo team una curva di apprendimento minima.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funzionalità principali {#key-features}

Approfondiamo le funzionalità chiave di Campaign v8:

* Esperienza moderna, amichevole e unificata. [Ulteriori informazioni](../get-started/connect-to-campaign.md).
* Nuove potenti funzionalità e processi senza soluzione di continuità. [Ulteriori informazioni](../get-started/user-interface.md)
* Nuovo modello di query semplificato e intuitivo. [Ulteriori informazioni](../query/query-modeler-overview.md)
* Funzionalità integrate di gestione delle campagne cross-channel. [Ulteriori informazioni](../msg/gs-messages.md)
* Attività del flusso di lavoro delle campagne nuove e riprogettate. [Ulteriori informazioni](../workflows/gs-workflows.md)
* Pubblico di destinazione con il modellatore di query. [Ulteriori informazioni](../query/query-modeler-overview.md)
* Facile creazione e gestione dei profili. [Ulteriori informazioni](../audience/about-recipients.md)
* Guida contestuale basata sull’intelligenza artificiale. [Ulteriori informazioni](../get-started/using-ai.md)
* Filtri predefiniti. [Ulteriori informazioni](../get-started/predefined-filters.md)
* HTML Converter per la progettazione di e-mail. [Ulteriori informazioni](../email/existing-content.md)
* SMS con offerte. [Ulteriori informazioni](../msg/offers.md)

## Console e interfaccia web {#console}

In qualità di utente di Campaign v8, potrai accedere sia alla nuova interfaccia web di Campaign che alla console v8. I dati e le impostazioni vengono sincronizzati da un ambiente all’altro. Tutti i dati e le impostazioni disponibili nella console client sono visibili nell’interfaccia utente di Campaign Web, dal menu di navigazione a sinistra di Explorer. [Ulteriori informazioni](../get-started/user-interface.md#user-interface-explorer)

Funzionalità supportate e non supportate e interoperabilità tra l’interfaccia utente di Campaign Web e la console client di Campaign [in questa pagina](../get-started/capability-matrix.md)

## Terminologia {#terminology}

La maggior parte dei concetti è simile nell’interfaccia web di Campaign e in Campaign Standard. Tuttavia, ci sono alcune differenze. Di seguito sono riportati alcuni esempi di differenze terminologiche tra Campaign Standard e l’interfaccia web di Campaign:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Le risorse personalizzate sono **Schemi** nell’interfaccia utente di Campaign Web.
* Le attività di marketing non esistono più.
* I messaggi sono **Consegne**.
* Gli operatori sono **Utenti**.
* I diritti denominati sono **Ruoli**.
* I gruppi di operatori sono **Gruppi di sicurezza**.
* Le autorizzazioni per le cartelle sono **Unità organizzative**

## Nuove funzioni {#new-features}

Per poter effettuare la transizione, abbiamo aggiunto [funzionalità principali](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) da Campaign Standard a v8:

* **Reporting dinamico**: il reporting dinamico fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Aggiunge l’accesso ai dati del profilo, consentendo l’analisi demografica per dimensioni di profilo come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Branding centralizzato**: ogni azienda dispone di linee guida visive e tecniche per il brand. Con Adobe Campaign, puoi definire una serie di specifiche per presentare ai clienti un brand coerente, dai loghi agli aspetti tecnici, come il mittente dell’e-mail, l’URL o i domini. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **API REST** - In qualità di utente di Campaign Standard migrato, puoi utilizzare le API Rest per creare integrazioni per Adobe Campaign e creare il tuo ecosistema interfacciando Adobe Campaign con il pannello di tecnologie utilizzato. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Pagine di destinazione** - Sono stati apportati molti miglioramenti a Campaign v8 per assicurarti di non perdere alcuna funzionalità. Per ulteriori informazioni, consulta [note sulla versione](../rn/release-notes.md#new-24-4) e la pagina di destinazione [documentazione](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->