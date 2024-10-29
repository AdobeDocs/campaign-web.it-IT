---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione di ottobre {#24-10-release}

**Data di rilascio**: 29 ottobre 2024

Le seguenti funzioni e miglioramenti sono disponibili a partire dalla versione di ottobre.

### Funzioni

<table>
<thead>
<tr>
<th><strong>Account esterni</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi impostare e gestire account esterni direttamente tramite l’interfaccia utente web di Adobe Campaign. Questa nuova funzione semplifica la configurazione di diversi tipi di account esterni, ad esempio e-mail non recapitate (POP3) o istanze di esecuzione.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/external-account.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Messaggistica transazionale</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi creare e monitorare i messaggi transazionali nell’interfaccia utente di Campaign Web. La messaggistica transazionale è un modulo specializzato in Adobe Campaign progettato per gestire i messaggi attivati. Questi messaggi vengono generati automaticamente in risposta a eventi provenienti da sistemi di informazione. Esempi comuni di tali eventi includono clic su pulsanti o collegamenti, abbandono del carrello, richiesta di avvisi sulla disponibilità del prodotto, creazione o modifica dell’account, ecc.</p>
<p>Per ulteriori informazioni, consulta la <a href="../transactional-messaging/transactional.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Miglioramenti

* **Attività del flusso di lavoro** - È ora possibile spostare un&#39;attività e tutti i relativi nodi secondari da una transizione a un&#39;altra all&#39;interno di un flusso di lavoro. Per eseguire questa operazione, nel riquadro delle proprietà dell&#39;attività è disponibile un pulsante **Sposta** dedicato. [Ulteriori informazioni](../workflows/orchestrate-activities.md#move)

* **Attività arricchimento flusso di lavoro**

   * È ora possibile definire un alias e un&#39;etichetta durante la creazione di un nuovo campo nell&#39;attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md#collection-settings)
   * È ora possibile aggiungere offerte per ogni profilo nell&#39;attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md##add-offers)

* **Distribuzione dei valori**: accedendo all’elenco dei campi per la personalizzazione, ora è possibile controllare come vengono distribuiti i valori per ciascun campo. Finestra popup dedicata che mostra il numero e la percentuale per ciascun valore. [Ulteriori informazioni](../query/build-query.md#distribution-values-query)


## Aggiornamenti di settembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Accelerazione dei contenuti dell’Assistente IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Dopo aver creato e personalizzato il messaggio, portalo al livello successivo con l’AI Assistant Content Accelerator in Adobe Campaign Web. Questo potente strumento consente di ottimizzare l’impatto dei contenuti generando una serie di testi coinvolgenti, titoli principali e immagini visivamente accattivanti.</p>
<p>Immergiti in un’esperienza pratica con <a href="https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator">la nostra anteprima delle funzionalità live</a>, progettata per consentirti di esplorarne le funzionalità in prima persona e comprenderne appieno le funzionalità.</a>.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/generative-gs.md">documentazione dettagliata</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Data di disponibilità: 12 settembre</p>
</td>
</tr>
</tbody>
</table>

## Versione di agosto {#24-8-release}

**Data di rilascio**: 3 settembre 2024

Le funzioni e i miglioramenti seguenti sono disponibili a partire dalla versione di agosto.

* **Parametri SMTP**: le impostazioni SMTP sono ora disponibili nelle impostazioni di consegna e-mail. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#smtp)

* **Variabili globali**: è ora possibile definire le variabili globali per stabilire i valori per le consegne. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuove funzioni in Disponibilità limitata {#acs-24-8}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Ciò significa che sono limitate a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuite in nessun altro ambiente.
>
>Consulta le seguenti pagine della documentazione: [Transizione da Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it){target="_blank"}.

* **Branding per direct mail**: gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull’identità del brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. I brand ora possono essere creati e collegati a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. [Ulteriori informazioni](https://experienceleague.adobe.com/it/docs/experience-cloud/campaign/branding/branding-assign)

* **Abbonamenti con pagine di destinazione**: è ora possibile collegare una pagina di destinazione a un servizio e inviare un messaggio di conferma quando gli utenti lo convalidano. [Ulteriori informazioni](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Frammenti visivi**: è ora possibile archiviare i frammenti di contenuti visivi. [Ulteriori informazioni](../content/create-fragment.md#archive)

* **Captcha nelle pagine di destinazione**: ora è possibile aggiungere Captcha per proteggere la pagina di destinazione dallo spam e dagli abusi causati dai bot. Ciò non è intrusivo per la clientela in quanto non richiede alcuna interazione da parte loro e si basa sulle interazioni con il sito. [Ulteriori informazioni](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
