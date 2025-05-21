---
audience: end-user
title: Variabili evento del flusso di lavoro
description: Scopri come sfruttare le variabili evento nei flussi di lavoro.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Variabili evento del flusso di lavoro {#event-variables}

Alcune attività del flusso di lavoro consentono di modificare gli script nell’editor di espressioni per eseguire azioni specifiche, ad esempio recuperare dati da attività precedenti, creare condizioni o calcolare nomi di file in base a variabili evento.

## Cosa sono le variabili evento {#scripting}

Gli script eseguiti nel contesto di un flusso di lavoro accedono a una serie di **oggetti** globali aggiuntivi, ad esempio il flusso di lavoro stesso in esecuzione (`instance`), le varie attività (`task`) o gli eventi che hanno attivato una determinata attività (`event`).

Ogni tipo di **oggetto** è associato a una categoria di **variabili** che è possibile utilizzare nell&#39;editor espressioni durante la modifica di script in attività, ad esempio **[!UICONTROL codice JavaScript]** o **[!UICONTROL Test]**.

* **Le variabili di istanza** (`instance.vars.xxx`) sono paragonabili alle variabili globali. Sono condivise da tutte le attività.
* **Le variabili attività** (`task.vars.xxx`) sono paragonabili alle variabili locali. Vengono utilizzati solo dall&#39;attività corrente. Queste variabili vengono utilizzate dalle attività persistenti per conservare i dati e talvolta vengono utilizzate per scambiare dati tra i diversi script della stessa attività.
* **Le variabili evento** (`vars.xxx`) consentono lo scambio di dati tra le attività elementari di un processo di workflow. Queste variabili vengono passate dall&#39;attività che ha attivato l&#39;attività in corso. Vengono quindi passate alle seguenti attività. **Le variabili evento** sono le variabili più comunemente utilizzate e devono essere utilizzate al posto delle variabili di istanza.

>[!NOTE]
>
>Ulteriori informazioni sugli script e sugli oggetti e le variabili esposti in Adobe Campaign sono disponibili nella documentazione di Campaign v8 (console client) in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Tieni presente che questa risorsa offre informazioni importanti, ma potrebbero esistere delle discrepanze in quanto si applica specificamente alla console client anziché all’interfaccia utente web di Campaign.

## Sfruttare le variabili di evento nell’editor di espressioni {#expression-editor}

Le variabili di evento predefinite sono disponibili per l’utilizzo nel riquadro a sinistra dell’editor di espressioni. Puoi anche crearne di nuovi inizializzando una nuova variabile nel codice.

![Schermata che mostra le variabili evento predefinite nel riquadro laterale sinistro dell&#39;editor di espressioni](assets/event-variables.png)

Oltre a queste variabili evento, puoi anche utilizzare il menu **[!UICONTROL Condizioni]** nel riquadro a sinistra per creare le condizioni e il menu **[!UICONTROL Aggiungi data corrente]** per applicare le funzioni relative alla formattazione della data.