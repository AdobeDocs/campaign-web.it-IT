---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f1f207785ad25ceb8f9891bfad74193768cb2937
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 91%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione di aprile 2026 {#26-4-release}

_29 aprile 2026_

### Miglioramento {#26-4-improvement}

La sezione **Dati di arricchimento** è ora disponibile nell&#39;attività del flusso di lavoro **Genera pubblico** (tipo di query). Puoi visualizzare, aggiungere, modificare e rimuovere **dati aggiuntivi** direttamente dall&#39;interfaccia utente di Campaign Web. Come nell&#39;attività **Enrichment**, è possibile aggiungere attributi di arricchimento singoli, collegamenti alle raccolte ed espressioni.

[Ulteriori informazioni](../workflows/activities/build-audience.md)

## Versione di marzo 2026 {#26-3-release}

_24 marzo_ 2026_

### Nuove funzioni {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Authoring dello schema (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La funzione di authoring dello schema è ora disponibile per tutta la clientela (GA). Questa funzionalità consente di creare e gestire gli schemi direttamente dall’interfaccia utente web di Campaign. Puoi creare nuove tabelle, estendere gli schemi esistenti e creare moduli personalizzati. Puoi definire strutture di dati personalizzate per supportare specifiche esigenze di business senza che sia necessario l’accesso alla console client.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/schemas.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Temi in E-mail designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>I temi forniscono una migliore esperienza di authoring per le e-mail consentendoti di definire stili di tema riutilizzabili che soddisfino le linee guida del tuo brand. Ora puoi utilizzare le variabili tema nei frammenti, garantendo così uno stile coerente nei diversi modelli e-mail. Questa funzione consente di creare e-mail più rapidamente con moduli preimpostati che riprendono elementi di contenuto quali titoli, descrizioni, immagini e collegamenti, mantenendo al contempo la coerenza del brand.</p>
<p>Nota: questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata) e verrà implementata globalmente in una versione futura.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/apply-email-themes.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integrazione di modelli Firefly personalizzati e modelli di generazione di immagini di terze parti</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Abilita l’integrazione diretta con modelli Firefly standard e personalizzati, nonché con modelli di immagini di terze parti approvati, per usufruire di maggiore flessibilità, controllo e allineamento al brand durante la generazione delle immagini.</p>
<p>Scegli il modello giusto per le tue esigenze:</p>
<ul><li> <strong>Modello Adobe</strong> (basato su Firefly Image Model 4) per la generazione immediata di immagini senza configurazione aggiuntiva</li><li> <strong>Modello partner</strong> (basato su Gemini 2.5 Flash) per funzionalità specializzate</li><li><strong>Modelli personalizzati</strong> (modelli specifici del brand basati sulle tue risorse) per la generazione di prodotti in linea con il brand che sono allineati con precisione all’identità del brand, allo stile e alle linee guida visive.</li></ul>
<p>Per ulteriori informazioni, consulta la <a href="../content/generative-models.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Attività di consegna automatizzata</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’attività del flusso di lavoro <strong>Consegna automatizzata</strong> è ora disponibile nella palette del flusso di lavoro. Puoi utilizzarla per creare o eseguire azioni di consegna (preparare, inviare una bozza, preparare e avviare, ecc.) direttamente all’interno del flusso di lavoro. Seleziona una consegna esistente creata all’esterno del flusso di lavoro per riutilizzarla a ogni esecuzione, oppure crea una nuova consegna da un modello a ogni esecuzione dell’attività.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Per ulteriori informazioni, consulta la <a href="../workflows/activities/automated-delivery.md">documentazione dettagliata.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Più rami del flusso di lavoro e attività di unione</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Ora sono supportati <strong>più rami</strong>. Invece di utilizzare un <strong>fork</strong>, puoi fare clic su <strong>Aggiungi ramo</strong> sulla barra degli strumenti. È stata migliorata anche l’attività <strong>AND-join</strong>. Si tratta ora di un’attività di <strong>unione</strong> generica che ti consente di scegliere tra le opzioni di unione AND e OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Per ulteriori informazioni, consulta la le pagine della documentazione <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrare le attività</a> e <a href="../workflows/activities/join.md">Unione</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-3-improvements}

* È stata aggiunta l’attività del flusso di lavoro **Inizio** per migliorare la compatibilità con la console client. Questa attività è facoltativa e non viene inserita per impostazione predefinita nei nuovi flussi di lavoro. Tuttavia, viene aggiunto automaticamente ai flussi di lavoro esistenti.
  [Ulteriori informazioni](../workflows/activities/about-activities.md#flow-control)
* Nelle impostazioni **Pianificazione** di una consegna, il campo di selezione del fuso orario è stato spostato sotto il campo **Data di contatto**. [Ulteriori informazioni](../msg/create-deliveries.md#gs-schedule)