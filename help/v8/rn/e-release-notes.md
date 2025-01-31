---
title: Note preliminari sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con la prossima versione dell’interfaccia utente di Campaign Web
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 202796bbaa26afb0741a5eb3947795ceff7e5414
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 18%

---

# Note preliminari sulla versione {#e-release}

L’interfaccia utente di Adobe Campaign Web offre continuamente nuove funzioni, miglioramenti alle funzioni esistenti e correzioni di bug. Nelle [note sulla versione](release-notes.md), tutte le modifiche sono consolidate alla fine di ogni mese.

**Le note preliminari sulla versione riportate di seguito sono soggette a modifiche senza preavviso fino alla data di disponibilità del rilascio**. I collegamenti, le schermate e la documentazione aggiornata sono pubblicati nella [note sulla versione](release-notes.md), alla data di rilascio.

## Versione di gennaio 2025 {#25-1-release}

**Data di rilascio**: 5 febbraio 2025

Le seguenti funzioni e miglioramenti sono disponibili a partire dalla versione di gennaio.

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
<p>I frammenti visivi sono blocchi visivi predefiniti che puoi riutilizzare in più consegne e-mail o in modelli di contenuto. Questa funzione è ora disponibile per tutti i clienti che eseguono su server build 8.6.4 e successive.</p>
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
<p>Ora puoi definire consegne esterne e modelli di consegna esterna nell’interfaccia web di Campaign. In questa modalità, i messaggi vengono compilati in un file di input che può essere condiviso con il provider esterno. Per impostazione predefinita, per il canale direct mailing viene utilizzata la modalità di consegna esterna.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creare regole business (regole di tipologia)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi creare tipologie e regole di tipologia nell’interfaccia web di Adobe Campaign. Una tipologia è una raccolta di regole di tipologia che consentono di controllare, filtrare e assegnare priorità alle consegne. Le tipologie garantiscono che le consegne contengano sempre gli elementi richiesti (ad esempio un collegamento per l’annullamento dell’abbonamento o una riga dell’oggetto) e applichino regole di filtro per escludere gruppi specifici dal pubblico di destinazione (ad esempio utenti non abbonati, concorrenti o clienti non fidelizzati).</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>È ora possibile creare enumerazioni direttamente tramite l’interfaccia utente web di Adobe Campaign. Un’enumerazione è un elenco di valori suggeriti dal sistema per compilare i campi. Utilizza le enumerazioni per standardizzare i valori di questi campi, aiutarti con l’input di dati o utilizzare all’interno di query.</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Ora puoi accedere alle opzioni tecniche nell’interfaccia utente web di Adobe Campaign e creare opzioni personalizzate in base alle tue esigenze. Ciò è particolarmente utile quando si lavora con attività del flusso di lavoro del codice JavaScript per memorizzare dati intermedi.</p>
<img src="assets/do-not-localize/options.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>È ora possibile creare codici JavaScript nell’interfaccia utente web di Adobe Campaign. Questo consente di creare funzioni riutilizzabili che possono essere utilizzate in tutti i flussi di lavoro, in modo simile a una libreria.</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#25-1-improvements}

* Personalizza la visualizzazione dei campi personalizzati nell’interfaccia:

   * Ora puoi selezionare campi personalizzati aggiuntivi da visualizzare nell’interfaccia
   * È ora possibile impostare regole per la visualizzazione di campi personalizzati di tipo collegamento, ad esempio limitare i valori di elenco in base all&#39;input di un altro campo
   * Ora è possibile disporre i campi nell’interfaccia in modo più flessibile: i campi possono estendersi su una singola colonna o essere raggruppati in sottosezioni per una migliore organizzazione
   * È ora possibile impostare campi specifici come di sola lettura

* Filtri recenti e Preferiti: per riutilizzare rapidamente gli attributi utilizzati di frequente, è ora possibile aggiungerli ai preferiti. In questo modo, sono facilmente accessibili per le attività future. Oltre ai preferiti, puoi anche visualizzare e utilizzare gli attributi selezionati più di recente.


