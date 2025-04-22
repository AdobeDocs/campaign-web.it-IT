---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 53%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di distribuzione continua che consente un approccio scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate diverse volte al mese. Controllali regolarmente.

Le modifiche e i miglioramenti disponibili con le versioni precedenti sono elencati [in questa pagina](release-notes-24.md).

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
<p>Ora è possibile creare tipologie e regole di tipologia nell’interfaccia utente di Adobe Campaign Web. Le tipologie controllano, filtrano e assegnano priorità all’invio delle consegne. Le tipologie verificano che le consegne contengano sempre componenti obbligatori (come un collegamento per l’annullamento dell’abbonamento o una riga dell’oggetto) o regole di filtro per escludere i gruppi dal pubblico (come utenti non abbonati, concorrenti o clienti non fidelizzati).</p>
<img src="assets/do-not-localize/typology.gif" alt="Illustrazione della creazione di regole di tipologia nell’interfaccia utente web di Adobe Campaign">
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
<p>È ora possibile creare mappature target nell’interfaccia utente di Campaign Web. Le mappature target definiscono il collegamento tra i diversi canali di consegna (e-mail, SMS, notifiche push) e i campi dati di uno schema. La mappatura del target definisce il pubblico target: profili, beneficiari del contratto, operatori, abbonati, potenziali clienti e altri.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Illustrazione della creazione di mappature di destinazione nell’interfaccia utente web di Adobe Campaign">
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
<img src="assets/do-not-localize/schemas.gif" alt="Illustrazione dei dettagli dello schema e dei campi personalizzati che si modificano nell’interfaccia utente web di Adobe Campaign">
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
<p>I frammenti visivi sono blocchi visivi predefiniti che puoi riutilizzare in più consegne e-mail o in modelli di contenuto. Questa funzione è ora disponibile per tutta la clientela per l’esecuzione di build sul server nella versione 8.6.4 e successive.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Illustrazione della creazione e dell’utilizzo di frammenti visivi nell’interfaccia utente di Adobe Campaign Web">
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
<img src="assets/do-not-localize/external-delivery.gif" alt="Illustrazione della configurazione della consegna esterna nell’interfaccia utente web di Adobe Campaign">
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
<p>È ora possibile creare enumerazioni direttamente tramite l’interfaccia utente web di Adobe Campaign. Un’enumerazione è un elenco di valori suggeriti dal sistema per compilare i campi. Utilizza le enumerazioni per standardizzare i valori di questi campi, assistere l’input dei dati o utilizzare all’interno di query.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Illustrazione della gestione dell’enumerazione nell’interfaccia utente web di Adobe Campaign">
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
<img src="assets/do-not-localize/options.gif" alt="Illustrazione della creazione di opzioni personalizzate nell’interfaccia utente web di Adobe Campaign">
<p>Per ulteriori informazioni, consulta la <a href="../administration/options.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Definisci e chiama i codici JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora possibile creare codici JavaScript nell’interfaccia utente web di Adobe Campaign. Questo consente di creare funzioni riutilizzabili che possono essere utilizzate in tutti i flussi di lavoro, in modo simile a una libreria.</p>
<img src="assets/do-not-localize/javascript.gif" alt="Illustrazione della creazione di codice JavaScript nell’interfaccia utente web di Adobe Campaign">
<p>Per ulteriori informazioni, consulta la <a href="../administration/javascript-codes.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Generazione di pagine di destinazione con AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’Assistente AI è ora disponibile con le consegne delle pagine di destinazione, consentendoti di generare testo, immagini o layout di pagina completi.</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="Illustrazione dell’utilizzo dell’Assistente IA per la generazione di pagine di destinazione nell’interfaccia utente web di Adobe Campaign">
<p>Per ulteriori informazioni sull’Assistente IA, consulta la <a href="../email/generative-lp.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#25-1-improvements}

* Personalizzazione della visualizzazione dei campi personalizzati nell’interfaccia:
   * Seleziona campi personalizzati aggiuntivi da visualizzare nell’interfaccia.
   * Imposta le regole per la visualizzazione dei campi personalizzati di tipo collegamento, ad esempio la limitazione dei valori di elenco in base all’input di un altro campo.
   * Disporre i campi in modo più flessibile nell&#39;interfaccia: i campi possono estendersi su una singola colonna o essere raggruppati in sottosezioni per una migliore organizzazione.
   * Imposta campi specifici come di sola lettura.

* Filtri Recenti e Preferiti: aggiungi gli attributi utilizzati di frequente ai preferiti per un accesso rapido. Oltre ai preferiti, visualizza e utilizza gli attributi selezionati più di recente.

* Account esterni: quando si crea un nuovo account esterno, è possibile selezionare il nuovo tipo **[!UICONTROL Indirizzamento]**. Consente di configurare un account esterno specifico da utilizzare nelle consegne esterne. [Ulteriori informazioni](../administration/external-account.md#routing).