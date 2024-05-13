---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Incremental query
description: Scopri come utilizzare l’attività del flusso di lavoro Incremental query
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: fc872fd3975cd15a10845185c87152e2a473df8f
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 19%

---

# Query incrementale {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Attività query incrementale"
>abstract="Utilizza la nuova attività Incremental Query per eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Query incrementale"
>abstract="Il **Query incrementale** l&#39;attività è un **Targeting** che consente di eseguire query sul database utilizzando Query Modeler. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Cronologia della query incrementale"
>abstract="Cronologia della query incrementale"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Dati elaborati della query incrementale"
>abstract="Dati elaborati della query incrementale"

Il **Query incrementale** l&#39;attività è un **Targeting** attività che consente di eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi.

>[!NOTE]
>
>Mentre la console client di Campaign integra il **[!UICONTROL Query incrementale]** con un modulo di pianificazione integrato, l’interfaccia utente di Campaign Web tratta questa funzionalità separatamente. Per pianificare le esecuzioni di query incrementali, è necessario aggiungere una **[!UICONTROL Scheduler]** attività nel flusso di lavoro prima del **[!UICONTROL Query incrementale]** attività. [Scopri come configurare un’attività di pianificazione](scheduler.md)

Il **[!UICONTROL Query incrementale]** L’attività può essere utilizzata per vari tipi di utilizzi:

* Segmentazione di singoli utenti per definire il target di un messaggio, un pubblico, ecc.
* Esportazione dei dati. Ad esempio, puoi utilizzare l’attività per esportare regolarmente i nuovi registri in file. Può essere utile se desideri utilizzare i dati di registro in strumenti di reporting o BI esterni.

La popolazione già interessata dalle esecuzioni precedenti viene memorizzata nel flusso di lavoro. Ciò significa che due flussi di lavoro avviati dallo stesso modello non condividono lo stesso registro. Tuttavia, due attività basate sulla stessa query incrementale nello stesso flusso di lavoro utilizzano lo stesso registro.

Se il risultato di una query incrementale è uguale a 0 durante una delle esecuzioni, il flusso di lavoro viene sospeso fino alla successiva esecuzione programmata della query. Le transizioni e le attività che seguono la query incrementale non vengono quindi elaborate prima dell’esecuzione successiva.

## Configurare l’attività Incremental query {#incremental-query-configuration}

Per configurare il **Query incrementale** attività:

![](../assets/incremental-query.png)

1. Aggiungi un **Query incrementale** attività nel flusso di lavoro.

1. In **[!UICONTROL Pubblico]** , scegli il **Dimensione targeting** quindi fai clic su **[!UICONTROL Continua]**.

   La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, iscritti, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions)

1. Utilizza il modellatore di query per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

1. In **[!UICONTROL Dati elaborati]** selezionare la modalità incrementale da utilizzare:

   * **[!UICONTROL Escludi risultati dell’esecuzione precedente]**: ogni volta che l’attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi.

     I record già oggetto di targeting nelle esecuzioni precedenti possono essere registrati per un numero massimo di giorni dal giorno in cui sono stati oggetto di targeting. A tale scopo, utilizza **[!UICONTROL Cronologia in giorni]** campo. Se questo valore è zero, i destinatari non vengono mai eliminati dal registro.

   * **[!UICONTROL Utilizza un campo data]**: questa opzione ti consente di escludere i risultati delle esecuzioni precedenti in base a un campo data specifico. A questo scopo, scegli il campo data desiderato dall’elenco di attributi disponibili per la dimensione di targeting selezionata. Nelle esecuzioni successive del flusso di lavoro, verranno recuperati solo i dati che sono stati modificati o creati dopo l’ultima data di esecuzione.

     Dopo la prima esecuzione del workflow, il **[!UICONTROL Data ultima esecuzione]** diventa disponibile. Specifica la data che verrà utilizzata per l’esecuzione successiva e viene aggiornata automaticamente ogni volta che il flusso di lavoro viene eseguito. Puoi comunque ignorare questo valore immettendone manualmente uno nuovo in modo tale che sia adatto alle tue esigenze.

   >[!NOTE]
   >
   >Il **[!UICONTROL Utilizza un campo data]** consente una maggiore flessibilità a seconda del campo data selezionato. Ad esempio, se il campo specificato corrisponde a una data di modifica, la modalità campo data consente di recuperare i dati aggiornati di recente, mentre l’altra modalità esclude semplicemente le registrazioni che erano già state oggetto di targeting in un’esecuzione precedente, anche se sono state modificate dopo l’ultima esecuzione del flusso di lavoro.

## Esempio {#incremental-query-example}

L’esempio seguente mostra la configurazione di un flusso di lavoro che filtra ogni settimana i profili abbonati al servizio Yoga Newsletter nel database di Adobe Campaign, al fine di inviare loro un’e-mail di benvenuto.

![](../assets/incremental-query-example.png)

Il flusso di lavoro è costituito dai seguenti elementi:

* A **[!UICONTROL Scheduler]** per eseguire il flusso di lavoro ogni lunedì alle 6.
* Un **[!UICONTROL Query incrementale]** attività, che esegue il targeting per tutti gli abbonati correnti durante la prima esecuzione, quindi solo per i nuovi abbonati della settimana durante le esecuzioni successive.
* Un **[!UICONTROL Consegna e-mail]** attività.
