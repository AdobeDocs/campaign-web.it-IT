---
title: Note sulla versione più recente
description: Scopri la nuova funzione in arrivo con l’interfaccia utente di Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 5%

---

# Note sulla versione {#latest-release}

<!--Last update: **March 19, 2024**-->

I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di distribuzione continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Di conseguenza, queste note sulla versione vengono aggiornate diverse volte al mese. Controllali regolarmente.

>[!AVAILABILITY]
>
>Questa versione è disponibile per tutti gli utenti che iniziano [Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=it). Ulteriori informazioni sulle versioni e sugli aggiornamenti della console client di Adobe Campaign in [Documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=it){target="_blank"}.

## Versione di marzo {#24-3-release}

**Data di rilascio**: 19-20 marzo 2024

### Canale direct mailing {#24-3-dm}

**Direct mail** channel è ora disponibile per l’utilizzo nei flussi di lavoro e come consegne autonome. La direct mailing è un canale offline che ti consente di creare, personalizzare e generare un file di estrazione e di condividerlo con i provider di direct mailing per inviare e-mail ai tuoi clienti.

![](../assets/do-not-localize/direct-mail.gif)

### Nuova attività del flusso di lavoro Modifica origine dati {#24-3-change-data-source}

Il **Cambia origine dati** l’attività di targeting ti consente di modificare l’origine dati utilizzata dalla tabella di lavoro del flusso di lavoro. Questa attività offre maggiore flessibilità consentendo di gestire i dati tra i diversi database e migliorare le prestazioni.

![](../assets/do-not-localize/change-data-source.gif)

### Miglioramento dell’attività di suddivisione del flusso di lavoro {#24-3-split}

Ora puoi utilizzare la **Genera tutti i sottoinsiemi nella stessa tabella** opzione in **Dividi** attività del flusso di lavoro per raggruppare tutti i sottoinsiemi in una singola transizione di output.

### Query modeler {#24-3-query-modeler}

* Il modellatore di query è ora disponibile per l’utilizzo in E-mail Designer. Consente di creare le condizioni durante la creazione di contenuto condizionale.
* Durante la creazione di una condizione personalizzata sono ora disponibili valori predefiniti per gli attributi di tipo data.
* Non è più possibile aggiungere operatori a una nuova transizione nel diagramma. Possono essere aggiunte solo a una transizione esistente prima di filtrare i componenti per raggrupparli.
