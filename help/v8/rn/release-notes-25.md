---
title: Note sulla versione precedente dell’interfaccia utente di Campaign Web v8
description: Versioni 2025 dell’interfaccia utente di Campaign Web
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 875e60defa2d96a6d7b3663516b757f3cc8cd154
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 100%

---

# Note sulle versioni 2025 {#2025-release}

In questa pagina sono elencate tutte le modifiche e i miglioramenti disponibili con le **versioni 2025**. Le note più recenti sulla versione sono disponibili in [questa pagina](release-notes.md).

## Versione di luglio 2025 {#25-7-release}

### Nuove funzioni {#25-7-features}

Le seguenti funzioni sono disponibili a partire dalla versione di luglio.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Supporto di CSS personalizzati in E-mail designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Durante la progettazione delle e-mail, ora è possibile aggiungere CSS personalizzati direttamente in E-mail designer. Questa funzionalità consente di applicare uno stile avanzato e specifico, per una maggiore flessibilità e controllo sull’aspetto del contenuto.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/custom-css.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Brand</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora è possibile creare e personalizzare i brand per definire chiaramente la propria identità visiva e verbale nelle comunicazioni. Con il punteggio di allineamento del brand, è possibile ricevere feedback in tempo reale su come il il contenuto ne rifletta il tono, lo stile e le linee guida, consentendo di rimanere coerente in ogni messaggio inviato.
</p>
<p>Per ulteriori informazioni, consulta la <a href="../content/brands.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Avvisi di consegna</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La funzione Avvisi di consegna è un sistema di gestione degli avvisi che consente a un gruppo di utenti di ricevere automaticamente le notifiche contenenti informazioni sull’esecuzione delle consegne.</p>
<p>Per ulteriori informazioni, consulta la <a href="../msg/delivery-alerting.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Reporting dinamico</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora è possibile accedere al reporting dinamico, che fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Consente di accedere ai dati del profilo, abilitando l’analisi demografica per dimensioni di profilo, come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. Il reporting dinamico è disponibile anche per le consegne e-mail e i messaggi transazionali multilingue.</p>
<p>Questa funzionalità è disponibile solo on-demand. Per ottenere l’accesso, contatta il tuo rappresentante Adobe. Il server deve essere aggiornato almeno alla versione 8.8.1. Consulta le <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it-IT" target="_blank">note sulla versione</a> della console client.
<p>Per ulteriori informazioni, consulta la <a href="../reporting/dynamic-reporting/get-started-reporting.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Branding centralizzato</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull’identità del brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. Puoi creare questi brand e collegarli a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. Le opzioni di branding sono ora disponibili per tutti i canali, inclusi SMS e direct mail.</p>
<p>Questa funzione è disponibile solo on-demand, per nuove implementazioni. Per ottenere l’accesso, contatta il tuo rappresentante Adobe. Il server deve essere aggiornato almeno alla versione 8.8.1. Consulta le <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it-IT" target="_blank">note sulla versione</a> della console client.
<p>Per ulteriori informazioni, consulta la <a href="../administration/branding/branding-gs.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

Oltre alle funzioni elencate in precedenza, questa versione include anche una serie di funzionalità disponibili nella console client:

* [Nuovo connettore di invio SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=it) (ambienti FDA)
* [API REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=it) (on-demand, ambienti FDA)

Consulta le [note sulla versione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it-IT){target="_blank"} della console client.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

-->

### Miglioramenti {#25-7-improvements}

* Ora puoi calcolare la popolazione target direttamente per ciascuna condizione e gruppo nel generatore di regole. Fai clic sul numero del risultato per visualizzare l’elenco dettagliato dei record. [Ulteriori informazioni](../query/build-query.md#validate-query)

* Ora puoi modificare o eliminare un filtro predefinito direttamente dal generatore di regole. [Ulteriori informazioni](../get-started/predefined-filters.md#manage-predefined-filter)

* Durante la configurazione di una consegna SMS, nella sezione **SMS** ora puoi accedere ai **parametri SMPP facoltativi (TLV)**. Questo parametro è lo stesso della console client. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#sms-tab)

* Ora puoi abilitare le notifiche in background su iOS utilizzando la nuova opzione **Contenuto disponibile**, che si trova nella sezione **Impostazioni avanzate** della schermata di modifica dei contenuti di iOS. Questo aggiunge il flag `content-available:1` nel payload `aps`. Ulteriori informazioni sono disponibili [in questa pagina](../push/content-push.md). Consulta anche [questa pagina](../push/rich-push-ios.md).

* Sono ora disponibili i seguenti miglioramenti alla pagina di destinazione:

   * Ora, al momento della configurazione di un servizio, puoi fare riferimento a una pagina di destinazione predefinita per l’iscrizione o l’annullamento dell’iscrizione. Durante la progettazione di un’e-mail, se definisci un collegamento a tale pagina di destinazione, quando gli utenti inviano il modulo presente sulla pagina di destinazione, viene eseguitp automaticamente l’abbonamento o l’annullamento dell’abbonamento a tale servizio. [Ulteriori informazioni](../audience/manage-services.md#create-service)
   * Una nuova opzione nella configurazione della pagina di destinazione consente l’accesso ai visitatori anonimi. Se questa opzione è deselezionata, solo gli utenti identificati potranno accedere al modulo e inviarlo. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione nella configurazione della pagina di destinazione consente di memorizzare dati interni aggiuntivi durante il suo invio. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione consente di utilizzare una pagina di destinazione per diversi servizi, rendendola dinamica. Quando aggiungi un collegamento a un’e-mail, se selezioni una pagina di destinazione dinamica puoi selezionare qualsiasi servizio. Se selezioni una pagina di destinazione a cui è associato un servizio specifico, questo servizio verrà utilizzato automaticamente (non è possibile selezionarne un altro). [Ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ora le pagine di destinazione supportano i contenuti condizionali. [Ulteriori informazioni](../landing-pages/lp-content.md)
   * È ora possibile collegare una pagina di destinazione a un servizio e inviare un messaggio di conferma quando gli utenti lo convalidano. [Ulteriori informazioni](../landing-pages/lp-content.md#lp-message)
   * Ora è possibile aggiungere Captcha per proteggere la pagina di destinazione dallo spam e dagli abusi causati dai bot. Ciò non è intrusivo per la clientela in quanto non richiede alcuna interazione da parte loro e si basa sulle interazioni con il sito. [Ulteriori informazioni](../landing-pages/create-lp.md#captcha)

## Versione di giugno 2025 {#25-6-release}

### Miglioramenti {#25-6-improvements}

* Il rapporto Riepilogo delle consegne è ora disponibile sia per il canale call center che per quelli personalizzati. [Ulteriori informazioni](../reporting/direct-mail.md)

* Durante la configurazione di una consegna SMS, ora puoi accedere a parametri SMS specifici. Questi sono gli stessi parametri disponibili nella console client. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#sms-tab)

* Le cartelle preferite vengono ora visualizzate nella parte superiore del pannello a sinistra nella pagina di Explorer, semplificandone l’accesso. [Ulteriori informazioni](../get-started/work-with-folders.md#favorite-folders)

* Il Generatore di regole ora supporta il trascinamento della selezione, che consente di ridisporre i componenti della query in modo più efficiente. [Ulteriori informazioni](../query/build-query.md#drag-and-drop)

* La “condizione umana” nel Generatore di regole è stata migliorata. Questa è la versione delle regole scritta in linguaggio semplice e mostrata nella parte inferiore dello schermo:

   * Gli attributi vengono ora evidenziati e viene visualizzato lo schema associato.
   * Puoi fare clic su questi elementi per visualizzare informazioni più dettagliate.
   * Ora puoi copiare la condizione umana utilizzando il pulsante corrispondente.

* L’accesso alle cartelle “Flussi di lavoro tecnici” e “Oggetti creati automaticamente” è ora limitato per impedirne la visualizzazione. [Ulteriori informazioni](../get-started/work-with-folders.md#about-folders)

## Versione di maggio 2025 {#25-5-release}

Le seguenti funzioni sono disponibili per tutti gli utenti a partire dalla versione di maggio.

<table>
<thead>
<tr>
<th><strong>Punteggio di allineamento del brand (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La funzione di punteggio di allineamento del brand offre un feedback chiaro direttamente nell’E-mail designer, consentendoti di visualizzare se il contenuto è allineato al tono, allo stile e alle linee guida del brand. Questa funzione è disponibile in versione Beta.</p>
<p>Per ulteriori informazioni, consulta la <a href="../content/brands-score.md">documentazione dettagliata</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Canale personalizzato per consegne esterne</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi orchestrare ed eseguire le consegne direttamente dall’interfaccia utente web di Adobe Campaign in base a canali esterni personalizzati. Queste consegne possono essere autonome o far parte di un flusso di lavoro. La creazione del canale esterno personalizzato integrato con una terza parte viene eseguita nella console.</p>
<p>Nota: le funzioni di reporting non sono disponibili nell’interfaccia utente web per il canale personalizzato. Per accedere ai rapporti, devi passare alla console client.</p>
<p>Per ulteriori informazioni, consulta la <a href="../call-center/gs-custom-channel.md">documentazione dettagliata</a>.</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#25-5-improvements}

La schermata di creazione delle regole di tipologia è stata aggiornata per facilitare la selezione del tipo di regola.

## Versione di aprile 2025 {#25-4-release}

**Data di rilascio**: 29 aprile 2025

### Nuove funzioni {#25-4-features}

Le seguenti funzioni sono disponibili per tutti gli utenti a partire dalla versione di aprile.

<table>
<thead>
<tr>
<th><strong>Canale call center</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Il canale call center è ora disponibile nell’interfaccia utente di Campaign Web. Questo canale si riferisce a un metodo di comunicazione utilizzato per gestire e tracciare comunicazioni o interazioni gestite tramite un call center, in genere le chiamate telefoniche effettuate dagli agenti a clienti o a potenziali clienti.</p>
<p>Nota: le funzioni di reporting non sono disponibili nell’interfaccia utente web per il canale call center. Per accedere ai rapporti, devi passare alla console client.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Per ulteriori informazioni, consulta la <a href="../call-center/gs-call-center.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nuovo generatore di regole</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora disponibile un nuovo generatore di regole che consente di definire condizioni complesse in un’interfaccia utente migliorata. Se necessario, puoi passare dal generatore di regole precedente a quello nuovo.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Per ulteriori informazioni, consulta la <a href="../query/query-modeler-overview.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Authoring di account esterni</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>In qualità di amministratore di Campaign, ora puoi impostare nuove connessioni con sistemi esterni dall’interfaccia utente di Campaign Web.
Puoi anche visualizzare, aggiornare e gestire gli account esterni esistenti.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/external-account.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#25-4-improvements}

**Miglioramenti generali all’interfaccia**

* Le opzioni Descrizione campo, Aggiungi ai preferiti e Distribuzione dei valori per gli attributi dello schema sono ora più visibili nell’interfaccia utente. Per ulteriori informazioni, consulta la [documentazione dettagliata](../get-started/attributes.md).
* Nell’interfaccia, la data e l’ora vengono ora visualizzate in base alla lingua principale impostata nelle preferenze di Experience League. Questo miglioramento è disponibile solo per alcune lingue. Per visualizzare l’elenco completo delle lingue supportate, consulta la [documentazione dettagliata](https://experienceleague.adobe.com/it/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor e-mail**: per migliorare l’accessibilità nell’interfaccia utente di Campaign Web, sono ora disponibili due nuovi campi nell’E-mail designer: corrispondono all’`title`elemento e all’attributo lang nell’`html`elemento del contenuto dell’e-mail. Nella sezione del corpo dell’e-mail, oltre al campo Preintestazione, puoi definire queste impostazioni. Per ulteriori informazioni, consulta la [documentazione dettagliata](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemi**

* Ora puoi modificare lo schema temporaneo di un elenco dall’interfaccia utente di Campaign Web. Per ulteriori informazioni, consulta la [documentazione dettagliata](../audience/manage-audience.md).
* Ora puoi visualizzare in anteprima i campi personalizzati di uno schema in una schermata di esempio. Per ulteriori informazioni, consulta la [documentazione dettagliata](../administration/custom-fields.md#add).
* Ora puoi spostare i campi personalizzati nell’elenco tramite il trascinamento. Per ulteriori informazioni, consulta la [documentazione dettagliata](../administration/custom-fields.md#add).


### Nuove funzioni in Disponibilità limitata {#25-4-features-la}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Ciò significa che sono limitate a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuite in nessun altro ambiente. Richiedono un aggiornamento del server Campaign alla versione v8.7.4.
>
>Consulta le seguenti pagine della documentazione: [Transizione da Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it).

* **Creazione di consegne multilingue**: nell’interfaccia utente di Adobe Campaign Web ora puoi inviare più consegne di e-mail in lingue diverse. La funzione Consegna multilingue consente di scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare l’anteprima di queste consegne nelle lingue scelte. Per ulteriori informazioni, consulta la [documentazione dettagliata](../email/edit-content.md).

* **Reporting dinamico per multilingue**: il reporting dinamico è ora disponibile per le consegne di e-mail multilingue. Per ulteriori informazioni, consulta la [documentazione dettagliata](../reporting/global-reports.md).

* **Supporto API REST SMS (LA)**: l’API REST per la messaggistica transazionale è ora disponibile per il canale SMS. Quando nel payload sono presenti sia e-mail che telefono cellulare, puoi utilizzare il campo “wishedChannel” per specificare il canale. Se non viene fornito, l’e-mail verrà utilizzata per impostazione predefinita a meno che wishedChannel non richieda esplicitamente l’invio di SMS. Per ulteriori informazioni, consulta la [documentazione dettagliata](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=it){target=_blank}.

## Versione di febbraio 2025 {#25-2-release}

**Data di rilascio**: 18 febbraio 2025

Le funzioni e i miglioramenti seguenti sono disponibili a partire dalla versione di febbraio.

### Funzioni {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Creare regole di business (regole di tipologia)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora è possibile creare tipologie e regole di tipologia nell’interfaccia utente di Adobe Campaign Web. Le tipologie consentono di controllare, filtrare e definire le priorità per l’invio delle consegne. Consentono di convalidare che le consegne contengano sempre i componenti obbligatori (come un collegamento per l’annullamento dell’abbonamento o un oggetto), oppure regole di filtro per escludere determinati gruppi dal pubblico (ad esempio utenti che hanno annullato l’abbonamento, concorrenti o clientela non fidelizzata).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/typologies.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Mappature target</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile creare mappature target nell’interfaccia utente di Campaign Web. Le mappature target definiscono il collegamento tra i diversi canali di consegna (e-mail, SMS, notifiche push) e i campi dati di uno schema. La mappatura target consente di definire il pubblico target: profili, beneficiari di contratti, operatori, iscritti, potenziali clienti, ecc.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/target-mappings.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Dettagli degli schemi</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile accedere ai dettagli di uno schema selezionandone il nome nell’elenco. La modifica dei campi personalizzati è ora accessibile dal pulsante <b>Modifica campi personalizzati</b> disponibile nei dettagli dello schema.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/schemas.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

## Versione di gennaio 2025  {#25-1-release}

**Data di rilascio**: 5 febbraio 2025

Le funzioni e i miglioramenti seguenti sono disponibili a partire dalla versione di gennaio.

### Funzioni {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Creare e utilizzare frammenti visivi</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>I frammenti visivi sono blocchi visivi predefiniti che è possibile riutilizzare in più consegne e-mail o in modelli di contenuto. Questa funzione è ora disponibile per tutta la clientela per l’esecuzione di build sul server nella versione 8.6.4 e successive.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>Per ulteriori informazioni, consulta la <a href="../content/use-visual-fragments.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Utilizzare un sistema di terze parti per inviare le consegne</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile definire le consegne esterne e i modelli di consegna esterna nell’interfaccia Web di Campaign. In questa modalità, i messaggi vengono compilati in un file di output che può essere condiviso con il provider esterno. Per impostazione predefinita, la modalità di consegna esterna viene utilizzata per il canale direct mail.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Per ulteriori informazioni, consulta la <a href="../msg/send-external-deliveries.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gestire le enumerazioni</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile creare enumerazioni direttamente tramite l’interfaccia utente web di Adobe Campaign. Un’enumerazione è un elenco di valori suggeriti dal sistema per compilare i campi. Le enumerazioni possono essere utilizzate per standardizzare i valori di tali campi, aiutare con l’input di dati o l’uso all’interno delle query.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/enumerations.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creare opzioni personalizzate</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora è possibile accedere alle opzioni tecniche nell’interfaccia utente web di Adobe Campaign e creare opzioni personalizzate in base alle esigenze. Ciò è particolarmente utile quando si utilizzano attività del flusso di lavoro del codice JavaScript per memorizzare dati intermedi.</p>
<img src="assets/do-not-localize/options.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/options.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definire e chiamare i codici JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile creare codici JavaScript nell’interfaccia utente web di Adobe Campaign. Questo consente di creare funzioni riutilizzabili che possono essere impiegate in tutti i flussi di lavoro analogamente a una libreria.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>Per ulteriori informazioni, consulta la <a href="../administration/javascript-codes.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Generazione della pagina di destinazione con l’Assistente IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’Assistente IA è ora disponibile per le consegne di pagine di destinazione e consente di generare testo, immagini o layout di pagina completi.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Per ulteriori informazioni sull’Assistente IA, consulta la <a href="../email/generative-lp.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>


### Miglioramenti {#25-1-improvements}

* Personalizzazione della visualizzazione dei campi personalizzati nell’interfaccia:

   * Ora è possibile selezionare campi personalizzati aggiuntivi da visualizzare nell’interfaccia
   * È possibile impostare regole per la visualizzazione di campi personalizzati di tipo collegamento, ad esempio limitando i valori di elenco in base all’input di un altro campo
   * Ora è possibile disporre i campi nell’interfaccia in modo più flessibile: i campi possono estendersi su una singola colonna o essere raggruppati in sottosezioni per una migliore organizzazione
   * È ora possibile impostare campi specifici di sola lettura

* Filtri recenti e Preferiti: per riutilizzare rapidamente gli attributi impiegati di frequente, è ora possibile aggiungerli ai preferiti. In questo modo, sono facilmente accessibili per le attività future. Oltre ai preferiti, è possibile anche visualizzare e utilizzare gli attributi selezionati più di recente.

* Account esterni: quando si crea un nuovo account esterno, è possibile selezionare il nuovo tipo **[!UICONTROL Indirizzamento]**. Consente di configurare un account esterno specifico da utilizzare nelle consegne esterne. [Ulteriori informazioni](../administration/external-account.md#routing)
