---
title: Note sulla versione precedente dell’interfaccia utente di Campaign Web v8
description: Versioni 2026 dell’interfaccia utente di Campaign Web
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 0cc09a983d412889f2b734a5bfb30bf422247ec0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 22%

---

# Note sulla versione 2026 {#2026-release}

In questa pagina sono elencate tutte le modifiche e i miglioramenti disponibili con le **versioni 2026**. Le ultime note sulla versione sono disponibili in [questa pagina](release-notes.md).

## Versione di febbraio 2026 {#26-2-release}

_17 febbraio 2026_

### Nuove funzioni {#26-2-features}

<!--table>
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
</table-->

<!--table>
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
</table-->

<table>
<thead>
<tr>
<th><strong>Vista Timeline nell’inventario delle campagne</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’inventario delle campagne ora include una vista Timeline che consente di visualizzare e gestire le campagne nel tempo: passa da un elenco all’altro e naviga per settimana, mese o giorno, utilizza il pulsante Oggi per passare alla data corrente e apri i dettagli della campagna (stato, flussi di lavoro, consegne) in un pannello a destra, con gli stessi filtri e cerca della vista elenco.</p>
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
<p>Ora puoi creare e gestire gli schemi direttamente dall’interfaccia utente di Campaign Web. Questa funzione consente di creare nuove tabelle, estendere gli schemi esistenti e creare moduli personalizzati. Puoi definire strutture di dati personalizzate per supportare esigenze aziendali specifiche senza richiedere l’accesso alla console client.</p>
<p>Nota: questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata) e verrà implementata globalmente in una versione futura.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/schemas.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)-->

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
<p>La funzione di consegna multilingue è ora disponibile per tutti i clienti (GA). Questa funzione consente di inviare più messaggi in diverse lingue nell’interfaccia utente di Adobe Campaign Web. Puoi scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare l’anteprima di queste consegne nelle lingue scelte. 
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
<p>La funzionalità di arricchimento dei profili nei messaggi transazionali è ora disponibile per tutti i clienti (GA). Oltre alle e-mail, ora sono supportati anche gli SMS e le notifiche push. Questa funzione ti consente di personalizzare i messaggi transazionali collegando i campi del database di Adobe Campaign al contenuto del messaggio. Puoi selezionare mappature target, colonne di arricchimento e una chiave di riconciliazione per garantire una personalizzazione accurata e in tempo reale, mantenendo al contempo le soglie di prestazioni.</p>
<p>Per ulteriori informazioni, consulta la <a href="../transactional-messaging/profile-enrichment.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager Live e copie per lingua</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’integrazione dei contenuti di Adobe Experience Manager ti consente di accedere a tutte le lingue e le Live Copy create in Adobe Experience Manager direttamente all’interno di Campaign durante la creazione delle consegne. Puoi aggiornare il contenuto in tempo reale per recuperare le versioni più recenti di Adobe Experience Manager. Questa integrazione elimina la sincronizzazione manuale dei contenuti tra Adobe Experience Manager e Campaign, semplificando il flusso di lavoro della campagna multilingue.</p>
<p>Per ulteriori informazioni, consulta la <a href="../integrations/aem-multilingual.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Esperimenti di contenuto - Test A/B</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Gli esperimenti sui contenuti in Adobe Campaign Web consentono di definire più varianti di consegna per test A/B al fine di misurare le prestazioni migliori per il pubblico di destinazione. Puoi variare il contenuto, l’oggetto o il mittente della consegna per testare versioni diverse e determinare quale variante produce i risultati migliori. Puoi eseguire test A/B su vari elementi e-mail, come l’oggetto, il nome del mittente e il contenuto del corpo dell’e-mail.</p>
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
<p>L’attività Consegna continua ti consente di aggiungere nuovi destinatari a una consegna esistente. Questo tipo di consegna evita di dover creare ogni volta una nuova consegna, rendendola più efficiente per gli avvisi o le notifiche a basso volume inviate in base alle esigenze. Una consegna continua crea una singola istanza di consegna. Tutti i registri di consegna (broadLog) e di tracciamento fanno riferimento a questa consegna, semplificandone il monitoraggio e il reporting.</p>
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
<p>Il processo di approvazione aiuta a coordinare più parti interessate e garantisce il controllo di qualità prima dell’invio delle consegne. Utilizza le approvazioni quando l’organizzazione richiede la convalida da parte di team diversi, ad esempio responsabili marketing che rivedono il contenuto o analisti di dati che convalidano i tipi di pubblico target.</p>
<p>Per ulteriori informazioni, consulta la <a href="../campaigns/campaign-approvals.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-1-improvements}

* Il reporting dinamico ora supporta le notifiche push e gli SMS. [Ulteriori informazioni](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtri predefiniti: una nuova opzione &quot;Filtro condiviso&quot; consente di rendere un filtro predefinito disponibile ad altri utenti dell’organizzazione. [Ulteriori informazioni](../get-started/predefined-filters.md#share-filter)
* I campi di personalizzazione creati in Adobe Experience Manager, come Nome, E-mail, Data e Indirizzo, sono ora inclusi e disponibili quando si utilizza il modello di contenuto.
* La valutazione della qualità dei contenuti ora verifica la leggibilità, la coesione e l’efficacia indipendentemente dalle linee guida del brand, identificando messaggi non chiari, toni incoerenti o lacune strutturali. [Ulteriori informazioni](../content/brands-score.md)
