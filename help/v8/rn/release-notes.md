---
title: Note sulla versione più recente
description: Scopri la nuova funzione in arrivo con l’interfaccia utente di Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 99%

---

# Note sulla versione {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Novità"
>abstract="I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Le note sulla versione vengono aggiornate più volte al mese. **La versione di marzo è ora live**, inclusi il canale Direct mail, la nuova attività per flussi di lavoro Cambia origine dati e altri miglioramenti."


<!--Last update: **March 19, 2024**-->

I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di consegna continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate più volte al mese. Consultale regolarmente.

>[!AVAILABILITY]
>
>Questa versione è disponibile per tutti gli utenti a partire da [Campaign v8.6 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it). Per ulteriori informazioni sulle versioni e gli aggiornamenti della console client di Adobe Campaign, consulta la [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=it){target="_blank"}.

## Note sulla versione di marzo {#24-3-release}

**Data di rilascio**: 19-20 marzo 2024

### Canale Direct mail {#24-3-dm}

Il canale **Direct mail** è ora disponibile per l’utilizzo nei flussi di lavoro e come consegne autonome. Direct mail è un canale offline che consente di creare, personalizzare e generare un file di estrazione e di condividerlo con i provider di servizi di direct mail per inviare comunicazioni per posta alla clientela. [Ulteriori informazioni](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nuova attività per flussi di lavoro Cambia origine dati {#24-3-change-data-source}

L’attività di targeting **Cambia origine dati** consente di cambiare l’origine dati della tabella di lavoro del flusso di lavoro. Questa attività offre maggiore flessibilità consentendo di gestire i dati tra diversi database e migliorare le prestazioni. [Ulteriori informazioni](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Miglioramento dell’attività per flussi di lavoro Dividi {#24-3-split}

Ora puoi utilizzare l’opzione **Genera tutti i sottoinsiemi nella stessa tabella** nell’attività **Dividi** per i flussi di lavoro, per raggruppare tutti i sottoinsiemi in una singola transizione di output. [Ulteriori informazioni](../workflows/activities/split.md)

### Query modeler {#24-3-query-modeler}

* Il query modeler è ora disponibile per l’utilizzo in E-mail designer. Consente di creare condizioni durante la creazione di contenuti condizionali. [Ulteriori informazioni](../personalization/conditions.md)
* Durante la creazione di una condizione personalizzata, ora sono disponibili valori predefiniti per gli attributi di tipo data. [Ulteriori informazioni](../query/build-query.md)
* Non è più possibile aggiungere operatori a una nuova transizione nel diagramma. Possono essere aggiunti solo a una transizione esistente prima di filtrare i componenti per raggrupparli. [Ulteriori informazioni](../query/build-query.md)
