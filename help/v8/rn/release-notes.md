---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

Le modifiche e i miglioramenti disponibili con le versioni precedenti sono elencati in [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Versione di aprile 2025 {#25-4-release}

**Data di rilascio**: mercoledì 29 aprile 2025


### Nuove funzioni {#25-4-features}

Le seguenti funzioni sono disponibili per tutti gli utenti a partire dalla versione di aprile.

<table>
<thead>
<tr>
<th><strong>Canale del call center</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Il canale del call center è ora disponibile nell’interfaccia utente web di Campaign. Questo canale si riferisce a un metodo di comunicazione utilizzato per gestire e tenere traccia delle comunicazioni o delle interazioni gestite tramite un call center, in genere le chiamate telefoniche effettuate dagli agenti a clienti o potenziali.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Per ulteriori informazioni, consulta la <a href="../call-center/gs-call-center.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nuovo generatore di regole</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>È ora disponibile un nuovo generatore di regole che consente di definire condizioni complesse in un’interfaccia utente migliorata. Se necessario, puoi passare dal generatore di regole precedente al nuovo.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Per ulteriori informazioni, consulta la <a href="../query/query-modeler-overview.md">documentazione dettagliata</a>.</p>
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
<p>In qualità di amministratore di Campaign, ora puoi impostare nuove connessioni con sistemi esterni dall’interfaccia utente di Campaign Web.
Puoi anche visualizzare, aggiornare e gestire gli account esterni esistenti.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/external-account.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#25-4-improvements}

**Miglioramenti generali all&#39;interfaccia**

* Le opzioni Descrizione campo, Aggiungi ai preferiti e Distribuzione dei valori per gli attributi dello schema sono ora più visibili nell’interfaccia utente. Per ulteriori informazioni, consulta la [documentazione dettagliata](../get-started/attributes.md).
* Nell’interfaccia di, la data e l’ora vengono ora visualizzate in base alla lingua primaria impostata nelle preferenze di Experience League. Questo miglioramento è disponibile solo per diverse lingue. Per visualizzare l&#39;elenco completo delle lingue supportate, fare riferimento alla [documentazione dettagliata](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor e-mail**: per migliorare l&#39;accessibilità nell&#39;interfaccia utente di Campaign Web, sono ora disponibili due nuovi campi nel Designer e-mail: corrispondono all&#39;elemento `title` e all&#39;attributo lang nell&#39;elemento `html` del contenuto dell&#39;e-mail. Puoi definire queste impostazioni oltre al campo Preheader, nella sezione email Body. Per ulteriori informazioni, consulta la [documentazione dettagliata](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemi**

* Ora puoi modificare lo schema temporaneo di un elenco dall’interfaccia utente web di Campaign. Per ulteriori informazioni, consulta la [documentazione dettagliata](../audience/manage-audience.md).
* Ora puoi visualizzare in anteprima i campi personalizzati di uno schema in una schermata di esempio. Per ulteriori informazioni, consulta la [documentazione dettagliata](../administration/custom-fields.md#add).
* È ora possibile spostare i campi personalizzati nell’elenco tramite trascinamento. Per ulteriori informazioni, consulta la [documentazione dettagliata](../administration/custom-fields.md#add).


### Nuove funzioni in Disponibilità limitata {#25-4-features-la}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Sono limitati ai clienti che eseguono la migrazione di **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente. Richiedono l’aggiornamento del server Campaign alla versione v8.7.4.
>
>Consulta le seguenti pagine della documentazione: [Transizione da Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it).

* **Creazione di consegne multilingue** - Nell&#39;interfaccia utente Web di Adobe Campaign è ora possibile inviare più consegne di e-mail in lingue diverse. La funzione Consegna multilingue consente di scegliere la lingua predefinita della consegna e le diverse lingue in cui la consegna può essere inviata. Puoi anche visualizzare in anteprima queste consegne nelle lingue scelte. Per ulteriori informazioni, consulta la [documentazione dettagliata](../email/edit-content.md).

* **Reporting dinamico per multilingue** - Il reporting dinamico è ora disponibile per le consegne di e-mail multilingue. Per ulteriori informazioni, consulta la [documentazione dettagliata](../reporting/global-reports.md).

* **Supporto API REST SMS (LA)** - L&#39;API REST per la messaggistica transazionale è ora disponibile per il canale SMS. Quando nel payload sono presenti sia e-mail che telefono cellulare, puoi utilizzare il campo &quot;wishedChannel&quot; per specificare il canale. Se non viene fornito, l’e-mail verrà utilizzata per impostazione predefinita a meno che il canale desiderato non richieda esplicitamente l’invio di SMS. Per ulteriori informazioni, consulta la [documentazione dettagliata](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

