---
title: Note sulla versione precedente dell’interfaccia utente di Campaign Web v8
description: Versioni 2024 dell’interfaccia utente di Campaign Web
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 19a7540af7502709b7eafdace038b5958e077173
workflow-type: tm+mt
source-wordcount: '2470'
ht-degree: 99%

---

# Note sulla versione 2024 {#2024-release}

In questa pagina sono elencate tutte le modifiche e i miglioramenti disponibili con le **versioni 2024**. Le note più recenti sulla versione sono disponibili in [questa pagina](release-notes.md).


## Versione di ottobre 2024 {#24-10-release}

**Data di rilascio**: 29 ottobre 2024

Le funzioni e i miglioramenti seguenti sono disponibili a partire dalla versione di ottobre.

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
<p>La messaggistica transazionale (Centro messaggi) è ora disponibile nell’interfaccia utente web di Campaign. Questo componente aggiuntivo è progettato per attivare messaggi generati da eventi attivati da sistemi informativi e può includere: fattura, conferma dell’ordine, conferma della spedizione, modifica della password, notifica di indisponibilità del prodotto, estratto conto, creazione di account del sito web, ecc.</p>
<p>Per ulteriori informazioni, consulta la <a href="../transactional-messaging/transactional.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>


### Miglioramenti

* **Attività dei flussi di lavoro** - È ora possibile spostare un’attività e tutti i relativi nodi secondari da una transizione a un&#39;altra all’interno di un flusso di lavoro. Per eseguire questa operazione, nel riquadro delle proprietà dell’attività è disponibile il pulsante dedicato **Sposta**. [Ulteriori informazioni](../workflows/orchestrate-activities.md#move)

* **Attività di arricchimento nei flussi di lavoro**

   * È ora possibile definire un alias e un’etichetta durante la creazione di un nuovo campo nell’attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md#collection-settings)
   * Ora è possibile aggiungere offerte per ogni profilo nell’attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md##add-offers)

* **Distribuzione dei valori**: accedendo all’elenco dei campi per la personalizzazione, ora è possibile controllare come vengono distribuiti i valori per ciascun campo. Finestra popup dedicata che mostra il numero e la percentuale per ciascun valore. [Ulteriori informazioni](../query/build-query.md#distribution-values-query)

* **Informazioni sulla versione e sul sistema** - Ora è possibile accedere ai dettagli delle versioni delle istanze, sia per la console client che per l’interfaccia utente web. In questa nuova sezione sono elencati anche tutti i pacchetti incorporati installati nell’ambiente. [Ulteriori informazioni](../get-started/user-interface.md#user-interface-about)

* **Elenchi** - Ora è possibile riordinare facilmente i valori di un elenco. [Ulteriori informazioni](../get-started/work-with-folders.md)

* **Consegna** - La variabile di consegna è ora accessibile dai campi di personalizzazione. [Ulteriori informazioni](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## Aggiornamenti di settembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Assistente IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Dopo aver creato e personalizzato il messaggio, passa a un livello successivo con l’Assistente AI in Adobe Campaign Web. Questo potente strumento consente di ottimizzare l’impatto dei contenuti generando una serie di testi coinvolgenti, titoli principali e immagini visivamente accattivanti.</p>
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
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=it){target="_blank"}.-->


## Note sulla versione di luglio {#24-7-release}

**Data di rilascio**: 30-31 luglio 2024

Le seguenti funzioni e i miglioramenti sono disponibili a partire dalla versione di luglio.

### Frammenti di contenuto {#24-7-1}

Ora puoi creare e utilizzare i frammenti di contenuto. Un frammento di contenuto è un componente riutilizzabile a cui è possibile fare riferimento in uno o più messaggi. Quando si modifica un frammento, viene aggiornato ogni contenuto che lo utilizza. Questa funzionalità consente di precreare più blocchi di contenuto personalizzati che possono essere utilizzati dagli utenti di marketing per assemblare rapidamente i contenuti dei messaggi in un processo di progettazione migliorato.

Sono disponibili due tipi di frammenti:

* I **frammenti di espressione** sono espressioni predefinite disponibili in una voce dedicata nell’editor di espressioni.
* I **frammenti visivi** sono blocchi visivi predefiniti che è possibile riutilizzare in più consegne e-mail o in modelli di contenuto. [Ulteriori informazioni](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >I **frammenti visivi** sono in disponibilità limitata (LA). Questa funzionalità è limitata a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non può essere distribuita in nessun altro ambiente.

### Gruppo trappola {#24-7-2}

Un **Gruppo trappola**, è un elenco di indirizzi seed. Viene utilizzato per includere indirizzi specifici nelle consegne e quindi eseguire il targeting dei profili che non corrispondono ai criteri di targeting definiti. In questo modo, i destinatari che non rientrano nel pubblico della consegna possono riceverla, come farebbe qualsiasi altro destinatario di targeting. Puoi utilizzare gli indirizzi seed quando invii le bozze o per proteggere la mailing list. [Ulteriori informazioni](../audience/trap-group.md)

### Modelli di notifiche push avanzate {#24-7-3}

Ora puoi inviare notifiche push avanzate. La notifica push avanzata è una forma migliorata di notifica mobile che va oltre i semplici messaggi di testo incorporando elementi multimediali come immagini, pulsanti interattivi o altri contenuti rich media. Con questa versione, è ora disponibile un set di modelli per notifiche push avanzate per le app iOS e Android.

[Ulteriori informazioni](../push/rich-push.md)

>[!AVAILABILITY]
>
>Questa funzionalità richiede un aggiornamento a Campaign v8.6.3 <!--or v8.7.2-->. Per ulteriori informazioni, consulta le [note sulla versione](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} della console client di Campaign v8.

### Miglioramenti {#improvements-24-7}

**Gestione cartelle**: è ora possibile gestire autorizzazioni e restrizioni sulle cartelle.

## Note sulla versione di giugno {#24-6-release}

**Data di rilascio**: 18-19 giugno 2024

Le seguenti funzioni e i miglioramenti sono disponibili per tutti gli utenti a partire dalla versione di giugno.

<!--### Delivery alerting {#24-6-3}

The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)-->

### Piani e programmi {#24-6-4}

Ora puoi creare piani e programmi per organizzare le campagne. Definendo una gerarchia di cartelle, puoi organizzare le campagne in programmi e i programmi in piani. [Ulteriori informazioni](../administration/plans-programs.md)

### Miglioramenti {#improvements-24-6}

* **Attività Riconciliazione in arricchimento**: l’attività **Arricchimento** può ora essere utilizzata per riconciliare i dati provenienti dallo schema del database di Campaign con i dati provenienti da un altro schema o con i dati provenienti da uno schema temporaneo, ad esempio i dati caricati tramite un’attività Carica file. Ad esempio, puoi utilizzare questa opzione per riconciliare il paese di un profilo, specificato in un file caricato, con uno dei paesi disponibili nella tabella dedicata del database di Campaign. [Ulteriori informazioni](../workflows/activities/enrichment.md)

## Note sulla versione di maggio {#24-5-release}

**Data di rilascio**: 21 maggio 2024

Le seguenti funzioni e i miglioramenti sono disponibili per tutti gli utenti a partire dalla versione di maggio.

### Audit trail  {#24-5-1}

La nuova funzionalità **Audit trail** fornisce un record dettagliato e cronologico di tutte le azioni e gli eventi che sono stati effettuati nell’istanza di Adobe Campaign in tempo reale. Offre un metodo pratico per tracciare tutte le modifiche apportate ai dati di Campaign, affrontando argomenti quali: lo stato dei flussi di lavoro, i singoli utenti più recenti per modificarli o le attività eseguite dagli utenti all’interno dell’istanza. [Ulteriori informazioni](../reporting/audit-trail.md)

### Campi personalizzati {#24-5-2}

I **Campi personalizzati** sono ulteriori attributi aggiunti agli schemi predefiniti tramite la console Adobe Campaign. Nell’interfaccia web di Campaign, questi campi personalizzati sono ora visibili in varie schermate, ad esempio nei dettagli di un profilo o in un profilo di test. Nell’interfaccia web, non è possibile creare campi personalizzati, ma ora è possibile modificare il modo in cui vengono visualizzati. [Ulteriori informazioni](../administration/custom-fields.md)

### Creare collegamenti tra tabelle {#24-5-3}

Nell’attività del flusso di lavoro **Arricchimento**, ora è possibile creare collegamenti con un’altra tabella. Utilizza la nuova sezione **Definizione collegamento** nei parametri dell’attività per creare un collegamento tra i dati della tabella di lavoro e il database di Adobe Campaign. Ad esempio, se carichi i dati da un file che contiene il numero di account, il paese e l’e-mail dei destinatari, ora puoi creare un collegamento alla tabella del paese per aggiornare queste informazioni nei rispettivi profili. [Ulteriori informazioni](../workflows/activities/enrichment.md#create-links)

### Miglioramenti generali {#improvements-24-5}

* **Direct mail**: ora puoi sfruttare l’editor di espressioni per selezionare gli attributi da visualizzare nei file di estrazione direct mail. [Ulteriori informazioni](../direct-mail/content-direct-mail.md)

* **Gestione cartelle**: è ora possibile creare una sottocartella di un tipo diverso rispetto alla cartella principale. [Ulteriori informazioni](../get-started/permissions.md#folders)

* **Globalizzazione**: nell’ambito del nostro impegno continuo per offrire un’esperienza utente unificata, abbiamo armonizzato la terminologia utilizzata nei prodotti e nelle app di Adobe Experience Cloud. Questo influisce sul termine tedesco “Titel” che viene modificato in “Label” quando si riferisce al nome di un oggetto. Le modifiche verranno implementate progressivamente nell’interfaccia utente e nella documentazione.


## Note sulla versione di aprile {#april-24-4-release}

**Data di rilascio**: 2 maggio 2024

### Nuove funzioni {#new-24-4}

Le seguenti funzioni sono disponibili per tutti gli utenti a partire dalla versione di aprile.

**Nuove attività del flusso di lavoro**

* **Aggiorna dati**: utilizza questa attività per eseguire aggiornamenti di massa sui campi del database. Esistono varie opzioni per personalizzare l’aggiornamento dei dati. [Ulteriori informazioni](../workflows/activities/update-data.md)
* **Servizi di iscrizione**: utilizza questa attività per abbonare o annullare l’abbonamento di più profili a/da un servizio in una singola azione. [Ulteriori informazioni](../workflows/activities/subscription-services.md)
* **Estrai file**: utilizza questa attività per esportare i dati da Adobe Campaign a un altro sistema come file esterno. [Ulteriori informazioni](../workflows/activities/extract-file.md)
* **Trasferisci file**: utilizza questa attività per ricevere o inviare file, verificare la presenza di file o elencarli su un server. Il protocollo utilizzato può essere un protocollo da server a server o HTTP. [Ulteriori informazioni](../workflows/activities/transfer-file.md)
* **Test**: utilizza questa attività per abilitare le transizioni in base a condizioni specifiche. [Ulteriori informazioni](../workflows/activities/test.md)
* **Codice JavaScript**: utilizza questa attività per eseguire uno snippet di codice JavaScript nel contesto di un flusso di lavoro. [Ulteriori informazioni](../workflows/activities/javascript-code.md)
* **Segnale esterno**: utilizza questa attività per attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o una chiamata API. [Ulteriori informazioni](../workflows/activities/external-signal.md)
* **Query incrementale**: utilizza questa attività per eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi. [Ulteriori informazioni](../workflows/activities/incremental-query.md)

**Modelli di notifiche push avanzate**

Ora puoi inviare notifiche push avanzate tramite Android. La notifica push avanzata è una forma di notifica mobile che va oltre i semplici messaggi di testo incorporando elementi multimediali come immagini, pulsanti interattivi o altri contenuti rich media. [Ulteriori informazioni](../push/rich-push.md)

Al momento questa funzione è presente in **Disponibilità limitata** (LA).


### Nuove funzioni in Disponibilità limitata {#acs-24-4}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Ciò significa che sono limitate a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuite in nessun altro ambiente.
>
>Consulta le seguenti pagine della documentazione: [Transizione da Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it).

* **Branding**: in qualità di utenti che hanno eseguito la migrazione da Campaign Standard, gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sulla relativa identità. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. Puoi creare questi brand e collegarli a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=it)

* **API REST**: in qualità di utente Campaign Standard migrato, puoi utilizzare le API REST per creare integrazioni per Adobe Campaign e il tuo ecosistema interfacciando Adobe Campaign con il pannello di tecnologie utilizzato. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=it)

* **Reporting dinamico**: in qualità di utente Campaign Standard migrato, puoi accedere al Reporting dinamico che fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Permette di accedere ai dati del profilo, abilitando l’analisi demografica per dimensioni di profilo, come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=it)

* **Pagine di destinazione**: i seguenti miglioramenti alle pagine di destinazione sono disponibili solo per chi proviene da Campaign Standard:

   * Ora, al momento della configurazione di un servizio, puoi fare riferimento a una pagina di destinazione predefinita per l’iscrizione o l’annullamento dell’iscrizione. Durante la progettazione di un’e-mail, se definisci un collegamento a tale pagina di destinazione, quando gli utenti inviano il modulo presente sulla pagina di destinazione, viene eseguitp automaticamente l’abbonamento o l’annullamento dell’abbonamento a tale servizio. [Ulteriori informazioni](../audience/manage-services.md#create-service)
   * Una nuova opzione nella configurazione della pagina di destinazione consente l’accesso ai visitatori anonimi. Se questa opzione è deselezionata, solo gli utenti identificati potranno accedere al modulo e inviarlo. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione nella configurazione della pagina di destinazione consente di memorizzare dati interni aggiuntivi durante il suo invio. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione consente di utilizzare una pagina di destinazione per diversi servizi, rendendola dinamica. Quando aggiungi un collegamento a un’e-mail, se selezioni una pagina di destinazione dinamica puoi selezionare qualsiasi servizio. Se selezioni una pagina di destinazione a cui è associato un servizio specifico, questo servizio verrà utilizzato automaticamente (non è possibile selezionarne un altro). [Ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ora le pagine di destinazione supportano i contenuti condizionali. [Ulteriori informazioni](../landing-pages/lp-content.md)

### Miglioramenti generali {#improvements-24-4}

I miglioramenti riportati di seguito sono disponibili per tutti i clienti a partire dalla versione di aprile.

* L’attività **Carica file** è stata migliorata con diverse sezioni che consentono di caricare un file di esempio, gestire gli errori e i rifiuti ed eliminare i file caricati dopo l’esecuzione dell’attività. [Ulteriori informazioni](../workflows/activities/load-file.md)


* Ora puoi **copiare e incollare le attività** da un flusso di lavoro a un altro in una scheda diversa del browser. [Ulteriori informazioni](../workflows/orchestrate-activities.md#copy-activities-copy)

* Tutte le attività del flusso di lavoro ora consentono di gestire le relative **opzioni di esecuzione**. Questo consente di definire la modalità di esecuzione dell’attività e il comportamento in caso di errori. [Ulteriori informazioni](../workflows/orchestrate-activities.md#execution-options-execution)

* L’opzione “Non attivare la transizione se la popolazione è vuota” nell’**attività Dividi** consente di scegliere se il flusso di lavoro deve passare all’attività successiva quando il risultato del segmento è vuoto. [Ulteriori informazioni](../workflows/activities/split.md)

## Note sulla versione di marzo {#24-3-release}

>[!AVAILABILITY]
>
>Questa versione è disponibile per tutti gli utenti a partire dalla versione [Campaign v8.6 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it). Per ulteriori informazioni sulle versioni e gli aggiornamenti della console client di Adobe Campaign, consulta la [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=it){target="_blank"}.

**Data di rilascio**: 19-20 marzo 2024

### Canale Direct mail {#24-3-dm}

Il canale **Direct mail** è ora disponibile per l’utilizzo nei flussi di lavoro e come consegne autonome. Direct mail è un canale offline che consente di creare, personalizzare e generare un file di estrazione e di condividerlo con i provider di servizi di direct mail per inviare comunicazioni per posta alla clientela.

### Nuova attività per flussi di lavoro Cambia origine dati {#24-3-change-data-source}

L’attività di targeting **Cambia origine dati** consente di cambiare l’origine dati della tabella di lavoro del flusso di lavoro. Questa attività offre maggiore flessibilità consentendo di gestire i dati tra diversi database e migliorare le prestazioni.

### Miglioramento dell’attività “Dividi” per flussi di lavoro {#24-3-split}

Ora puoi utilizzare l’opzione **Genera tutti i sottoinsiemi nella stessa tabella** nell’attività **Dividi** del flusso di lavoro, per raggruppare tutti i sottoinsiemi in una singola transizione di output.

### Query modeler {#24-3-query-modeler}

* Il query modeler è ora disponibile per l’utilizzo in E-mail designer. Questo consente di creare le condizioni durante la creazione di contenuti condizionali.
* Durante la creazione di una condizione personalizzata, ora sono disponibili valori predefiniti per gli attributi di tipo data.
* Non è più possibile aggiungere operatori a una nuova transizione nel diagramma. Possono essere aggiunti solo a una transizione esistente prima di filtrare i componenti per raggrupparli.