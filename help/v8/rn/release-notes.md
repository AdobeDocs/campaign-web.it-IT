---
title: Note sulla versione più recente
description: Scopri la nuova funzione in arrivo con l’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d50dfc4ea433fa48301707b40164e2fdf9fa64fd
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 26%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarli regolarmente."

<!--Last update: **March 19, 2024**-->

I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Note sulla versione di aprile {#april-24-4-release}

**Data di rilascio**: 2 maggio 2024

### Nuove funzioni {#new-24-4}

Le seguenti funzioni sono disponibili per tutti gli utenti a partire dalla versione di aprile.

**Nuove attività del flusso di lavoro**

* **Aggiorna dati** : utilizza questa attività per eseguire aggiornamenti di massa sui campi del database. Diverse opzioni consentono di personalizzare l’aggiornamento dei dati. [Ulteriori informazioni](../workflows/activities/update-data.md)
* **Servizi di abbonamento** : utilizza questa attività per abbonare o annullare l’abbonamento di più profili a/da un servizio in una singola azione. [Ulteriori informazioni](../workflows/activities/subscription-services.md)
* **Extract file** : utilizza questa attività per esportare i dati da Adobe Campaign a un altro sistema come file esterno. [Ulteriori informazioni](../workflows/activities/extract-file.md)
* **Trasferisci file** : utilizza questa attività per ricevere o inviare file, verificare la presenza di file o elencarli su un server. Il protocollo utilizzato può essere un protocollo server-to-server o HTTP. [Ulteriori informazioni](../workflows/activities/transfer-file.md)
* **Test** : utilizza questa attività per abilitare le transizioni in base a condizioni specificate. [Ulteriori informazioni](../workflows/activities/test.md)
* **Codice JavaScript** : utilizza questa attività per eseguire uno snippet di codice JavaScript nel contesto di un flusso di lavoro. [Ulteriori informazioni](../workflows/activities/javascript-code.md)
* **Segnale esterno** : utilizza questa attività per attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o una chiamata API. [Ulteriori informazioni](../workflows/activities/external-signal.md)
* **Query incrementale** : utilizza questa attività per eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Questo consente di eseguire il targeting solo per i nuovi elementi. [Ulteriori informazioni](../workflows/activities/incremental-query.md)

**Modelli di notifiche push potenziate**

Ora puoi inviare notifiche push potenziate tramite Android. La notifica push potenziata è una forma avanzata di notifica mobile che va oltre i semplici messaggi di testo incorporando elementi multimediali come immagini, pulsanti interattivi o altri contenuti rich media. [Ulteriori informazioni](../push/rich-push.md)

Questa funzione è attiva **Disponibilità limitata** (LA).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Nuove funzioni in Disponibilità limitata {#acs-24-4}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Sono limitati ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.
>
>Consulta le seguenti pagine della documentazione: [Transizione di Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Marchio** - In qualità di utente Campaign Standard migrato, gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull’identità di un brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. Puoi creare questi brand e collegarli a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **API REST** - In qualità di utente Campaign Standard migrato, puoi utilizzare le API Rest per creare integrazioni per Adobe Campaign e creare il tuo ecosistema interfacciando Adobe Campaign con il pannello di tecnologie utilizzato. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Reporting dinamico** - In qualità di utente Campaign Standard migrato, puoi accedere al Reporting dinamico che fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Aggiunge l’accesso ai dati del profilo, consentendo l’analisi demografica per dimensioni di profilo come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Pagine di destinazione** - I seguenti miglioramenti alle pagine di destinazione sono disponibili solo per gli utenti che passano da Campaign Standard:

   * Ora puoi fare riferimento a una pagina di destinazione predefinita per l’abbonamento o il suo annullamento al momento della configurazione di un servizio. Durante la progettazione di un’e-mail, se definisci un collegamento a tale pagina di destinazione, gli utenti che inviano il modulo della pagina di destinazione si abbonano o annullano automaticamente l’abbonamento a questo servizio. [Ulteriori informazioni](../audience/manage-services.md#create-service)
   * Una nuova opzione nella configurazione della pagina di destinazione consente ai visitatori anonimi di accedere alla pagina di destinazione. Deselezionando questa opzione, solo gli utenti identificati possono accedere al modulo e inviarlo. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione nella configurazione della pagina di destinazione consente di memorizzare dati interni aggiuntivi durante l’invio della pagina di destinazione. [Ulteriori informazioni](../landing-pages/create-lp.md#create-landing-page)
   * Una nuova opzione consente di utilizzare una pagina di destinazione per diversi servizi, rendendola dinamica. Quando aggiungi un collegamento a un’e-mail, se selezioni una pagina di destinazione dinamica puoi selezionare qualsiasi servizio. Se selezioni una pagina di destinazione a cui è associato un servizio specifico, questo servizio verrà utilizzato automaticamente (non è possibile selezionarne un altro). [Ulteriori informazioni](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Il contenuto condizionale è ora supportato nelle pagine di destinazione. [Ulteriori informazioni](../landing-pages/lp-content.md)

### Miglioramenti generali {#improvements-24-4}

I miglioramenti riportati di seguito sono disponibili per tutti i clienti a partire dalla versione di aprile.
<!--**Workflow - Copy/Paste into another tab**: -->

* Il **Carica file** l’attività è stata migliorata con diverse sezioni che ti consentono di caricare un file di esempio, gestire gli errori e i rifiuti e eliminare i file caricati dopo l’esecuzione dell’attività. [Ulteriori informazioni](../workflows/activities/load-file.md)


* Ora puoi **attività copia/incolla** da un flusso di lavoro a un altro flusso di lavoro da una scheda diversa del browser. [Ulteriori informazioni](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Tutte le attività del flusso di lavoro ora consentono di gestire i **opzioni di esecuzione**. Questo ti consente di definire la modalità di esecuzione dell’attività e il comportamento in caso di errori. [Ulteriori informazioni](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* L’opzione &quot;Non attivare la transizione se la popolazione è vuota&quot; nel **Attività split** consente di scegliere se il flusso di lavoro deve passare all’attività successiva quando il risultato del segmento è vuoto. [Ulteriori informazioni](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **Campi personalizzati** sono attributi aggiuntivi aggiunti agli schemi predefiniti tramite la console Adobe Campaign. Nell’interfaccia utente web di Campaign, questi campi personalizzati sono ora visibili in varie schermate, ad esempio i dettagli di un profilo o di un profilo di test. Nell’interfaccia utente web, non è possibile creare campi personalizzati, ma ora è possibile modificarne la modalità di visualizzazione. [Ulteriori informazioni](../administration/custom-fields.md)


## Note sulla versione di marzo {#24-3-release}

>[!AVAILABILITY]
>
>Questa versione è disponibile per tutti gli utenti a partire da [Campaign v8.6 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it). Per ulteriori informazioni sulle versioni e gli aggiornamenti della console client di Adobe Campaign, consulta la [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=it){target="_blank"}.

**Data di rilascio**: 19-20 marzo 2024

### Canale Direct mail {#24-3-dm}

Il canale **Direct mail** è ora disponibile per l’utilizzo nei flussi di lavoro e come consegne autonome. Direct mail è un canale offline che consente di creare, personalizzare e generare un file di estrazione e di condividerlo con i provider di servizi di direct mail per inviare comunicazioni per posta alla clientela.

### Nuova attività per flussi di lavoro Cambia origine dati {#24-3-change-data-source}

L’attività di targeting **Cambia origine dati** consente di cambiare l’origine dati della tabella di lavoro del flusso di lavoro. Questa attività offre maggiore flessibilità consentendo di gestire i dati tra diversi database e migliorare le prestazioni.

### Miglioramento dell’attività per flussi di lavoro Dividi {#24-3-split}

Ora puoi utilizzare la **Genera tutti i sottoinsiemi nella stessa tabella** opzione in **Dividi** attività del flusso di lavoro per raggruppare tutti i sottoinsiemi in una singola transizione di output.

### Query modeler {#24-3-query-modeler}

* Il query modeler è ora disponibile per l’utilizzo in E-mail designer. Consente di creare le condizioni durante la creazione di contenuto condizionale.
* Durante la creazione di una condizione personalizzata sono ora disponibili valori predefiniti per gli attributi di tipo data.
* Non è più possibile aggiungere operatori a una nuova transizione nel diagramma. Possono essere aggiunte solo a una transizione esistente prima di filtrare i componenti per raggrupparli.
