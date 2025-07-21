---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 98%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti introdotti nelle versioni precedenti sono elencati nel [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Aggiornamenti di luglio 2025 {#25-7-updates}

>[!AVAILABILITY]
>
>Per usufruire di questi aggiornamenti, il server deve essere aggiornato almeno alla versione 8.8.1. Consulta le [note sulla versione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it){target="_blank"} della console client.

Precedentemente rilasciate in Disponibilità limitata, le seguenti funzionalità sono ora disponibili per tutti gli ambienti (Disponibilità generale):

* **Creazione di consegne multilingue**: nell’interfaccia utente di Adobe Campaign Web ora puoi inviare più consegne di e-mail in lingue diverse. La funzione Consegna multilingue consente di scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare l’anteprima di queste consegne nelle lingue scelte. [Ulteriori informazioni](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}
-->

* **Avvisi sulle consegne**: la funzione avvisi sulle consegne è un sistema di gestione degli avvisi che consente a un gruppo di utenti di ricevere automaticamente le notifiche contenenti informazioni sull’esecuzione delle consegne. [Ulteriori informazioni](../msg/delivery-alerting.md)

* **Miglioramenti alle pagine di destinazione**: sono ora disponibili i seguenti miglioramenti alle pagine di destinazione:

   * Ora, al momento della configurazione di un servizio, puoi fare riferimento a una pagina di destinazione predefinita per l’iscrizione o l’annullamento dell’iscrizione. Durante la progettazione di un’e-mail, se definisci un collegamento a tale pagina di destinazione, quando gli utenti inviano il modulo presente sulla pagina di destinazione, viene eseguitp automaticamente l’abbonamento o l’annullamento dell’abbonamento a tale servizio. [Ulteriori informazioni](../audience/manage-services.md#create-service)
   * Una nuova opzione nella configurazione della pagina di destinazione consente l’accesso ai visitatori anonimi. Se questa opzione è deselezionata, solo gli utenti identificati potranno accedere al modulo e inviarlo. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione nella configurazione della pagina di destinazione consente di memorizzare dati interni aggiuntivi durante il suo invio. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione consente di utilizzare una pagina di destinazione per diversi servizi, rendendola dinamica. Quando aggiungi un collegamento a un’e-mail, se selezioni una pagina di destinazione dinamica puoi selezionare qualsiasi servizio. Se selezioni una pagina di destinazione a cui è associato un servizio specifico, questo servizio verrà utilizzato automaticamente (non è possibile selezionarne un altro). [Ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ora le pagine di destinazione supportano i contenuti condizionali. [Ulteriori informazioni](../landing-pages/lp-content.md)
   * È ora possibile collegare una pagina di destinazione a un servizio e inviare un messaggio di conferma quando gli utenti lo convalidano. [Ulteriori informazioni](../landing-pages/lp-content.md#lp-message)
   * Ora è possibile aggiungere Captcha per proteggere la pagina di destinazione dallo spam e dagli abusi causati dai bot. Ciò non è intrusivo per la clientela in quanto non richiede alcuna interazione da parte loro e si basa sulle interazioni con il sito. [Ulteriori informazioni](../landing-pages/create-lp.md#captcha)

Precedentemente rilasciate in Disponibilità limitata, le seguenti funzionalità sono ora disponibili **on-demand**:

* **Reporting dinamico**: ora è possibile accedere al reporting dinamico, che fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Consente di accedere ai dati del profilo, abilitando l’analisi demografica per dimensioni di profilo, come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. Il reporting dinamico è disponibile anche per le consegne e-mail e i messaggi transazionali multilingue. [Ulteriori informazioni](../reporting/dynamic-reporting/get-started-reporting.md)

* **Branding centralizzato**: gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull’identità del brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. Puoi creare questi brand e collegarli a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. Le opzioni di branding sono ora disponibili per tutti i canali, inclusi SMS e direct mail. [Ulteriori informazioni](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Questa funzione è disponibile solo per nuove implementazioni.

Oltre alle funzioni elencate in precedenza, questa versione include anche una serie di funzionalità disponibili nella console client:

* [Nuovo connettore di invio SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=it). (Ambienti FDA)
* [API REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=it) (su richiesta, ambienti FDA)

Consulta le [note sulla versione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it){target="_blank"} della console client.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->