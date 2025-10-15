---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: ht
source-wordcount: '524'
ht-degree: 100%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti introdotti nelle versioni precedenti sono elencati nelle pagine [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Aggiornamenti di ottobre 2025 {#25-9-updates}

_9 ottobre 2025_

<table>
<thead>
<tr>
<th><strong>Funzionalità multilingue per messaggi transazionali, notifiche push e SMS (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nell’interfaccia utente di Adobe Campaign Web è ora possibile inviare più messaggi transazionali, notifiche push e messaggi SMS in lingue diverse. La funzione Consegna multilingue consente di scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare l’anteprima di queste consegne nelle lingue scelte.</p>
<p>Nota: questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata) e verrà implementata globalmente in una versione futura.</p>
<p>Per ulteriori informazioni, consulta la <a href="../msg/multilingual.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Arricchimento del profilo nei messaggi transazionali (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Questa funzionalità ti consente di personalizzare i messaggi transazionali collegando i campi del database di Adobe Campaign al contenuto del messaggio. Puoi selezionare mappature target, colonne di arricchimento e una chiave di riconciliazione per garantire una personalizzazione accurata e in tempo reale, mantenendo al contempo le soglie di prestazioni.</p>
<p>Nota: questa funzionalità è disponibile solo per un set di organizzazioni (disponibilità limitata) e verrà implementata globalmente in una versione futura. Questa funzione è attualmente disponibile solo per le e-mail.</p>
<p>Per ulteriori informazioni, consulta la <a href="../transactional-messaging/profile-enrichment.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>


## Versione di settembre 2025 {#25-9-release}

_23 settembre 2025_

Le seguenti funzioni sono disponibili a partire dalla versione di settembre.

<table>
<thead>
<tr>
<th><strong>Canale personalizzato per consegne API</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi orchestrare ed eseguire le consegne direttamente dall’interfaccia utente di Adobe Campaign Web in base a canali API personalizzati. Queste consegne possono essere autonome o far parte di un flusso di lavoro. La configurazione del canale API personalizzato viene eseguita nella console.</p>
<p>Per ulteriori informazioni, consulta la <a href="../call-center/gs-custom-channel.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Authoring di account esterni</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>In qualità di amministratore di Campaign, ora puoi configurare nuove connessioni con sistemi esterni dall’interfaccia utente di Campaign Web. Puoi anche visualizzare, aggiornare e gestire gli account esterni esistenti.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/create-external-account.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Blocco del contenuto e-mail</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign ora ti consente di bloccare i contenuti nei modelli e-mail, bloccando l’intero modello oppure strutture e componenti specifici. Questo consente di evitare modifiche o eliminazioni non intenzionali, garantendo un maggiore controllo sulla personalizzazione dei modelli e migliorando l’efficienza e l’affidabilità delle campagne e-mail.</p>
<p>Per ulteriori informazioni, consulta la <a href="../content/content-locking.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Miglioramenti {#25-9-improvements}

* È stato aggiunto un set di nuovi operatori durante la configurazione di una condizione utilizzando la funzionalità di contenuto condizionale di E-mail designer.
* Le dimensioni filtro sono ora disponibile nell’attività del flusso di lavoro **Crea pubblico**. Per visualizzarle o modificarle, fai clic sull’icona accanto alla dimensione di targeting. [Ulteriori informazioni](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

