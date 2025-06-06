---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro codice JavaScript
description: Scopri come utilizzare l’attività del flusso di lavoro del codice JavaScript
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 32%

---

# Codice JavaScript {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="Codice JavaScript"
>abstract="L’attività **Codice JavaScript** esegue uno script JavaScript nel contesto di un flusso di lavoro. Questo consente di eseguire azioni o raccogliere informazioni dal database. Utilizza attività del codice Java Script **semplici** per eseguire uno snippet di codice durante l’esecuzione del flusso di lavoro. Le attività Codice JavaScript **avanzate** consentono di eseguire operazioni più complesse eseguendo due diversi snippet di codice in modo sequenziale. La prima volta che viene avviato il flusso di lavoro, viene eseguita la prima chiamata. Ogni volta che il flusso di lavoro viene eseguito di nuovo, viene eseguito il codice definito nella seconda chiamata."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="Snippet JavaScript"
>abstract="Definisci lo script da eseguire durante l’esecuzione dell’attività. Se stai configurando un’attività di JavaScript **avanzata**, modifica due snippet di codice: il codice della prima chiamata da eseguire durante la prima esecuzione del flusso di lavoro e il codice della chiamata successiva da eseguire durante le esecuzioni successive del flusso di lavoro."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="Esecuzione JavaScript"
>abstract="Configura il ritardo di esecuzione per interrompere l’attività dopo un periodo di esecuzione. Per impostazione predefinita, la fase di esecuzione non può superare 1 ora. Dopo questo ritardo, il processo viene interrotto con un messaggio di errore e l’esecuzione dell’attività non riesce. Per ignorare questo limite, imposta il valore su 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Transizione JavaScript"
>abstract="Per aggiungere una o più transizioni di output, fai clic sul pulsante **[!UICONTROL Aggiungi transizioni]** e specifica un’etichetta e un nome interno per ogni transizione."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_processerrors"
>title="Errori del processo"
>abstract="Attiva l’opzione **[!UICONTROL Errori di processo]** per mantenere gli errori che si verificano durante l’esecuzione dello script in una transizione di output aggiuntiva."

L&#39;attività **codice JavaScript** è un&#39;attività **Gestione dati**. Utilizza questa attività per eseguire uno script JavaScript nel contesto di un flusso di lavoro. Ciò consente di raccogliere informazioni dal database o di eseguire altre operazioni complesse.

## Configurare l’attività del codice JavaScript {#javascript-code-configuration}

Per configurare l&#39;attività **codice JavaScript**, eseguire la procedura seguente:

1. Aggiungi un&#39;attività **codice JavaScript** al flusso di lavoro.

1. Scegli il tipo di attività da creare:

   * **Semplice**: eseguire uno snippet di codice.
   * **Avanzate**: esegui operazioni più avanzate eseguendo due diversi snippet di codice. [Scopri come configurare un&#39;attività JavaScript avanzata](#advanced)

   >[!NOTE]
   >
   >Con l&#39;interfaccia utente di Campaign Web, due attività sono state consolidate in una mediante l&#39;unione delle funzionalità del codice JavaScript **Semplice** e **Avanzate**. Questo consolidamento non influisce sulla funzionalità dell’attività.

1. Conferma, quindi fai clic sul pulsante **[!UICONTROL Modifica codice]** per aprire l&#39;editor espressioni. Il riquadro a sinistra fornisce sintassi predefinite che è possibile utilizzare per generare il codice, incluse le variabili evento. [Scopri come utilizzare le variabili evento e l&#39;editor di espressioni](../event-variables.md).

   ![Interfaccia dell&#39;editor di espressioni per l&#39;attività codice JavaScript](../assets/javascript-editor.png)

1. Nella sezione **[!UICONTROL Esecuzione]** configurare il ritardo per interrompere l&#39;attività dopo un periodo di esecuzione. Per impostazione predefinita, la fase di esecuzione non può superare 1 ora. Dopo questo ritardo, il processo viene interrotto con un messaggio di errore e l’esecuzione dell’attività non riesce. Per ignorare questo limite, imposta il valore su 0.

   ![Interfaccia di configurazione per il ritardo di esecuzione](../assets/javascript-config.png)

1. Attiva l’opzione **[!UICONTROL Errori di processo]** per mantenere gli errori che si verificano durante l’esecuzione dello script in una transizione di output aggiuntiva.

## Attività avanzate codice JavaScript {#advanced}

Le attività avanzate di JavaScript consentono di eseguire operazioni complesse. Queste attività ti consentono di:

* Eseguire due diversi snippet di codice. Il primo frammento di codice viene eseguito la prima volta che il flusso di lavoro viene avviato. Ogni volta che il flusso di lavoro viene eseguito di nuovo, viene eseguito lo snippet di codice definito nella seconda chiamata.
* Aggiungi più transizioni di output con cui puoi interagire in modo dinamico utilizzando uno script.

Per configurare un’attività di codice JavaScript avanzato, effettua le seguenti operazioni:

1. Seleziona il tipo **Avanzate**, quindi configura i frammenti di codice da eseguire:

   * Fai clic su **[!UICONTROL Modifica codice prima chiamata]** per definire lo script da eseguire durante la prima chiamata.
   * Fai clic su **[!UICONTROL Modifica codice chiamata successiva]** per definire lo script da eseguire durante le chiamate successive del flusso di lavoro. (facoltativo)

1. Per aggiungere una o più transizioni di output, fai clic sul pulsante **[!UICONTROL Aggiungi transizioni]** e specifica un’etichetta e un nome interno per ogni transizione.

   In questo esempio, due transizioni vengono configurate e attivate dallo script nel frammento di codice in base a condizioni specifiche.

   ![Esempio di transizioni configurate](../assets/javascript-transitions.png)

1. Completa la configurazione dell’attività e avvia il flusso di lavoro.

## Esempio {#javascript-code-example}

### Inizializzare le variabili in base alla popolazione in ingresso {#example1}

Questo esempio mostra come inizializzare una variabile in base al numero di profili interessati da un flusso di lavoro.

![Esempio di inizializzazione della variabile basata sul conteggio dei profili](../assets/javascript-example1.png)

In questo esempio, viene eseguito il targeting dei profili VIP del database. Viene creata una variabile denominata &quot;channel&quot; con un valore che dipende dal numero di profili target dell’attività Build audience:

* Se il targeting riguarda più di 1000 profili, inizializza la variabile con il valore &quot;e-mail&quot;.
* In caso contrario, inizializzalo con il valore &quot;sms&quot;.

Per ottenere questo risultato, segui questi passaggi:

1. Aggiungi un&#39;attività **Codice JavaScript** di tipo **Semplice** dopo l&#39;attività **Genera pubblico**.

1. Fai clic su **Modifica codice** e configura lo snippet di codice come mostrato di seguito:

   ```
   if (vars.recCount > 1000)
       vars.channel = "email";
   else
       vars.channel = "sms";
   ```

1. Avvia il flusso di lavoro. La variabile &quot;channel&quot; viene creata con il valore &quot;email&quot; o &quot;sms&quot;, a seconda del numero di profili interessati dall&#39;attività **Build audience**.

### Attiva le transizioni in base al valore di una variabile {#example2}

Questo esempio mostra come attivare una transizione basata sul valore di una variabile.

![Esempio di transizioni attivate dai valori delle variabili](../assets/javascript-example2-transitions.png)

In questo esempio, il flusso di lavoro inizia con un&#39;attività **External signal**, in cui viene passata una variabile (`interest`) da un altro flusso di lavoro. Il valore della variabile è &quot;in esecuzione&quot; o &quot;yoga&quot;, a seconda delle operazioni di filtro eseguite nel flusso di lavoro iniziale.

Vengono attivate diverse transizioni nel flusso di lavoro in base al valore della variabile.

Per ottenere questo risultato, segui questi passaggi:

1. Aggiungi un&#39;attività **Codice JavaScript** dopo l&#39;attività External signal con tipo **Avanzate**.

1. Aggiungi due transizioni: una per ogni possibile valore della variabile (&quot;in esecuzione&quot;, &quot;yoga&quot;).

1. Fai clic su **Modifica codice prima chiamata** e configura lo snippet di codice come mostrato di seguito:

   ```
   if (vars.interest == "running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Completa la configurazione di ciascuna transizione in base alle tue esigenze, quindi avvia il flusso di lavoro. Una delle due transizioni di output viene attivata in base al valore della variabile `interest` passata tramite l&#39;attività **External signal**.