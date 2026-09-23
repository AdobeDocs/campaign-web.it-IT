---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 7a22b75c81435fa891fa8aa73c5c1acad1931710
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione di settembre 2026 {#26-9-release}

_22 settembre 2026_

### Nuove funzioni {#26-9-features}

<table>
<thead>
<tr>
<th><strong>Canale LINE</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign ora supporta il canale <strong>LINE</strong>, una popolare applicazione di messaggistica istantanea. Crea e invia messaggi LINE utilizzando contenuti di testo, immagini o video, in consegne autonome o in flussi di lavoro, insieme agli altri canali. <a href="../line/get-started-line.md">Ulteriori informazioni</a></p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-9-improvements}

* **Accesso alla navigazione laterale**: gli amministratori ora possono nascondere voci di menu specifiche dalla navigazione laterale. [Ulteriori informazioni](../administration/schemas-browse-access.md#customize-screen-display-screen-def)
* **Tipi di approvazione aggiuntivi**: ora è possibile richiedere approvazioni di budget e di inizio consegna per le consegne di Campaign, oltre alle approvazioni di contenuto e destinazione. [Ulteriori informazioni](../campaigns/campaign-approvals.md#configure-approval-settings-configure-approvals)
* **Destinazione SMS basata sul visitatore**: la mappatura della destinazione visitatore è ora disponibile per le consegne SMS. [Ulteriori informazioni](../sms/create-sms.md)
* **Pulsante Annulla flusso di lavoro**: un nuovo pulsante **Annulla** consente di ripristinare le modifiche non salvate in un flusso di lavoro. [Ulteriori informazioni](../workflows/orchestrate-activities.md#save-or-discard-your-changes-save-cancel)
* **Deduplicazione con più valori**: l&#39;opzione **Dopo un elenco di valori** ora supporta più attributi. [Ulteriori informazioni](../workflows/activities/deduplication.md#configure-the-deduplication-activity-deduplication-configuration)
* **Mappatura destinazione mobile**: è ora possibile creare mappature destinazione per destinazioni app mobili. [Ulteriori informazioni](../administration/target-mappings.md#create-a-target-mapping-create-mapping)
* **Arricchimento del database esterno**: è ora possibile arricchire dati da un database esterno nell&#39;attività **Arricchimento** o **Genera pubblico**. [Ulteriori informazioni](../workflows/activities/enrichment.md#external-data)
* **Riconciliazione pubblico file**: ora puoi configurare se importare i destinatari nel database quando esegui il targeting di un pubblico da un file. [Ulteriori informazioni](../audience/file-audience.md#select-and-configure-the-input-file-upload)
* **Partecipazioni dirette alle raccolte**: quando selezioni un attributo direttamente da una raccolta, ora puoi scegliere come creare la condizione: utilizzando l&#39;opzione predefinita consigliata, una funzione di aggregazione o un&#39;unione diretta avanzata. [Ulteriori informazioni](../query/build-query.md#custom-conditions-on-linked-tables-1-1-and-1-n-links-links)

