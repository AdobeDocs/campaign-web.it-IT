---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Versione del 26 luglio {#26-7-release}

_28 luglio 2026_

### Nuove funzioni {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Gestione delle offerte</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ora puoi gestire le offerte end-to-end direttamente dall’interfaccia utente web di Campaign. Configura gli ambienti e gli spazi delle offerte, crea il catalogo e le categorie delle offerte, crea le offerte con regole di idoneità e pesi di priorità e approvale e implementale per l’utilizzo nelle consegne. Le configurazioni avanzate rimangono disponibili nella console client.</p>
<p>Per ulteriori informazioni, consulta la <a href="../offers/gs-offer-management.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Configurazione del brand</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Gli amministratori tecnici ora possono creare e configurare i brand direttamente dall’interfaccia utente web di Campaign, senza utilizzare la console client. Tutte le impostazioni del brand, inclusi identità, sottodominio e protocolli, parametri di intestazione e-mail e parametri di tracciamento URL, sono ora disponibili nell’interfaccia web.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/branding/branding-configure.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Risorse pubbliche in E-mail Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Quando aggiungi immagini alle e-mail, ora puoi selezionare <strong>risorse pubbliche</strong>. Questo ti consente di scegliere un’immagine già disponibile nell’istanza di Adobe Campaign, ad esempio un file precedentemente importato nel Designer e-mail o una risorsa pubblica caricata dalla console client.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/content-components.md#image">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Attività del flusso di lavoro di caricamento dati (RDBMS)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L'attività <strong>Caricamento dati (RDBMS)</strong> è ora disponibile nell'interfaccia utente di Campaign Web. Utilizza questa attività per caricare i dati direttamente da un database relazionale esterno nel flusso di lavoro. I dati estratti sono disponibili in tutto il flusso di lavoro e possono essere utilizzati per il targeting, l’arricchimento o l’ulteriore elaborazione dei dati.</p>
<p>Per ulteriori informazioni, consulta la <a href="../workflows/activities/data-loading-rdbms.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Pagine JavaScript dinamiche</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Le pagine JavaScript dinamiche (JSSP) consentono di creare pagine lato server che generano contenuto dinamico quando si accede tramite un URL, ad esempio API personalizzate, esportazioni o logica dell’applicazione web. È ora possibile creare, modificare, duplicare ed eliminare queste pagine direttamente dall’interfaccia utente di Campaign Web.</p>
<p>Per ulteriori informazioni, consulta la <a href="../administration/dynamic-javascript-pages.md">documentazione dettagliata</a>.</p>
</td>
</tr>
</tbody>
</table>

### Miglioramenti {#26-7-improvements}

* Sono stati apportati i seguenti miglioramenti alla **configurazione dello schema personalizzato**:
  * La nuova sezione **Dati azione** ti consente di limitare le azioni disponibili nei record di uno schema personalizzato, indipendentemente dalle regole di sicurezza configurate nelle singole cartelle. [Ulteriori informazioni](../administration/schemas-action-data.md)
  * Sono stati aggiunti **filtri personalizzati** nella sezione **Configurazione elenco inventario**. Consentono di scegliere gli attributi da visualizzare come campi di accesso rapido nel riquadro dei filtri della visualizzazione elenco. [Ulteriori informazioni](../administration/schemas-custom-filters.md)

* Sono stati apportati i seguenti miglioramenti ai **flussi di lavoro**:
  * L’eliminazione di un’attività del flusso di lavoro è ora più flessibile: quando l’attività presenta attività successive, puoi scegliere di eliminarle tutte, eliminare solo l’attività selezionata o eliminarla mantenendo le attività successive in un nuovo ramo. [Ulteriori informazioni](../workflows/orchestrate-activities.md#delete-activity)
  * È ora possibile disconnettere una transizione tra due attività del flusso di lavoro senza eliminarle. Ciò consente di riorganizzare un diagramma di flusso di lavoro, ad esempio per mettere temporaneamente da parte un gruppo di attività che si desidera mantenere, senza doverle eliminare e ricreare. [Ulteriori informazioni](../workflows/orchestrate-activities.md#disconnect-transition)
  * Attorno all&#39;area di lavoro del flusso di lavoro vengono ora visualizzate barre di scorrimento orizzontali e verticali, che consentono di spostarsi tra flussi di lavoro di grandi dimensioni trascinando direttamente l&#39;area da visualizzare. [Ulteriori informazioni](../workflows/orchestrate-activities.md)
  * Quando si salva o si avvia/riavvia un flusso di lavoro, ora viene visualizzato un avviso se un altro utente ha modificato il flusso di lavoro nell’interfaccia utente Web o nella console client da quando è stato aperto. Puoi scegliere di ignorare le altre modifiche, ricaricare il flusso di lavoro per ottenere la versione più recente o annullare.

* **Indirizzo e-mail mittente**: ora puoi limitare il campo **Da e-mail** delle consegne a un elenco predefinito di indirizzi, utilizzando l&#39;opzione **NmsDelivery_senderAddressMask**. [Ulteriori informazioni](../administration/options.md#restrict-sender-address)
* Sono stati migliorati **i messaggi di errore di accesso**: quando un tentativo di accesso non riesce, l&#39;interfaccia utente Web visualizza ora un messaggio di errore più specifico per diversi scenari (ad esempio, quando all&#39;utente non è assegnata alcuna area di sicurezza o il suo indirizzo IP è limitato).
