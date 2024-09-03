---
title: Note sulla versione dell’interfaccia utente di Campaign Web v8
description: Scopri le nuove funzioni in arrivo con l’ultima versione dell’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# Note sulla versione {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Note sulla versione"
>abstract="Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, le note sulla versione di Campaign vengono aggiornate diverse volte al mese, con le funzioni, i miglioramenti e le correzioni più recenti. Si consiglia di controllarle regolarmente."

Le versioni dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

## Note sulla versione di agosto {#24-8-release}

**Data di rilascio**: 3 settembre 2024

Le seguenti funzioni e miglioramenti sono disponibili a partire dalla versione di agosto.

* **Distribuzione dei valori** - Quando si accede all&#39;elenco dei campi per la personalizzazione, è ora possibile controllare la distribuzione dei valori per ciascun campo. Una finestra a comparsa dedicata mostra il numero e la percentuale per ciascun valore. [Ulteriori informazioni](../query/build-query.md#distribution-values-query)

* **Parametri SMTP** - Le impostazioni SMTP sono ora disponibili nelle impostazioni di consegna e-mail. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#smtp)

* **Variabili globali** - È ora possibile definire le variabili globali per definire i valori per le consegne. [Ulteriori informazioni](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuove funzioni in Disponibilità limitata {#acs-24-8}

>[!AVAILABILITY]
>
>Le seguenti funzionalità sono in Disponibilità limitata (LA). Ciò significa che sono limitate a chi esegue la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuite in nessun altro ambiente.
>
>Consulta le seguenti pagine della documentazione: [Passaggio di Campaign Standard a Campaign v8](../rn/acs-migration.md) e [Funzionalità per gli utenti di Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=it){target="_blank"}.

* **Branding per Direct Mail** - Gli amministratori tecnici possono ora definire uno o più brand per centralizzare i parametri che influiscono sull&#39;identità di un brand. Ciò include il logo del brand, il dominio dell’URL di accesso delle pagine di destinazione o le impostazioni di tracciamento dei messaggi. Ora puoi creare questi brand e collegarli a messaggi o pagine di destinazione. Questa configurazione viene gestita tramite modelli. [Ulteriori informazioni](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Iscrizioni con pagine di destinazione** - È ora possibile collegare una pagina di destinazione a un servizio e inviare un messaggio di conferma quando gli utenti lo convalidano. [Ulteriori informazioni](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Frammenti visivi** - È ora possibile archiviare frammenti di contenuto visivo. [Ulteriori informazioni](../content/create-fragment.md#archive)

* **Captcha nelle pagine di destinazione** - È ora possibile aggiungere captcha per proteggere la pagina di destinazione dallo spam e dagli abusi causati dai bot. Ciò non è intrusivo per i clienti in quanto non richiede alcuna interazione da parte loro e si basa sulle interazioni con il sito. [Ulteriori informazioni](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
