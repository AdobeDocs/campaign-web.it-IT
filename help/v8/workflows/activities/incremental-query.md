---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Incremental query
description: Scopri come utilizzare l’attività del flusso di lavoro Incremental query
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 19%

---

# Query incrementale {#incremental-query}



>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Query incrementale"
>abstract="La **Query incrementale** è un’attività di **Targeting** che consente di eseguire query sul database utilizzando il query modeler. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Cronologia della query incrementale"
>abstract="Cronologia della query incrementale"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Dati elaborati della query incrementale"
>abstract="Dati elaborati della query incrementale"

L&#39;attività **Incremental query** è un&#39;attività **Targeting** che consente di eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. Ciò ti consente di eseguire il targeting solo per nuovi elementi.

>[!NOTE]
>
>Mentre la console del client Campaign integra l&#39;attività **[!UICONTROL Incremental query]** con una pianificazione integrata, l&#39;interfaccia utente di Campaign Web tratta questa funzionalità separatamente. Per pianificare le esecuzioni di query incrementali, è necessario aggiungere un&#39;attività **[!UICONTROL Scheduler]** nel flusso di lavoro prima dell&#39;attività **[!UICONTROL Incremental query]**. [Scopri come configurare un&#39;attività Scheduler](scheduler.md)

L&#39;attività **[!UICONTROL Incremental query]** può essere utilizzata per vari tipi di utilizzi:

* Segmentazione di singoli utenti per definire il target di un messaggio, un pubblico, ecc.
* Esportazione dei dati. Ad esempio, puoi utilizzare l’attività per esportare regolarmente i nuovi registri in file. Può essere utile se desideri utilizzare i dati di registro in strumenti di reporting o BI esterni.

La popolazione già interessata dalle esecuzioni precedenti viene memorizzata nel flusso di lavoro. Ciò significa che due flussi di lavoro avviati dallo stesso modello non condividono lo stesso registro. Tuttavia, due attività basate sulla stessa query incrementale nello stesso flusso di lavoro utilizzano lo stesso registro.

Se il risultato di una query incrementale è uguale a 0 durante una delle esecuzioni, il flusso di lavoro viene sospeso fino alla successiva esecuzione programmata della query. Le transizioni e le attività che seguono la query incrementale non vengono quindi elaborate prima dell’esecuzione successiva.

## Configurare l’attività Incremental query {#incremental-query-configuration}

Segui questi passaggi per configurare l&#39;attività **Incremental query**:

![](../assets/incremental-query.png)

1. Aggiungi un&#39;attività **Incremental query** al flusso di lavoro.

1. Nella sezione **[!UICONTROL Pubblico]**, scegli la **dimensione di targeting**, quindi fai clic su **[!UICONTROL Continua]**.

   La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, iscritti, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions)

1. Utilizza il modellatore di query per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

1. Nella sezione **[!UICONTROL Dati elaborati]**, selezionare la modalità incrementale da utilizzare:

   * **[!UICONTROL Escludi risultati dell&#39;esecuzione precedente]**: ogni volta che l&#39;attività viene eseguita, i risultati delle esecuzioni precedenti vengono esclusi.

     I record già oggetto di targeting nelle esecuzioni precedenti possono essere registrati per un numero massimo di giorni dal giorno in cui sono stati oggetto di targeting. A tale scopo, utilizzare il campo **[!UICONTROL Cronologia in giorni]**. Se questo valore è zero, i destinatari non vengono mai eliminati dal registro.

   * **[!UICONTROL Utilizza un campo data]**: questa opzione ti consente di escludere i risultati di esecuzioni precedenti in base a un campo data specifico. A questo scopo, scegli il campo data desiderato dall’elenco di attributi disponibili per la dimensione di targeting selezionata. Nelle esecuzioni successive del flusso di lavoro, verranno recuperati solo i dati che sono stati modificati o creati dopo l’ultima data di esecuzione.

     Dopo la prima esecuzione del flusso di lavoro, diventa disponibile il campo **[!UICONTROL Data ultima esecuzione]**. Specifica la data che verrà utilizzata per l’esecuzione successiva e viene aggiornata automaticamente ogni volta che il flusso di lavoro viene eseguito. Puoi comunque ignorare questo valore immettendone manualmente uno nuovo in modo tale che sia adatto alle tue esigenze.

   >[!NOTE]
   >
   >La modalità **[!UICONTROL Utilizza un campo data]** consente una maggiore flessibilità a seconda del campo data selezionato. Ad esempio, se il campo specificato corrisponde a una data di modifica, la modalità campo data consente di recuperare i dati aggiornati di recente, mentre l’altra modalità esclude semplicemente le registrazioni che erano già state oggetto di targeting in un’esecuzione precedente, anche se sono state modificate dopo l’ultima esecuzione del flusso di lavoro.

## Esempio {#incremental-query-example}

L’esempio seguente mostra la configurazione di un flusso di lavoro che filtra ogni settimana i profili abbonati al servizio Yoga Newsletter nel database di Adobe Campaign, al fine di inviare loro un’e-mail di benvenuto.

![](../assets/incremental-query-example.png)

Il flusso di lavoro è costituito dai seguenti elementi:

* Un&#39;attività **[!UICONTROL Scheduler]**, per eseguire il flusso di lavoro ogni lunedì alle 6.
* Un&#39;attività **[!UICONTROL Incremental query]**, che esegue il targeting per tutti i sottoscrittori correnti durante la prima esecuzione, quindi solo per i nuovi sottoscrittori della settimana durante le esecuzioni successive.
* Un&#39;attività **[!UICONTROL Email delivery]**.
