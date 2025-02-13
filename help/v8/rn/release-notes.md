---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 93%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti introdotti nelle versioni precedenti sono elencati [in questa pagina](release-notes-24.md).

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

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

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
<th><strong>Generazione di pagine di destinazione con l’Assistente AI</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’Assistente AI è ora disponibile con le consegne delle pagine di destinazione, consentendoti di generare testo, immagini o layout di pagina completi.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Per ulteriori informazioni sull'Assistente AI, consulta la <a href="../email/generative-lp.md">documentazione dettagliata</a>.</p>
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