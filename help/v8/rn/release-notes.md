---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti introdotti nelle versioni precedenti sono elencati [in questa pagina](release-notes-24.md).

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

* **Attività dei flussi di lavoro** - È ora possibile spostare un’attività e tutti i relativi nodi secondari da una transizione a un&#39;altra all’interno di un flusso di lavoro. Per eseguire questa operazione, nel riquadro delle proprietà dell’attività è disponibile il pulsante dedicato **Sposta**. [Ulteriori informazioni](../workflows/orchestrate-activities.md#move)

* **Attività di arricchimento nei flussi di lavoro**

   * È ora possibile definire un alias e un’etichetta durante la creazione di un nuovo campo nell’attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md#collection-settings)
   * Ora è possibile aggiungere offerte per ogni profilo nell’attività **Arricchimento**. [Ulteriori informazioni](../workflows/activities/enrichment.md##add-offers)

* **Distribuzione dei valori**: accedendo all’elenco dei campi per la personalizzazione, ora è possibile controllare come vengono distribuiti i valori per ciascun campo. Finestra popup dedicata che mostra il numero e la percentuale per ciascun valore. [Ulteriori informazioni](../query/build-query.md#distribution-values-query)

* **Informazioni sulla versione e sul sistema** - Ora è possibile accedere ai dettagli delle versioni delle istanze, sia per la console client che per l’interfaccia utente web. In questa nuova sezione sono elencati anche tutti i pacchetti incorporati installati nell’ambiente. [Ulteriori informazioni](../get-started/user-interface.md#user-interface-about)

* **Elenchi** - Ora è possibile riordinare facilmente i valori di un elenco. [Ulteriori informazioni](../get-started/work-with-folders.md)

* **Consegna** - La variabile di consegna è ora accessibile dai campi di personalizzazione. [Ulteriori informazioni](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)