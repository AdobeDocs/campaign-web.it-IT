---
title: 'Configurare le opzioni di [!DNL Campaign] '
description: Scopri come configurare le opzioni di Campaign e creare opzioni personalizzate.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: 10a43da9df57a32f987b3d4c51bea91da10cbf92
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 5%

---

# Configurare opzioni [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Opzioni"
>abstract="Opzioni"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Crea opzione"
>abstract="Crea opzione"

Adobe Campaign Web include opzioni tecniche che consentono di configurare l&#39;applicazione in modo più specifico. Alcune di queste opzioni sono integrate, mentre altre possono essere aggiunte manualmente in base alle esigenze.

>[!IMPORTANT]
>Le opzioni incorporate sono preconfigurate e devono essere modificate solo da utenti avanzati. In caso di domande o richieste, contatta il rappresentante Adobe.

## Accedere alle opzioni di Campaign {#access}

Le opzioni sono disponibili dal menu **[!UICONTROL Amministrazione]** / **[!UICONTROL Opzioni]**. Utilizza il riquadro dei filtri per restringere l’elenco e individuare rapidamente l’opzione necessaria.

![](assets/options-list.png)\
[Elenco opzioni visualizzato nel menu Amministrazione / Opzioni]

>[!NOTE]
>Sebbene la posizione del menu delle opzioni differisca tra la console di Adobe Campaign e l’interfaccia utente Web, l’elenco è identico e funziona come un mirror. Per ulteriori dettagli sulle opzioni disponibili, consulta l&#39;elenco delle opzioni in [Documentazione di Campaign v7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

Nell&#39;elenco delle opzioni è possibile:

* **Duplicare o eliminare un&#39;opzione**: fare clic sul pulsante con i puntini di sospensione e selezionare l&#39;azione desiderata.
* **Modifica un&#39;opzione**: fare clic sul nome dell&#39;opzione per aprirne le proprietà. Apporta le modifiche e salva.
* **Creare un&#39;opzione personalizzata**: fare clic sul pulsante **[!UICONTROL Crea opzione]**.

## Creare un’opzione {#create}

L’interfaccia utente di Adobe Campaign Web consente di creare opzioni personalizzate per soddisfare le tue esigenze. Ciò è particolarmente utile quando si utilizzano attività del flusso di lavoro del **[!UICONTROL codice JavaScript]** per archiviare dati intermedi.

Per creare un&#39;opzione:

1. Accedere all&#39;elenco delle opzioni e fare clic su **[!UICONTROL Crea opzione]**.
1. Immettere un nome per l&#39;opzione, selezionarne il tipo e impostare il valore desiderato.
1. Fai clic su **[!UICONTROL Crea]** per creare l&#39;opzione.

![Crea un&#39;interfaccia di opzione che mostra i campi per nome, tipo e valore](assets/options-create.png)

Le opzioni possono fungere da memorizzazione temporanea dei dati, offrendo i seguenti vantaggi:

* Valori digitati: le opzioni supportano tipi di dati specifici, ad esempio date, numeri interi, stringhe e così via.
* Flessibilità: le opzioni consentono agli utenti di memorizzare e recuperare i dati in modo efficiente senza il sovraccarico di gestione delle tabelle del database.

Nell&#39;esempio seguente viene creata un&#39;opzione personalizzata denominata `sampleOption` con il valore iniziale &quot;a&quot;. Un&#39;attività **[!UICONTROL codice JavaScript]** in un flusso di lavoro modifica il valore di questa opzione e la memorizza in una variabile. Il valore aggiornato viene visualizzato nei registri del flusso di lavoro e riportato nel menu **[!UICONTROL Opzioni]**.

1. Crea l’opzione.

   ![Interfaccia di creazione opzione personalizzata con il nome `sampleOption` e il valore iniziale &quot;a&quot;](assets/options-sample-create.png)

1. Configura un&#39;attività **[!UICONTROL codice JavaScript]** e avvia il flusso di lavoro.

   ![Interfaccia di configurazione attività codice JavaScript](assets/options-sample-javascript.png)

1. Esegui il flusso di lavoro per visualizzare il valore aggiornato nei registri del flusso di lavoro.

   ![Registri del flusso di lavoro che mostrano il valore aggiornato dell&#39;opzione personalizzata](assets/options-sample-logs.png)

1. Il valore aggiornato è ora visibile nel menu **[!UICONTROL Opzioni]**.

   ![Il menu Opzioni visualizza il valore aggiornato dell&#39;opzione personalizzata](assets/options-sample-updated.png)
