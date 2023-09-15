---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Dividi
description: Scopri come utilizzare l’attività del flusso di lavoro Dividi
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 98%

---


# Dividi {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Attività Dividi"
>abstract="L’attività **Dividi** è un’attività di **Targeting** che consente di segmentare le popolazioni in ingresso in più sottoinsiemi in base a criteri di selezione diversi, ad esempio le regole di filtro o le dimensioni della popolazione."


L’attività **Dividi** è un’attività di **Targeting** che consente di segmentare le popolazioni in ingresso in più sottoinsiemi in base a criteri di selezione diversi, ad esempio le regole di filtro o le dimensioni della popolazione.

## Configurazione {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Dividi filtro attività"
>abstract="Per applicare una condizione di filtro al sottoinsieme, fai clic su **[!UICONTROL Crea filtro]** e configura la regola di filtro desiderata. Ad esempio, includi i profili della popolazione in ingresso il cui indirizzo e-mail esiste nel database."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Dividi limite attività"
>abstract="Per limitare il numero di profili selezionati dal sottoinsieme, attiva l’opzione **[!UICONTROL Abilita limite]** e specifica il numero o le percentuali della popolazione da includere."


Per configurare l’attività **Dividi** segui questi passaggi:

1. Aggiungi un’attività **Dividi** al flusso di lavoro.

1. Il riquadro di configurazione dell’attività si apre con un sottoinsieme predefinito. Fai clic sul pulsante **Aggiungi segmento** per aggiungere tutti i sottoinsiemi desiderati per segmentare la popolazione in ingresso.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Quando viene eseguita l’attività Dividi, la popolazione viene segmentata in diversi sottoinsiemi nell’ordine in cui vengono aggiunti all’attività. Ad esempio, se il primo sottoinsieme recupera il 70% della popolazione iniziale, il sottoinsieme aggiunto successivamente applicherà i propri criteri di selezione solo al restante 30% e così via.
   >
   > Prima di configurare i sottoinsiemi, accertati di averli aggiunti nell’ordine corretto, in quanto non è possibile modificarne la posizione.

1. Una volta aggiunti i sottoinsiemi, l’attività mostra tante transizioni di output quanti sono i sottoinsiemi. Si consiglia vivamente di modificare l’etichetta di ciascun sottoinsieme per identificarlo facilmente nell’area di lavoro del flusso di lavoro.

1. Configura in che modo ogni sottoinsieme deve filtrare la popolazione in ingresso. Per farlo, segui questi passaggi:

   1. Apri il sottoinsieme per visualizzarne le proprietà.

   1. Per applicare una condizione di filtro al sottoinsieme, fai clic su **[!UICONTROL Crea filtro]** e configura la regola di filtro desiderata. Ad esempio, includi i profili della popolazione in ingresso il cui indirizzo e-mail esiste nel database.

   1. Per limitare il numero di profili selezionati dal sottoinsieme, attiva l’opzione **[!UICONTROL Abilita limite]** e specifica il numero o le percentuali della popolazione da includere.

      >[!NOTE]
      >
      >Quando imposti un limite di popolazione per un sottoinsieme, puoi classificare i profili selezionati in base a un attributo di profilo specifico, in ordine crescente o decrescente. A tale scopo, attiva l’opzione **[!UICONTROL Abilita ordinamento]**. Ad esempio, puoi limitare un sottoinsieme in modo da includere solo i primi 50 profili con l’importo di acquisto più alto.

   ![](../assets/workflow-split-subset.png)

1. Dopo aver configurato tutti i sottoinsiemi, puoi selezionare la popolazione rimanente che non corrisponde a nessuno dei sottoinsiemi e includerli in un’ulteriore transizione in uscita. A tale scopo, attiva l’opzione **[!UICONTROL Genera complemento]**.

   ![](../assets/workflow-split-complement.png)

L’attività adesso è configurata. All’esecuzione del flusso di lavoro, la popolazione verrà segmentata in diversi sottoinsiemi, nell’ordine in cui sono stati aggiunti all’attività.

## Esempio

Nell’esempio seguente, l’attività **[!UICONTROL Dividi]** viene utilizzata per segmentare un pubblico in sottoinsiemi distinti in base al canale di comunicazione che si desidera utilizzare:

* **Sottoinsieme 1 “push”**: questo sottoinsieme comprende tutti i profili che hanno installato l’app mobile.
* **Sottoinsieme 2 “sms”**: utenti di telefoni cellulari. Per la popolazione rimanente che non rientrava nel sottoinsieme 1, il sottoinsieme 2 applica una regola di filtro per selezionare i profili con i telefoni cellulari nel database.
* **Transizione del complemento**: questa transizione acquisisce tutti i profili rimanenti che non corrispondono al sottoinsieme 1 o al sottoinsieme 2. In particolare, include i profili che non hanno installato l’app mobile e non dispongono di un telefono cellulare, ad esempio gli utenti che non hanno installato l’app mobile o non dispongono di un numero di cellulare registrato.

![](../assets/workflow-split-example.png)
