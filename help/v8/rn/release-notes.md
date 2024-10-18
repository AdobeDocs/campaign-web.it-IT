---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: a1b1a40be4d2004181f03bba5c43d0302d6f2c47
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 95%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Aggiornamenti di settembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Accelerazione dei contenuti dell’Assistente IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Dopo aver creato e personalizzato il messaggio, portalo al livello successivo con l’AI Assistant Content Accelerator in Adobe Campaign Web. Questo potente strumento consente di ottimizzare l’impatto dei contenuti generando una serie di testi coinvolgenti, titoli principali e immagini visivamente accattivanti.</p>
<p>Immergiti in un’esperienza pratica con <a href="https://experienceleague.adobe.com/it/apps/journey-optimizer/ai-assistant-content-accelerator">la nostra anteprima delle funzionalità live</a>, progettata per consentirti di esplorarne le funzionalità in prima persona e comprenderne appieno le funzionalità.</a>.</p>
<p>Per ulteriori informazioni, consulta la <a href="../email/generative-gs.md">documentazione dettagliata</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Data di disponibilità: 12 settembre</p>
</td>
</tr>
</tbody>
</table>

## Note sulla versione di agosto {#24-8-release}

**Data di rilascio**: 3 settembre 2024

Le funzioni e i miglioramenti seguenti sono disponibili a partire dalla versione di agosto.

* **Distribuzione dei valori**: accedendo all’elenco dei campi per la personalizzazione, ora è possibile controllare come vengono distribuiti i valori per ciascun campo. Finestra popup dedicata che mostra il numero e la percentuale per ciascun valore. [Ulteriori informazioni](../query/build-query.md#distribution-values-query)

* **Parametri SMTP**: le impostazioni SMTP sono ora disponibili nelle impostazioni di consegna e-mail. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#smtp)

* **Variabili globali**: è ora possibile definire le variabili globali per stabilire i valori per le consegne. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuove funzioni in Disponibilità limitata {#acs-24-8}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Ciò significa che sono limitate a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuite in nessun altro ambiente.
>
>Consulta le seguenti pagine della documentazione: [Transizione da Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it){target="_blank"}.

* **Branding per direct mail**: gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull’identità del brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. I brand ora possono essere creati e collegati a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. [Ulteriori informazioni](https://experienceleague.adobe.com/it/docs/experience-cloud/campaign/branding/branding-assign)

* **Abbonamenti con pagine di destinazione**: è ora possibile collegare una pagina di destinazione a un servizio e inviare un messaggio di conferma quando gli utenti lo convalidano. [Ulteriori informazioni](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Frammenti visivi**: è ora possibile archiviare i frammenti di contenuti visivi. [Ulteriori informazioni](../content/create-fragment.md#archive)

* **Captcha nelle pagine di destinazione**: ora è possibile aggiungere Captcha per proteggere la pagina di destinazione dallo spam e dagli abusi causati dai bot. Ciò non è intrusivo per la clientela in quanto non richiede alcuna interazione da parte loro e si basa sulle interazioni con il sito. [Ulteriori informazioni](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
