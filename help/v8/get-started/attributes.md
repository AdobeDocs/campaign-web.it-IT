---
audience: end-user
title: Selezionare gli attributi e aggiungerli ai preferiti
description: Scopri come utilizzare gli attributi e accedere facilmente agli attributi preferiti e utilizzati di recente.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: 3bedb4562c5858cd6057fd8a17064ccac8303c39
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 100%

---

# Selezionare gli attributi e aggiungerli ai preferiti {#folders}

L’interfaccia utente di Campaign Web consente di selezionare gli attributi dal database in varie posizioni, a seconda dell’azione che desideri eseguire. Ad esempio, puoi selezionare gli attributi quando definisci le colonne di output per una consegna direct mail o per un file da estrarre. Analogamente, gli attributi possono essere selezionati quando utilizzi il query modeler per creare regole, filtri o tipi di pubblico.

![](assets/attributes-list.png)

Per riutilizzare rapidamente gli attributi usati di frequente, è possibile aggiungerli ai preferiti. In questo modo, sono facilmente accessibili per le attività future. Oltre ai preferiti, è possibile anche visualizzare e utilizzare gli attributi selezionati più di recente.

L’interfaccia fornisce inoltre uno strumento di distribuzione dei valori, che consente di visualizzare la distribuzione dei valori di un attributo all’interno di una tabella. Questo strumento può aiutarti a identificare l’intervallo e la frequenza dei valori, per maggiore coerenza nei dati durante la creazione di query o espressioni.

## Attributi preferiti e recenti {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Preferiti e recenti"
>abstract="Il menu **[!UICONTROL Preferiti e recenti]** nel selettore degli attributi fornisce presenta in modo organizzato gli attributi che hai aggiunto ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Per aiutarti a trovare più facilmente gli attributi che ti servono, gli attributi preferiti sono elencati per primi, seguiti da quelli utilizzati di recente."

Il menu **[!UICONTROL Preferiti e recenti]** nel selettore degli attributi fornisce presenta in modo organizzato gli attributi che hai aggiunto ai preferiti, insieme a un elenco degli attributi utilizzati di recente. Per aiutarti a trovare più facilmente gli attributi che ti servono, gli attributi preferiti sono elencati per primi, seguiti da quelli utilizzati di recente.

![](assets/attributes-favorites.png)

Per aggiungere un attributo ai preferiti, passa il puntatore sul relativo pulsante delle informazioni e seleziona l’icona a forma di stella. L’attributo verrà quindi aggiunto all’elenco dei preferiti. Se non desideri più mantenere un attributo tra i preferiti, puoi rimuoverlo selezionando nuovamente l’icona a forma di stella.

Puoi aggiungere fino a 20 attributi preferiti. Gli attributi recenti e preferiti sono associati a ogni utente all’interno di un’organizzazione. Ciò significa che sono accessibili da computer diversi, per un’esperienza fluida quando si passa da un dispositivo a un altro.

## Identificare la distribuzione dei valori all’interno di una tabella {#distribution}

Il pulsante **Distribuzione dei valori**, disponibile nel riquadro delle informazioni di un attributo, consente di analizzare la distribuzione dei valori per tale attributo all’interno della tabella. Questa funzione è particolarmente utile per comprendere i valori disponibili, i relativi conteggi e le percentuali. Consente inoltre di evitare problemi associati a valori incoerenti, per via di ortografia o maiuscole diverse, durante la creazione di query o di espressioni.

![](assets/attributes-distribution-values.png)

Per gli attributi con un numero elevato di valori, lo strumento visualizza solo i primi venti. In tali casi, verrà visualizzata la notifica **[!UICONTROL Carico parziale]** per indicare questa limitazione. Puoi applicare filtri avanzati per perfezionare i risultati visualizzati e concentrarti su valori o sottoinsiemi di dati specifici. Informazioni dettagliate sull’utilizzo dei filtri sono disponibili [qui](../get-started/work-with-folders.md#filter-the-values).

Per ulteriori informazioni sull’utilizzo dello strumento per la distribuzione dei valori in contesti diversi, consulta le sezioni seguenti:

- [Distribuzione dei valori in una cartella](../get-started/work-with-folders.md##distribution-values-folder)
- [Distribuzione dei valori in una query](../query/build-query.md#distribution-values-query)
