---
title: Note sulla versione precedente dell’interfaccia utente di Campaign Web v8
description: Versioni 2026 dell’interfaccia utente di Campaign Web
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 4eae8f0ea3c176a12e040f7406aac699e14a5ba8
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 97%

---

# Note sulla versione 2026 {#2026-release}

In questa pagina sono elencate tutte le modifiche e i miglioramenti disponibili con le **versioni 2026**. Le note sulla versione più recenti sono disponibili in [questa pagina](release-notes.md).

## Versione di aprile 2026 {#26-4-release}

_29 aprile, 2026_

### Miglioramento {#26-4-improvement}

La sezione **Dati di arricchimento** è ora disponibile nell’attività del flusso di lavoro **Crea pubblico** (tipo di query). Puoi visualizzare, aggiungere, modificare e rimuovere **dati aggiuntivi** direttamente dall’interfaccia utente web di Campaign. Come nell’attività **Arricchimento**, è possibile aggiungere attributi di arricchimento singoli, collegamenti alle raccolte ed espressioni.

[Ulteriori informazioni](../workflows/activities/build-audience.md)

## Versione di marzo 2026 {#26-3-release}

_Marzo_ 24, 2026_

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

* L’attività del flusso di lavoro **Avvia** è stata aggiunta per migliorare la compatibilità con Client Console. Questa attività è facoltativa e non viene inserita per impostazione predefinita nei nuovi flussi di lavoro. Tuttavia, viene aggiunta automaticamente ai flussi di lavoro esistenti.
  [Ulteriori informazioni](../workflows/activities/about-activities.md#flow-control)
* Nelle impostazioni **Pianificazione** di una consegna, il campo di selezione del fuso orario è stato spostato sotto il campo **Data di contatto**. [Ulteriori informazioni](../msg/create-deliveries.md#gs-schedule)

## Versione di febbraio 2026 {#26-2-release}

_17 febbraio 2026_

### Nuove funzioni {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>Vista Timeline nell’inventario della campagna</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’inventario della campagna ora include una vista Timeline che consente di visualizzare e gestire le campagne nel tempo: passa da vista elenco a timeline e naviga per settimana, mese o giorno, utilizza il pulsante Oggi per passare alla data corrente e apri i dettagli della campagna (stato, flussi di lavoro, consegne) in un pannello a destra, con gli stessi filtri e la ricerca della vista elenco.</p>
<p>Per ulteriori informazioni, consulta la <a href="../campaigns/manage-campaigns.md#timeline">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Authoring dello schema (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi creare e gestire gli schemi direttamente dall’interfaccia utente di Campaign Web. Questa funzione ti consente di creare nuove tabelle, estendere gli schemi esistenti e creare moduli personalizzati. Puoi definire strutture di dati personalizzate per supportare specifiche esigenze di business senza che sia necessario l’accesso alla console client.</p>
<p>Nota: questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata) e verrà implementata globalmente in una versione futura.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/schemas.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## Versione di gennaio 2026 {#26-1-release}

_27 gennaio 2026_

### Nuove funzioni {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Funzionalità di consegna multilingue (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La funzione di consegna multilingue è ora disponibile per tutti i clienti (GA). Questa funzione consente di inviare più messaggi in diverse lingue nell’interfaccia utente di Adobe Campaign Web. Puoi scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare in anteprima queste consegne nelle lingue scelte. 
<p>Per ulteriori informazioni, consulta la <a href="../msg/multilingual.md">documentazione dettagliata</a>.</p>
<p>Sono stati apportati i seguenti miglioramenti alle notifiche push multilingue:</p>
<ul>
<li>Ora puoi compilare rapidamente tutte le varianti di lingua caricando un file CSV contenente il tuo contenuto multilingue. <a href="../msg/multilingual.md#csv-upload">Ulteriori informazioni</a>
</li>
<li>Sono ora supportate le notifiche push potenziate.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Arricchimento del profilo nei messaggi transazionali (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La funzionalità di arricchimento del profilo nei messaggi transazionali è ora disponibile per tutta la clientela (GA). Oltre alle e-mail, ora sono supportati anche gli SMS e le notifiche push. Questa funzione ti consente di personalizzare i messaggi transazionali collegando i campi del database di Adobe Campaign al contenuto del messaggio. Puoi selezionare mappature target, colonne di arricchimento e una chiave di riconciliazione per garantire una personalizzazione accurata e in tempo reale, mantenendo al contempo le soglie di prestazione.</p>
<p>Per ulteriori informazioni, consulta la <a href="../transactional-messaging/profile-enrichment.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Live Copy e copie per lingua di Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’integrazione dei contenuti di Adobe Experience Manager consente di accedere a tutte le lingue e le Live Copy create in Adobe Experience Manager direttamente all’interno di Campaign durante la creazione delle consegne. Puoi aggiornare il contenuto in tempo reale per recuperare le versioni più recenti di Adobe Experience Manager. Questa integrazione elimina la sincronizzazione dei contenuti manuale tra Adobe Experience Manager e Campaign, semplificando il flusso di lavoro della campagna multilingue.</p>
<p>Per ulteriori informazioni, consulta la <a href="../integrations/aem-multilingual.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Esperimenti sul contenuto - Test A/B</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Gli esperimenti sui contenuti in Adobe Campaign Web consentono di definire più varianti di consegna per test A/B al fine di individuare quelle con prestazioni migliori per il pubblico target. Puoi variare il contenuto, l’oggetto o il mittente della consegna per testare versioni diverse e determinare quale variante produce i risultati migliori. Puoi condurre test A/B su vari elementi e-mail, come l’oggetto, il nome del mittente e il contenuto del corpo dell’e-mail.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/ab-testing.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Attività di consegna continua</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’attività Consegna continua ti consente di aggiungere nuovi destinatari a una consegna esistente. Questo tipo di consegna evita di dover creare ogni volta una nuova consegna, e rende più efficiente l’invio di avvisi o notifiche a basso volume in base alle esigenze. Una consegna continua crea una singola istanza di consegna. Tutti i registri di consegna (broadLog) e di tracciamento fanno riferimento a quest’unica consegna, semplificandone il monitoraggio e il reporting.</p>
<p>Per ulteriori informazioni, consulta la <a href="../workflows/activities/continuous-delivery.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gestione dell’approvazione delle campagne</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Il processo di approvazione aiuta a coordinare più stakeholder e garantisce il controllo di qualità prima dell’invio delle consegne. Utilizza le approvazioni quando l’organizzazione richiede la convalida da parte di team diversi, ad esempio responsabili di marketing che rivedono il contenuto o analisti di dati che convalidano i tipi di pubblico target.</p>
<p>Per ulteriori informazioni, consulta la <a href="../campaigns/campaign-approvals.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-1-improvements}

* Il reporting dinamico ora supporta le notifiche push e gli SMS. [Ulteriori informazioni](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtri predefiniti: una nuova opzione “Filtro condiviso” consente di rendere un filtro preimpostato disponibile ad altri utenti dell’organizzazione. [Ulteriori informazioni](../get-started/predefined-filters.md#share-filter)
* I campi di personalizzazione creati in Adobe Experience Manager, come Nome, E-mail, Data e Indirizzo, sono ora inclusi e disponibili quando si utilizza il modello di contenuto.
* La valutazione della qualità dei contenuti ora controlla la leggibilità, la coesione e l’efficacia indipendentemente dalle linee guida del brand, per individuare messaggi poco chiari e incoerenza a livello di tono o struttura. [Ulteriori informazioni](../content/brands-score.md)
