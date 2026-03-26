---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione di marzo 2026 {#26-3-release}

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
<p>La funzione di authoring dello schema è ora disponibile per tutti i clienti (GA). Questa funzionalità consente di creare e gestire gli schemi direttamente dall’interfaccia utente web di Campaign. È possibile creare nuove tabelle, estendere gli schemi esistenti e creare moduli personalizzati. Puoi definire strutture di dati personalizzate per supportare esigenze aziendali specifiche senza richiedere l’accesso alla console client.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/schemas.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Temi nel Designer e-mail (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>I temi forniscono una migliore esperienza di authoring per le e-mail consentendoti di definire stili di tema riutilizzabili che soddisfino le linee guida del tuo marchio. Ora puoi utilizzare le variabili tema nei frammenti, garantendo così uno stile coerente nei diversi modelli e-mail. Questa funzione consente di creare e-mail più rapidamente con moduli predefiniti che riprendono elementi di contenuto quali titoli, descrizioni, immagini e collegamenti, mantenendo al contempo la coerenza del brand.</p>
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
<p>Integrazione perfetta di modelli Firefly standard e personalizzati, insieme a modelli di immagini di terze parti approvati, per fornire maggiore flessibilità, controllo e allineamento del brand durante la generazione delle immagini.</p>
<p>Scegli il modello giusto per le tue esigenze:</p>
<ul><li> <strong>Adobe model</strong> (con tecnologia Firefly Image Model 4) per la generazione immediata di immagini senza installazione aggiuntiva</li><li> <strong>Modello partner</strong> (con tecnologia Gemini 2.5 Flash) per funzionalità specializzate</li><li><strong>Modelli personalizzati</strong> (modelli specifici del brand addestrati sulle tue risorse) per la generazione di prodotti sul brand che sono allineati con precisione alla tua identità del brand, allo stile e alle linee guida visive.</li></ul>
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
<p>L'attività del flusso di lavoro <strong>Consegna automatica</strong> è ora disponibile nella palette del flusso di lavoro. Puoi utilizzarlo per creare o eseguire azioni di consegna (preparare, inviare una bozza, preparare e avviare, ecc.) direttamente all’interno del flusso di lavoro. Seleziona una consegna esistente creata all’esterno del flusso di lavoro per riutilizzarla a ogni esecuzione, oppure crea una nuova consegna da un modello a ogni esecuzione dell’attività.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Per ulteriori informazioni, consulta la <a href="../workflows/activities/automated-delivery.md"> documentazione dettagliata.</p>
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

<p><strong>Sono supportati più rami</strong>. Invece di utilizzare un <strong>Fork</strong>, puoi fare clic su <strong>Aggiungi ramo</strong> nella barra degli strumenti. Anche l'attività <strong>AND-join</strong> è stata migliorata. Si tratta ora di un'attività <strong>Join</strong> generica che consente di scegliere tra le opzioni di join AND e OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Per ulteriori informazioni, consulta <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrare le attività</a> e <a href="../workflows/activities/join.md">Partecipare</a> pagine della documentazione.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-3-improvements}

* L&#39;attività del flusso di lavoro **Start** è stata aggiunta per migliorare la compatibilità con Client Console. Questa attività è facoltativa e non viene inserita per impostazione predefinita nei nuovi flussi di lavoro. Tuttavia, viene aggiunto automaticamente ai flussi di lavoro esistenti.
  [Ulteriori informazioni](../workflows/activities/about-activities.md#flow-control)
* Il campo di selezione del fuso orario nelle impostazioni **Pianifica** di una consegna è stato spostato sotto il campo **Data di contatto**. [Ulteriori informazioni](../msg/create-deliveries.md#gs-schedule)