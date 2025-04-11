---
audience: end-user
title: Selezionare gli attributi e aggiungerli ai preferiti
description: Scopri come utilizzare gli attributi e accedere facilmente agli attributi preferiti e utilizzati di recente.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: c0c9c5da3369e55269411b7348004006cd3c139e
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 35%

---

# Selezionare gli attributi e aggiungerli ai preferiti {#folders}

L’interfaccia utente di Campaign Web consente agli utenti di selezionare gli attributi dal database in varie posizioni, a seconda dell’azione eseguita. Ad esempio, è possibile selezionare gli attributi durante la definizione delle colonne di output per una consegna direct mailing o per un file da estrarre. Analogamente, gli attributi possono essere selezionati quando si utilizza il modellatore di query per creare regole, filtri o creare tipi di pubblico.

![Selezionare gli attributi dall&#39;interfaccia del database, visualizzando le opzioni degli attributi.](assets/attributes-list.png)

Per riutilizzare rapidamente gli attributi utilizzati di frequente, aggiungili ai preferiti. In questo modo, sono facilmente accessibili per le attività future. Oltre ai preferiti, gli utenti possono visualizzare e utilizzare gli attributi selezionati più di recente.

L’interfaccia fornisce inoltre uno strumento di distribuzione dei valori, che consente di visualizzare la distribuzione dei valori di un attributo all’interno di una tabella. Questo strumento consente di identificare l’intervallo e la frequenza dei valori, garantendo la coerenza dei dati durante la creazione di query o espressioni.

## Attributi preferiti e recenti {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Preferiti e recenti"
>abstract="Il menu **[!UICONTROL Preferiti e recenti]** nel selettore degli attributi fornisce presenta in modo organizzato gli attributi che hai aggiunto ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Per aiutarti a trovare più facilmente gli attributi che ti servono, gli attributi preferiti sono elencati per primi, seguiti da quelli utilizzati di recente."

Il menu **[!UICONTROL Preferiti e recenti]** nel selettore attributi fornisce una visualizzazione organizzata degli attributi aggiunti ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Gli attributi preferiti vengono visualizzati per primi, seguiti da quelli utilizzati di recente, semplificando l&#39;individuazione degli attributi richiesti.

![Menu Preferiti e attributi recenti, con gli attributi preferiti e utilizzati di recente.](assets/attributes-favorites.png)

Per aggiungere un attributo ai preferiti, passa il puntatore sul relativo pulsante delle informazioni e seleziona l’icona a forma di stella. L&#39;attributo viene quindi aggiunto automaticamente all&#39;elenco dei preferiti. Per rimuovere un attributo dai preferiti, selezionare di nuovo l&#39;icona a forma di stella.

Gli utenti possono aggiungere fino a 20 attributi ai preferiti. Gli attributi preferiti e recenti sono associati a ogni utente all’interno di un’organizzazione, garantendo l’accessibilità tra computer diversi e fornendo un’esperienza fluida tra i dispositivi.

## Identificare la distribuzione dei valori all’interno di una tabella {#distribution}

Il pulsante **Distribuzione di valori**, disponibile nel riquadro delle informazioni di un attributo, consente agli utenti di analizzare la distribuzione dei valori per tale attributo all&#39;interno della tabella. Questa funzione è utile per comprendere i valori disponibili, i loro conteggi e le percentuali. Consente inoltre di evitare problemi come l’uso incoerente delle maiuscole o dell’ortografia durante la creazione di query o di espressioni.

![Interfaccia dello strumento Distribuzione dei valori, con conteggi e percentuali dei valori degli attributi.](assets/attributes-distribution-values.png)

Per gli attributi con un numero elevato di valori, lo strumento visualizza solo i primi venti. In questi casi, viene visualizzata una notifica **[!UICONTROL Carico parziale]** per indicare questa limitazione. Applica filtri avanzati per perfezionare i risultati visualizzati e concentrati su valori o sottoinsiemi di dati specifici. Le istruzioni dettagliate sull&#39;utilizzo dei filtri sono disponibili [qui](../get-started/work-with-folders.md#filter-the-values).

Per ulteriori informazioni sull’utilizzo dello strumento per la distribuzione dei valori in contesti diversi, consulta le sezioni seguenti:

* [Distribuzione dei valori in una cartella](../get-started/work-with-folders.md##distribution-values-folder)
* [Distribuzione dei valori in una query](../query/build-query.md#distribution-values-query)