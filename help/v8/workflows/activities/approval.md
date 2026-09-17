---
audience: end-user
title: Attività del flusso di lavoro di approvazione
description: Scopri come utilizzare l’attività del flusso di lavoro di approvazione
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 3%
---
# Approvazione {#approval}

>[!CONTEXTUALHELP]
>id="acw_orchestration_approval"
>title="Attività di approvazione"
>abstract="L&#39;attività **Approval** richiede la partecipazione di un operatore. Assegna l’attività a un gruppo o a un singolo operatore, personalizza il titolo e il messaggio della notifica e definisci le possibili risposte come rami di output."

L&#39;attività del flusso di lavoro **Approvazione** ti consente di assegnare un&#39;attività a un gruppo o a un singolo operatore, personalizzare il titolo e il messaggio dell&#39;e-mail di notifica e definire le possibili risposte (ad esempio Sì/No) come rami di output.

Utilizza questa attività ogni volta che un passaggio nel flusso di lavoro richiede una decisione umana prima di continuare, ad esempio per ottenere l’approvazione per un budget, un pubblico di destinazione o un contenuto, prima che il flusso di lavoro proceda.

## Funzionamento del processo di approvazione {#process}

Richiede la partecipazione di almeno un operatore. Questa attività non blocca il flusso di lavoro: è possibile eseguire altre attività mentre il flusso di lavoro attende una risposta.

In attesa di risposta, l’attività viene visualizzata come in sospeso nell’area di lavoro. L’assegnatario risponde utilizzando il collegamento incluso nel messaggio di notifica.

Di seguito è riportato il processo dell&#39;attività di approvazione:

1. Crea un flusso di lavoro e configura un&#39;attività **Approval**.
1. Avvia il flusso di lavoro. Quando raggiunge l&#39;attività **Approval**, viene creata un&#39;attività per l&#39;assegnatario.
1. L’assegnatario riceve il messaggio di notifica, fa clic sul collegamento e seleziona una risposta.
1. Una volta che l’assegnatario risponde, il flusso di lavoro continua attraverso la transizione che corrisponde alla propria risposta.

Per configurare questa attività, effettua le seguenti operazioni:

1. Assegna l&#39;attività, [leggi tutto](#assignment)
1. Definisci il messaggio di notifica, [ulteriori informazioni](#message)
1. Definisci le risposte possibili, [ulteriori informazioni](#answers)
1. Facoltativamente, definire una scadenza, [ulteriori informazioni](#expiration)

## Assegna l’attività {#assignment}

L’assegnazione del task a un gruppo o a un operatore è obbligatoria: viene visualizzato un avviso fino a quando non lo fai.

![Schermata che mostra la sezione Assegnazione dell&#39;attività Approvazione](../assets/workflow-approval1.png){zoomable="yes"}

Segui questi passaggi:

1. Nel campo **[!UICONTROL Tipo di assegnazione]**, scegliere se l&#39;attività è assegnata a un **[!UICONTROL Gruppo]** (impostazione predefinita) o a un **[!UICONTROL Operatore]**.

1. Selezionare quindi **[!UICONTROL Gruppo]** (di operatori) o **[!UICONTROL Operatore]** (operatore singolo).

1. Abilita **[!UICONTROL Approvazione multipla]** se desideri che ogni assegnatario risponda prima che il flusso di lavoro continui. Questa opzione è disponibile indipendentemente dal tipo di assegnazione. Se disabilitato, il flusso di lavoro continua non appena un assegnatario risponde e tale risposta è quella presa in considerazione.

1. Fai clic su **[!UICONTROL Parametri avanzati]** per selezionare il modello di consegna utilizzato per la notifica. Per impostazione predefinita, viene utilizzato un modello incorporato, ma puoi selezionare qualsiasi altro modello di consegna.

   ![Schermata che mostra i parametri avanzati dell&#39;attività Approval](../assets/workflow-approval1bis.png){zoomable="yes"}

## Definire il messaggio di notifica {#message}

Ora puoi definire il messaggio di notifica inviato all’assegnatario.

![Schermata che mostra la sezione Messaggio dell&#39;attività Approvazione](../assets/workflow-approval2.png){zoomable="yes"}

Segui questi passaggi:

1. Definisci il **[!UICONTROL Titolo]** della notifica inviata all&#39;assegnatario.

1. Definisci il **[!UICONTROL Messaggio]** della notifica inviata all&#39;assegnatario.

Entrambi i campi supportano la personalizzazione: fai clic sull&#39;icona di personalizzazione per inserire le variabili evento, ad esempio l&#39;operatore **[!UICONTROL che ha risposto]** e la **[!UICONTROL risposta]**, che puoi riutilizzare in un&#39;altra posizione nel flusso di lavoro.

![Schermata che mostra la personalizzazione del messaggio](../assets/workflow-approval2bis.png){zoomable="yes"}

## Definire le risposte possibili {#answers}

L&#39;attività include due risposte predefinite, **[!UICONTROL Sì]** e **[!UICONTROL No]**. Ogni risposta corrisponde a una transizione di output nell’area di lavoro.

![Schermata che mostra la sezione Risposte dell&#39;attività Approvazione](../assets/workflow-approval3.png){zoomable="yes"}

Fai clic su **[!UICONTROL Aggiungi risposta]** per definire ulteriori scelte.

Quando l’assegnatario risponde, il flusso di lavoro continua attraverso la transizione corrispondente alla sua scelta.

## Definire una scadenza {#expiration}

Infine, puoi definire una scadenza per l’attività di approvazione. Analogamente a una risposta, una scadenza attiva la propria transizione di output se l’assegnatario non ha risposto entro la scadenza.

![Schermata che mostra la sezione Scadenza dell&#39;attività di approvazione](../assets/workflow-approval4.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Aggiungi scadenza]**.

1. Definisci un **[!UICONTROL Etichetta]** per la transizione di output corrispondente.

1. Nell&#39;elenco a discesa **[!UICONTROL Tipo di scadenza]** scegliere una delle opzioni seguenti:

   * **[!UICONTROL Ritardo dopo l&#39;inizio dell&#39;attività]**: definire un ritardo di attesa dopo l&#39;inizio dell&#39;attività di approvazione.
   * **[!UICONTROL Ritardo dopo una data]**: definisci un ritardo di attesa dopo una data specifica.
   * **[!UICONTROL Ritardo prima di una data]**: definisci un ritardo di attesa prima di una data specifica.
   * **[!UICONTROL Scadenza calcolata dallo script]**: utilizzare uno script per calcolare la scadenza.

1. Abilita **[!UICONTROL Non terminare l&#39;attività]** se desideri attivare la transizione di scadenza senza terminare l&#39;attività di approvazione, in modo che l&#39;assegnatario possa ancora rispondere in seguito.

Puoi definire più scadenze per la stessa attività di approvazione.

A questo punto puoi avviare il flusso di lavoro. Una volta che l’assegnatario risponde, il flusso di lavoro continua attraverso la transizione che corrisponde alla propria risposta. [Ulteriori informazioni](#process)

## Argomenti correlati {#related}

* [Informazioni sulle attività dei flussi di lavoro](about-activities.md)
* [Configurare e gestire il processo di approvazione](../../campaigns/campaign-approvals.md)
