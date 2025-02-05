---
audience: end-user
title: Seleziona gli attributi e aggiungili ai preferiti
description: Scopri come utilizzare gli attributi e accedere facilmente agli attributi preferiti e utilizzati di recente.
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 6%

---

# Seleziona gli attributi e aggiungili ai preferiti {#folders}

L’interfaccia utente di Campaign Web consente di selezionare gli attributi dal database in varie posizioni, a seconda dell’azione che desideri eseguire. Ad esempio, puoi selezionare gli attributi quando definisci le colonne di output per una consegna direct mailing o per un file da estrarre. Analogamente, gli attributi possono essere selezionati quando si utilizza il modellatore di query per creare regole, filtri o tipi di pubblico.

![](assets/attributes-list.png)

Per riutilizzare rapidamente gli attributi utilizzati di frequente, è possibile aggiungerli ai preferiti. In questo modo, sono facilmente accessibili per le attività future. Oltre ai preferiti, è possibile anche visualizzare e utilizzare gli attributi selezionati più di recente.

L’interfaccia fornisce anche uno strumento di distribuzione dei valori, che consente di visualizzare la distribuzione dei valori di un attributo all’interno di una tabella. Questo strumento può aiutarti a identificare l’intervallo e la frequenza dei valori, garantendo la coerenza dei dati durante la creazione di query o espressioni.

## Preferiti e attributi recenti {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Preferiti e recenti"
>abstract="Il menu **[!UICONTROL Preferiti e recenti]** nel selettore attributi fornisce una visualizzazione organizzata degli attributi aggiunti ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Gli attributi preferiti vengono visualizzati per primi, seguiti da quelli utilizzati di recente, semplificando l&#39;individuazione degli attributi necessari."

Il menu **[!UICONTROL Preferiti e recenti]** nel selettore attributi fornisce una visualizzazione organizzata degli attributi aggiunti ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Gli attributi preferiti vengono visualizzati per primi, seguiti da quelli utilizzati di recente, semplificando l&#39;individuazione degli attributi necessari.

![](assets/attributes-favorites.png)

Per aggiungere un attributo ai preferiti, posiziona il cursore del mouse sul pulsante delle informazioni e seleziona l’icona a forma di stella. L&#39;attributo verrà quindi aggiunto automaticamente all&#39;elenco dei preferiti. Se non desideri più mantenere un attributo come preferito, puoi rimuoverlo selezionando nuovamente l’icona a forma di stella.

Puoi aggiungere fino a 20 attributi preferiti. Gli attributi Preferiti e recenti sono associati a ogni utente all’interno di un’organizzazione. Ciò significa che sono accessibili da macchine diverse, garantendo un’esperienza fluida tra i dispositivi.

## Identificare la distribuzione dei valori all&#39;interno di una tabella {#distribution}

Il pulsante **Distribuzione di valori**, disponibile nel riquadro delle informazioni di un attributo, consente di analizzare la distribuzione dei valori per tale attributo all&#39;interno della tabella. Questa funzione è particolarmente utile per comprendere i valori disponibili, i relativi conteggi e le percentuali. Consente inoltre di evitare problemi come l’utilizzo incoerente delle maiuscole o dell’ortografia durante la creazione di query o di espressioni.

![](assets/attributes-distribution-values.png)

Per gli attributi con un numero elevato di valori, lo strumento visualizza solo i primi venti. In tali casi, una notifica **[!UICONTROL Carico parziale]** apparirà per indicare questa limitazione. Puoi applicare filtri avanzati per perfezionare i risultati visualizzati e concentrarti su valori o sottoinsiemi di dati specifici. Le istruzioni dettagliate sull&#39;utilizzo dei filtri sono disponibili [qui](../get-started/work-with-folders.md#filter-the-values).

Per ulteriori informazioni sull&#39;utilizzo dello strumento di distribuzione dei valori in contesti diversi, vedere le sezioni seguenti:

- [Distribuzione dei valori in una cartella](../get-started/work-with-folders.md##distribution-values-folder)
- [Distribuzione dei valori in una query](../query/build-query.md#distribution-values-query)
