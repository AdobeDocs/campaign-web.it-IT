---
audience: end-user
title: Utilizzare l’attività External signal
description: Scopri come utilizzare l’attività del flusso di lavoro External signal
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 9%

---

# Segnale esterno {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Segnale esterno"
>abstract="L’attività **Segnale esterno** ti consente di attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Parametri del segnale esterno"
>abstract="Parametri del segnale esterno"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Trigger di fine"
>abstract="Trigger di fine"

L&#39;attività **External signal** è un&#39;attività **Flow control**. Consente di attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API.

>[!NOTE]
>
>In questa pagina sono descritti i passaggi principali per configurare un&#39;attività **[!UICONTROL External Signal]** nell&#39;interfaccia utente di Campaign Web e attivarla da un altro flusso di lavoro o da una chiamata API. Informazioni dettagliate su come attivare un flusso di lavoro e le relative best practice e come utilizzare le API di Campaign sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Segui questi passaggi per configurare l&#39;attività **External signal** e attivarne l&#39;esecuzione:

1. Aggiungi un&#39;attività **External signal** al flusso di lavoro.

1. Completa la configurazione del flusso di lavoro e avviane l’esecuzione. L&#39;attività **[!UICONTROL External Signal]** viene visualizzata come &quot;In sospeso&quot; in attesa di essere attivata.

   ![](../assets/external-signal-pending.png)

1. Recupera le informazioni seguenti:

   * Il nome interno del flusso di lavoro ****, visualizzato accanto alla relativa etichetta.

     +++Esempio di visualizzazione

     ![](../assets/external-signal-workflow-name.png)

+++

   * Il nome dell&#39;attività **External signal**, visualizzato nelle **[!UICONTROL opzioni di esecuzione]** del flusso di lavoro.

     +++Esempio di visualizzazione

     ![](../assets/external-signal-name.png)

+++

1. Per attivare il flusso di lavoro, è necessario eseguire la funzione JavaScript `PostEvent`. Questa funzione ti consente di trasmettere le variabili con i valori selezionati e di sfruttarle nel flusso di lavoro attivato.

   La funzione `PostEvent` può essere eseguita da un altro flusso di lavoro o da una chiamata API.

   * Per attivare un&#39;attività **[!UICONTROL External signal]** da un flusso di lavoro, eseguire la funzione PostEvent dal riquadro **[!UICONTROL Script di inizializzazione]**, accessibile dalle **[!UICONTROL opzioni di esecuzione]** dell&#39;attività. Per l&#39;attività **[!UICONTROL Codice JavaScript]**, eseguire la funzione dallo script dell&#39;attività.

     La sintassi è la seguente:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Esempio di visualizzazione

   In questo esempio viene attivata l’attività &quot;signal1&quot; External signal che è stata aggiunta al flusso di lavoro il cui nome interno è &quot;WKF12345&quot;. Stiamo inoltre trasmettendo una variabile denominata &quot;customID&quot;, con il valore &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Per attivare un&#39;attività **[!UICONTROL External signal]** da una chiamata API, segui i passaggi descritti nella documentazione API di Campaign. [Scopri come utilizzare il metodo `PostEvent` statico](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
