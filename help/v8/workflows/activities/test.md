---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro di test
description: Scopri come utilizzare l’attività del flusso di lavoro di test
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 29%

---


# Test {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Attività di test"
>abstract="L’attività **Test** è un’attività di **Controllo del flusso**. Consente di abilitare le transizioni in base a condizioni specificate."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Condizioni"
>abstract="L&#39;attività **Test** può avere più transizioni di output. Durante l’esecuzione del flusso di lavoro, ogni condizione viene testata in sequenza fino a quando non ne viene soddisfatta una. Se nessuna delle condizioni è soddisfatta, il flusso di lavoro prosegue lungo il percorso della **[!UICONTROL condizione di impostazione predefinita]**. Se non viene attivata alcuna condizione predefinita, il flusso di lavoro si interrompe a questo punto."

L’attività **Test** è un’attività di **Controllo del flusso**. Consente di abilitare le transizioni in base a condizioni specificate.

## Configurare l’attività di test {#test-configuration}

Per configurare l&#39;attività **Test**, eseguire la procedura seguente:

1. Aggiungi un&#39;attività **Test** al flusso di lavoro.

1. Per impostazione predefinita, l&#39;attività **[!UICONTROL Test]** presenta un semplice test booleano. Se la condizione definita nella transizione &quot;True&quot; è soddisfatta, la transizione viene attivata. In caso contrario, viene attivata una transizione predefinita &quot;False&quot;.

1. Per configurare la condizione associata a una transizione, fai clic sull&#39;icona **[!UICONTROL Apri finestra di personalizzazione]**. Utilizza l’editor di espressioni per definire le regole necessarie per attivare questa transizione. È inoltre possibile utilizzare variabili evento, condizioni e funzioni data/ora. [Scopri come utilizzare le variabili evento e l&#39;editor di espressioni](../event-variables.md).

   Inoltre, modifica il campo **[!UICONTROL Etichetta]** per personalizzare il nome della transizione nell&#39;area di lavoro del flusso di lavoro.

   ![Configurazione predefinita dell&#39;attività Test](../assets/workflow-test-default.png)

1. Aggiungere più transizioni di output a un&#39;attività **[!UICONTROL Test]**. A tale scopo, fare clic sul pulsante **[!UICONTROL Aggiungi condizione]** e configurare l&#39;etichetta e la condizione associata per ogni transizione.

1. Durante l’esecuzione del flusso di lavoro, ogni condizione viene testata in sequenza fino a quando non ne viene soddisfatta una. Se nessuna delle condizioni è soddisfatta, il flusso di lavoro prosegue lungo il percorso della **[!UICONTROL condizione di impostazione predefinita]**. Se non viene attivata alcuna condizione predefinita, il flusso di lavoro si interrompe a questo punto.

## Esempio {#example}

In questo esempio, vengono attivate transizioni diverse in base al numero di profili interessati da un&#39;attività **[!UICONTROL Genera pubblico]**:
* Se il targeting riguarda più di 10.000 profili, viene inviato un messaggio e-mail.
* Per un numero di profili compreso tra 1.000 e 10.000, viene inviato un SMS.
* Se i profili target scendono al di sotto di 1.000, vengono indirizzati a una transizione &quot;non contattare&quot;.

![Esempio di transizioni delle attività di test](../assets/workflow-test-example.png)

Per ottenere questo risultato, la variabile dell&#39;evento `vars.recCount` viene utilizzata nelle condizioni &quot;e-mail&quot; e &quot;sms&quot; per contare il numero di profili target e attivare la transizione appropriata.

![Configurazione dell&#39;esempio di attività di test](../assets/workflow-test-example-config.png)
