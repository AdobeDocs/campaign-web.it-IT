---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Codice JavaScript
description: Scopri come utilizzare l’attività del flusso di lavoro del codice JavaScript
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# Codice JavaScript {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="Codice JavaScript"
>abstract="Il **Codice JavaScript** attività ti consente di eseguire uno script JavaScript nel contesto di un flusso di lavoro. Questo consente di eseguire azioni o raccogliere informazioni dal database. Utilizzare **Semplice** Attività di codice JavaScript per eseguire un frammento di codice all’esecuzione del flusso di lavoro. **Avanzate** Le attività di codice JavaScript consentono di eseguire operazioni più complesse eseguendo due diversi snippet di codice in ordine sequenziale. La prima volta che viene avviato il flusso di lavoro, viene eseguita la prima chiamata. Ogni volta che il flusso di lavoro viene eseguito di nuovo, viene eseguito il codice definito nella seconda chiamata."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="Snippet JavaScript"
>abstract="Definisci lo script da eseguire durante l’esecuzione dell’attività. Se stai configurando un’ **Avanzate** Attività JavaScript, devi modificare due snippet di codice: il primo codice di chiamata da eseguire alla prima esecuzione del flusso di lavoro e il codice di chiamata successivo da eseguire alle chiamate successive del flusso di lavoro."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="Esecuzione JavaScript"
>abstract="Configura il ritardo di esecuzione per interrompere l’attività dopo un periodo di esecuzione. Per impostazione predefinita, la fase di esecuzione non può superare 1 ora. Dopo questo ritardo, il processo viene interrotto con un messaggio di errore e l’esecuzione dell’attività non riesce. Per ignorare questo limite, imposta il valore su 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Transizione JavaScript"
>abstract="Per aggiungere più transizioni di output, fare clic sul pulsante **[!UICONTROL Aggiungere transizioni]** pulsante. Ciò ti consente, ad esempio, di attivare una transizione specifica basata su una condizione specifica definita nell’attività del codice JavaScript. Questa opzione è disponibile per **Avanzate** Solo attività di codice JavaScript."

Il **Codice JavaScript** l&#39;attività è un **Gestione dei dati** attività. Utilizza questa attività per eseguire uno script JavaScript nel contesto di un flusso di lavoro. Questo consente di raccogliere informazioni dal database o di eseguire altre operazioni complesse.

## Configurare l’attività del codice JavaScript {#javascript-code-configuration}

Per configurare il **Codice JavaScript** attività:

1. Aggiungi un **Codice JavaScript** attività nel flusso di lavoro.

1. Scegli il tipo di attività da creare:

   * **Semplice**: esegui un frammento di codice.
   * **Avanzate**: questa opzione consente di eseguire operazioni più avanzate eseguendo due diversi snippet di codice. [Scopri come configurare un’attività JavaScript avanzata](#advanced)

   >[!NOTE]
   >
   >Con l’interfaccia utente di Campaign Web, abbiamo consolidato due attività in una unendo entrambe **Semplice** e **Avanzate** Funzionalità del codice JavaScript. Questo consolidamento non influisce in alcun modo sulla funzionalità dell’attività.

1. Conferma quindi fai clic su **[!UICONTROL Modifica codice]** per aprire l’editor di espressioni. Il riquadro a sinistra fornisce sintassi predefinite che è possibile utilizzare per creare il codice, incluse le variabili evento. [Scopri come utilizzare le variabili evento e l’editor di espressioni](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. In **[!UICONTROL Esecuzione]** , configura il ritardo per arrestare l&#39;attività dopo un periodo di esecuzione. Per impostazione predefinita, la fase di esecuzione non può superare 1 ora. Dopo questo ritardo, il processo viene interrotto con un messaggio di errore e l’esecuzione dell’attività non riesce. Per ignorare questo limite, imposta il valore su 0.

   ![](../assets/javascript-config.png)

1. Attiva **[!UICONTROL Errori di processo]** per mantenere gli errori che si verificano durante l’esecuzione dello script in una transizione di output aggiuntiva.

## Attività di codice JavaScript avanzate {#advanced}

Le attività JavaScript avanzate consentono di eseguire operazioni complesse. Consente di:

* Eseguire due diversi snippet di codice. Il primo frammento di codice viene eseguito la prima volta che il flusso di lavoro viene avviato. Ogni volta che il flusso di lavoro viene eseguito di nuovo, viene eseguito lo snippet di codice definito nella seconda chiamata.
* Aggiungi più transizioni di output con cui puoi interagire in modo dinamico utilizzando uno script.

Per configurare un’attività di codice JavaScript avanzato, effettua le seguenti operazioni:

1. Seleziona la **Avanzate** digita, quindi configura gli snippet di codice da eseguire:

   * Clic **[!UICONTROL Modifica il codice della prima chiamata]** per definire lo script da eseguire durante la prima chiamata.
   * Clic **[!UICONTROL Modifica il codice della chiamata successiva]** per definire lo script da eseguire durante le chiamate successive del flusso di lavoro. (facoltativo)

1. Per aggiungere una o più transizioni di output, fare clic sul pulsante **[!UICONTROL Aggiungere transizioni]** e specifica un’etichetta e un nome interno per ciascuna transizione.

   In questo esempio abbiamo configurato due transizioni che vengono attivate dallo script nel frammento di codice in base a condizioni specifiche.

   ![](../assets/javascript-transitions.png)

1. Completa la configurazione dell’attività e avvia il flusso di lavoro.

## Esempio {#javascript-code-example}

### Inizializzare le variabili in base alla popolazione in ingresso {#example1}

Questo esempio mostra come inizializzare una variabile in base al numero di profili interessati da un flusso di lavoro.

![](../assets/javascript-example1.png)

In questo caso, eseguiamo il targeting dei profili VIP dal nostro database. Vogliamo creare una variabile denominata &quot;channel&quot; con un valore che dipende dal numero di profili target dell’attività Build audience:

* Se il targeting riguarda più di 1000 profili, inizializza la variabile con il valore &quot;e-mail&quot;.
* In caso contrario, inizializzalo con il valore &quot;sms&quot;.

Per farlo, segui questi passaggi:

1. Aggiungi un **Codice JavaScript** attività con il tipo **Semplice** dopo il **Creare un pubblico** attività.

1. Clic **Modifica codice** e configura lo snippet di codice come segue:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Avvia il flusso di lavoro. La variabile &quot;channel&quot; viene creata con il valore &quot;email&quot; o &quot;sms&quot;, a seconda del numero di profili interessati dal **Creare un pubblico** attività.

### Attiva le transizioni in base al valore di una variabile {#example2}

Questo esempio mostra come attivare una transizione basata sul valore di una variabile.

![](../assets/javascript-example2-transitions.png)

In questo caso, il flusso di lavoro inizia con **Segnale esterno** attività, in cui una variabile (`interest`) viene passato da un altro flusso di lavoro. Il valore della variabile è &quot;in esecuzione&quot; o &quot;yoga&quot;, a seconda delle operazioni di filtro eseguite nel flusso di lavoro iniziale.

Vogliamo attivare diverse transizioni nel flusso di lavoro, in base al valore della variabile.

Per farlo, segui questi passaggi:

1. Aggiungi un **Codice JavaScript** attività dopo l’attività External signal con il tipo **Avanzate**.

1. Aggiungi due transizioni: una per ogni possibile valore della variabile (&quot;in esecuzione&quot;, &quot;yoga&quot;).

1. Clic **Modifica il codice della prima chiamata** e configura lo snippet di codice come segue:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Completa la configurazione di ciascuna transizione in base alle tue esigenze, quindi avvia il flusso di lavoro. Viene attivata una delle due transizioni di output, in base al valore della `interest` variabile passata tramite **Segnale esterno** attività.
