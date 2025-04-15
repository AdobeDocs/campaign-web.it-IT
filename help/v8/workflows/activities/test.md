---
audience: end-user
title: Utilizzare l'attività Test workflow
description: Scopri come utilizzare l'attività Test workflow
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
>abstract="L&#39;attività **Test** può avere più transizioni di output. Durante l’esecuzione del flusso di lavoro, ogni condizione viene testata in sequenza fino a quando non ne viene soddisfatta una. Se nessuna delle condizioni è soddisfatta, il flusso di lavoro prosegue lungo il percorso della **[!UICONTROL condizione di impostazione predefinita]**. Se non è attivata alcuna condizione predefinita, il workflow si interrompe a questo punto."

L’attività **Test** è un’attività di **Controllo del flusso**. Consente di abilitare le transizioni in base a condizioni specificate.

## Configurare l&#39;attività di test {#test-configuration}

Per configurare l&#39;attività **di test** , effettuate le seguenti operazioni:

1. Aggiungi un&#39;attività **di test** al workflow.

1. Per impostazione predefinita, l&#39;attività **[!UICONTROL Test]** presenta un test booleano semplice. Se viene soddisfatta la condizione definita nel transizione &quot;True&quot;, viene attivata la transizione. In caso contrario, viene attivato un transizione predefinito &quot;False&quot;.

1. Per configurare la condizione associata a un transizione, fare clic sull&#39;icona **[!UICONTROL della finestra di dialogo]** Apri personalizzazione. Utilizzare l&#39;espressione editor per definire le regole necessarie per attivare questo transizione. È inoltre possibile utilizzare variabili di evento, condizioni e funzioni di data/ora. [Scopri come utilizzare le variabili di evento e l&#39;espressione editor](../event-variables.md).

   Modifica inoltre il **[!UICONTROL campo Etichetta]** per personalizzare il nome del transizione nell&#39;area di lavoro workflow.

   ![Configurazione predefinita dell&#39;attività di test](../assets/workflow-test-default.png)

1. Aggiungi più transizioni di output a un&#39;attività **[!UICONTROL di test]** . A tale scopo, fare clic sulla **[!UICONTROL pulsante Aggiungi condizione]** e configurare l&#39;etichetta e la condizione associata per ogni transizione.

1. Durante l’esecuzione del flusso di lavoro, ogni condizione viene testata in sequenza fino a quando non ne viene soddisfatta una. Se nessuna delle condizioni è soddisfatta, il flusso di lavoro prosegue lungo il percorso della **[!UICONTROL condizione di impostazione predefinita]**. Se non è attivata alcuna condizione predefinita, il workflow si interrompe a questo punto.

## Esempio {#example}

In questo esempio, vengono attivate transizioni diverse in base al numero di profili di destinazione di un&#39;attività **[!UICONTROL di creazione di pubblico]** :
* Se viene scelto come target più di 10.000 profili, viene inviato un messaggio e-mail.
* Per 1.000-10.000 profili, viene inviato un SMS.
* Se i profili con targeting scendono al di sotto di 1.000, vengono indirizzati a un transizione &quot;non contattare&quot;.

![Esempio di transizioni di attività di test](../assets/workflow-test-example.png)

Per raggiungere questo obiettivo, la `vars.recCount` variabile di evento viene utilizzata nelle condizioni &quot;email&quot; e &quot;sms&quot; per contare il numero di profili mirati e attivare il transizione appropriato.

![Configurazione dell&#39;esempio di attività Test](../assets/workflow-test-example-config.png)
