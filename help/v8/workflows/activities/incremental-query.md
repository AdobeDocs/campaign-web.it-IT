---
audience: end-user
title: Utilizzare l'attività Query workflow incrementale
description: Scopri come utilizzare l'attività di workflow query incrementale
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 11%

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

L&#39;attività **Incremental query** è un&#39;attività **Targeting** che consente di eseguire query sul database su base pianificata. Ogni volta che questa attività viene eseguita, i risultati delle esecuzioni precedenti sono esclusi. In questo modo è possibile destinazione solo nuovi elementi.

>[!NOTE]
>
>Mentre la console client Campaign integra l&#39;attività **[!UICONTROL di query]** incrementale con uno scheduler incorporato, l&#39;interfaccia utente Web Campaign tratta questa funzionalità separatamente. Per programmare l&#39;esecuzione di query incrementali, aggiungere un&#39;attività **[!UICONTROL di pianificazione]** nel workflow prima dell&#39;attività **[!UICONTROL di query]** incrementale. [Scopri come configurare un&#39;attività del modulo di pianificazione](scheduler.md)

L&#39;attività **[!UICONTROL di query]** incrementale può essere utilizzata per vari scopi:

* Segmentazione di individui per definire la destinazione di un messaggio, un pubblico o altre operazioni.
* Esportazione dei dati. Ad esempio, utilizza l’attività per esportare regolarmente i nuovi registri in file. Questa funzione è utile per la generazione di rapporti esterni o per gli strumenti di business intelligence.

La popolazione già interessata dalle esecuzioni precedenti viene memorizzata nel flusso di lavoro. Due flussi di lavoro avviati dallo stesso modello non condividono lo stesso registro. Tuttavia, due attività basate sulla stessa query incrementale nello stesso flusso di lavoro utilizzano lo stesso registro.

Se il risultato di una query incrementale è uguale a 0 durante una delle esecuzioni, il flusso di lavoro viene sospeso fino alla successiva esecuzione programmata della query. Le transizioni e le attività che seguono la query incrementale non vengono elaborate prima dell’esecuzione successiva.

## Configurare l’attività Incremental query {#incremental-query-configuration}

Per configurare l&#39;attività **di query** incrementale, effettuate le seguenti operazioni:

[Descrizione: schermata che mostra l&#39;interfaccia di configurazione per l&#39;attività di query incrementale in Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Aggiungi un&#39;attività **di query** incrementale al workflow.

1. **[!UICONTROL Nella sezione Pubblico]**, scegli la **dimensione** Targeting, quindi fai clic su **[!UICONTROL Continua]**.

   La dimensione di targeting definisce la popolazione target dell’operazione, ad esempio destinatari, beneficiari del contratto, operatori o abbonati. Per impostazione predefinita, il target viene selezionato dai destinatari. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions)

1. Utilizza il modellatore di query per definire la query, in modo analogo a come si crea un pubblico durante la progettazione di una nuova e-mail. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

1. Nella sezione **[!UICONTROL Dati elaborati]**, selezionare la modalità incrementale da utilizzare:

   * **[!UICONTROL Escludi risultati dell&#39;esecuzione precedente]**: ogni volta che l&#39;attività viene eseguita, i risultati delle esecuzioni precedenti vengono esclusi.

     I record già oggetto di targeting nelle esecuzioni precedenti possono essere registrati per un numero massimo di giorni dal giorno in cui sono stati oggetto di targeting. Utilizza il campo **[!UICONTROL Cronologia in giorni]** per impostare questo valore. Se questo valore è zero, i destinatari non vengono mai eliminati dal registro.

   * **[!UICONTROL Usa un campo]** data: questa opzione esclude i risultati di esecuzioni precedenti basate su un campo data specifico. Scegliete il campo data desiderato dall&#39;elenco di attributi disponibili per la dimensione targeting selezionata. Nelle esecuzioni successive del workflow, verranno recuperati solo i dati modificati o creati dopo l&#39;ultima data di esecuzione.

     Dopo la prima esecuzione del workflow, diventa disponibile il **[!UICONTROL campo Data]** ultima esecuzione. Specifica la data utilizzata per l&#39;esecuzione successiva e viene aggiornato automaticamente ogni volta che viene eseguito il workflow. È possibile eseguire manualmente l&#39;override di questo valore in base alle proprie esigenze.

   >[!NOTE]
   >
   >La modalità **[!UICONTROL Utilizza un campo data]** offre maggiore flessibilità a seconda del campo data selezionato. Ad esempio, se il campo specificato corrisponde a una data di modifica, la modalità campo data recupera i dati aggiornati di recente. L&#39;altra modalità esclude le registrazioni già incluse in un&#39;esecuzione precedente, anche se sono state modificate dopo l&#39;ultima esecuzione del flusso di lavoro.

## Esempio {#incremental-query-example}

L’esempio seguente mostra la configurazione di un flusso di lavoro che filtra i profili nel database di Adobe Campaign ogni settimana. Si rivolge alle persone abbonate al servizio newsletter Yoga e invia loro un’e-mail di benvenuto.

![Schermata di un esempio di configurazione del flusso di lavoro per filtrare i profili abbonati al servizio newsletter Yoga.](../assets/incremental-query-example.png)

Il flusso di lavoro include i seguenti elementi:

* Un&#39;attività **[!UICONTROL di pianificazione]** , che esegue il workflow ogni lunedì alle 6 del mattino.
* Un&#39;attività **[!UICONTROL di query]** incrementale, che indirizza tutti i sottoscrittori correnti durante la prima esecuzione e solo i nuovi sottoscrittori durante le esecuzioni successive.
* Un&#39;attività **[!UICONTROL di recapito]** e-mail.