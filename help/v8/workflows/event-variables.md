---
audience: end-user
title: Variabili evento flusso di lavoro
description: Scopri come sfruttare le variabili evento nei flussi di lavoro.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: c3f04d3828f22207bd5e9a0e8c334e8f7a57b2c1
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Variabili evento flusso di lavoro {#event-variables}

Alcune attività del flusso di lavoro consentono di modificare gli script nell’editor di espressioni per eseguire azioni specifiche, ad esempio recuperare dati provenienti da attività precedenti, creare condizioni o calcolare nomi di file in base a variabili evento.

## Cosa sono le variabili evento {#scripting}

Gli script eseguiti nel contesto di un workflow accedono a una serie di **oggetti** ad esempio il flusso di lavoro stesso in esecuzione (`ìnstance`), le sue varie attività (`task`) o gli eventi che hanno attivato una determinata attività (`event`).

A ogni tipo di **oggetto** è associato a una categoria di **Variabili** che possono essere utilizzate nell’editor espressioni durante la modifica di script in attività come **[!UICONTROL Codice JavaScript]** o **[!UICONTROL Test]**.

* **Variabili di istanza** (`instance.vars.xxx`) sono paragonabili alle variabili globali. Sono condivise da tutte le attività.
* **Variabili attività** (`task.vars.xxx`) sono paragonabili a variabili locali. Vengono utilizzati solo dall&#39;attività corrente. Queste variabili vengono utilizzate dalle attività persistenti per conservare i dati e talvolta vengono utilizzate per scambiare dati tra i diversi script di una stessa attività.
* **Variabili evento** (`vars.xxx`) consente lo scambio di dati tra le attività elementari di un processo del flusso di lavoro. Queste variabili vengono passate dall&#39;attività che ha attivato l&#39;attività in corso. Vengono quindi passate alle seguenti attività. **Variabili evento** sono le variabili utilizzate più di frequente e devono essere utilizzate al posto delle variabili di istanza.

>[!NOTE]
>
>Ulteriori informazioni sugli script e sugli oggetti e le variabili esposti in Adobe Campaign sono disponibili nella documentazione di Campaign v8 (console client) in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Tieni presente che questa risorsa offre informazioni importanti, ma potrebbero esistere delle discrepanze in quanto si applica specificamente alla console client anziché all’interfaccia utente web di Campaign.

## Sfruttare le variabili di evento nell’editor di espressioni {#expression-editor}

Le variabili di evento predefinite sono disponibili per l’utilizzo nel riquadro a sinistra dell’editor di espressioni. Puoi anche crearne di nuovi inizializzando una nuova variabile nel codice.

![](assets/event-variables.png)

Oltre a queste variabili evento, puoi anche sfruttare **[!UICONTROL Condizioni]** nel riquadro a sinistra per creare le condizioni e il **[!UICONTROL Aggiungi data corrente]** per utilizzare le funzioni relative alla formattazione della data.
