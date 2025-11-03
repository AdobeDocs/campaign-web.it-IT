---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 64%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti introdotti nelle versioni precedenti sono elencati nelle pagine [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Versione di ottobre 2025 {#25-10-updates}

_28 ottobre 2025_

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

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

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

<table>
<thead>
<tr>
<th><strong>Integrazione con Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Per migliorare l’efficienza del marketing e mantenere la coerenza del marchio, ora puoi integrare perfettamente le esperienze GenStudio for Performance Marketing con Campaign. Questo consente di sfruttare la creazione di contenuti basati sull’intelligenza artificiale di GenStudio insieme alle funzionalità avanzate di orchestrazione di Campaign.<p>
<p>Per ulteriori informazioni, consulta la <a href="../integrations/genstudio.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Supporto della modalità scura in E-mail designer</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>E-mail Designer ora offre la possibilità di passare alla visualizzazione in modalità scura, dove puoi definire anche impostazioni personalizzate specifiche. Il rendering finale dipende dal client e-mail del destinatario e non tutti i client e-mail supportano la modalità scura.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/accessible-content.md#dark-mode">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Miglioramenti {#25-10-improvements}

* Nelle consegne create nella console client, la sezione **Pubblico** ora indica se è stata definita una condizione dinamica per le destinazioni bozza. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Ora puoi passare dal generatore di regole nuovo a quello precedente quando imposti una condizione utilizzando la funzionalità di contenuto condizionale di E-mail Designer. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Ora puoi selezionare i collegamenti della raccolta, ad esempio gli acquisti, nella definizione della schermata dello schema Destinatari. I dati correlati vengono visualizzati nelle schermate del profilo tramite una scheda dedicata. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* In qualità di amministratore di Campaign, ora puoi impostare connessioni a Salesforce CRM e Microsoft Dynamics.
  [Ulteriori informazioni](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

