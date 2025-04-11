---
audience: end-user
title: Passaggio da Campaign Standard ad Adobe Campaign Web
description: Interfaccia utente di Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Passaggio da Campaign Standard a Campaign v8 {#acs-to-ac}

Gli utenti di Adobe Campaign Standard ora possono effettuare la transizione a Adobe Campaign Managed Cloud Services v8. Questa transizione offre diversi vantaggi:

* **Solida infrastruttura IT**: Managed Cloud Services v8 fornisce un&#39;infrastruttura IT più solida, garantendo prestazioni, affidabilità e scalabilità migliorate per le campagne.
* **Supporto avanzato**: il team Managed Cloud Services offre assistenza di alto livello per garantire una transizione senza intoppi e un monitoraggio continuo della piattaforma. Il supporto include la risoluzione dei problemi e la manutenzione proattiva.
* **Integrazione con Adobe Experience Platform**: Managed Cloud Services v8 si connette perfettamente con Adobe Experience Platform, consentendo agli utenti di sfruttare appieno i propri dati e di distribuire campagne personalizzate e di impatto tra i canali.
* **Interfaccia utente ed esperienza coerenti**: la transizione a Managed Cloud Services v8 non interrompe i flussi di lavoro. Gli utenti continuano a godere dell’interfaccia e dell’esperienza familiari, riducendo al minimo la curva di apprendimento per i team.

**In qualità di utente di Campaign Standard che passa a Campaign v8, scopri come iniziare [in questo documento](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funzionalità principali {#key-features}

Gli utenti di Campaign v8 possono accedere sia alla nuova interfaccia web di Campaign che alla console v8. I dati e le impostazioni vengono sincronizzati tra gli ambienti. Tutti i dati e le impostazioni disponibili nella console client sono visibili nell’interfaccia utente di Campaign Web, accessibile dal menu di navigazione a sinistra di Explorer. [Ulteriori informazioni](../get-started/user-interface.md#user-interface-explorer)

L’interfaccia utente di Campaign Web è progettata per consentire agli addetti al marketing di creare e orchestrare facilmente campagne. Le funzionalità principali dell’interfaccia utente di Campaign v8 Web includono:

* **Esperienza moderna, amichevole e unificata**. [Ulteriori informazioni](../get-started/connect-to-campaign.md).
* **Nuove potenti funzionalità e processi senza soluzione di continuità**. [Ulteriori informazioni](../get-started/user-interface.md).
* **Modellatore di query semplificato e intuitivo**. [Ulteriori informazioni](../query/query-modeler-overview.md).
* **Funzionalità integrate di gestione campagne cross-channel**. [Ulteriori informazioni](../msg/gs-messages.md).
* **Attività flusso di lavoro campagna riprogettate**. [Ulteriori informazioni](../workflows/gs-workflows.md).
* **Facile creazione e gestione dei profili**. [Ulteriori informazioni](../audience/about-recipients.md).
* **Filtri predefiniti**. [Ulteriori informazioni](../get-started/predefined-filters.md).
* **Convertitore HTML per progettazione e-mail**. [Ulteriori informazioni](../email/existing-content.md).
* **SMS con offerte**. [Ulteriori informazioni](../msg/offers.md).

La console client di Campaign è progettata per consentire ad amministratori e sviluppatori di configurare e personalizzare il proprio ambiente. Le funzionalità chiave disponibili nella console client di Campaign sono descritte in dettaglio in [questa documentazione](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Ulteriori informazioni sulle funzionalità supportate e non supportate e sull&#39;interoperabilità tra l&#39;interfaccia utente di Campaign Web e la console client di Campaign [in questa pagina](../get-started/capability-matrix.md).

## Terminologia {#terminology}

Tra Campaign v8 e Campaign Standard la maggior parte dei concetti è simile. Tuttavia, esistono alcune differenze terminologiche. Alcuni esempi:

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

Per garantire una transizione fluida a Campaign v8, a Campaign v8 sono state aggiunte le funzionalità principali di Campaign Standard. Queste funzionalità sono descritte in dettaglio nella [documentazione](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it){target="_blank} e sono disponibili solo per gli utenti che passano da Campaign Standard.

* **Reporting dinamico**: Reporting dinamico fornisce report personalizzabili in tempo reale per misurare l&#39;impatto delle attività di marketing. Include l’accesso ai dati del profilo per l’analisi demografica per dimensioni come genere, città ed età, insieme ai dati funzionali delle campagne e-mail come aperture e clic. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=it){target="_blank"}.

* **Branding centralizzato**: Adobe Campaign consente alle aziende di definire linee guida visive e tecniche per il brand. Gli utenti possono presentare ai clienti un brand coerente, dai loghi agli aspetti tecnici come il mittente dell’e-mail, l’URL o i domini. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=it).

* **API REST**: gli utenti migrati da Campaign Standard possono utilizzare le API REST per creare integrazioni per Adobe Campaign e creare ecosistemi interfacciando Adobe Campaign con altre tecnologie. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=it){target="_blank"}.

* **Pagine di destinazione**: le pagine di destinazione di Campaign v8 includono miglioramenti per garantire la parità di funzionalità con Campaign Standard. Per ulteriori informazioni, consulta le [note sulla versione](../rn/release-notes.md#new-24-4) e la pagina di destinazione della [documentazione](../landing-pages/get-started-lp.md).

* **Frammenti visivi**: i frammenti visivi sono componenti visivi riutilizzabili a cui si fa riferimento in una o più consegne e-mail o modelli di contenuto. La modifica di un frammento aggiorna tutto il contenuto che lo utilizza. Questa funzionalità consente agli utenti di marketing di precreare più blocchi di contenuto personalizzati per l’assemblaggio rapido dei messaggi in un processo di progettazione migliorato. [Ulteriori informazioni](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->