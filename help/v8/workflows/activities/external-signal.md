---
audience: end-user
title: Utilizzare l’attività External signal
description: Scopri come utilizzare l’attività del flusso di lavoro External signal
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 8%

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

L&#39;attività **External signal** è un&#39;attività **Flow control**. Ti consente di attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API.

>[!NOTE]
>
>In questa pagina vengono illustrati i passaggi principali per configurare un&#39;attività **[!UICONTROL External Signal]** nell&#39;interfaccia utente di Campaign Web e attivarla da un altro flusso di lavoro o da una chiamata API. Informazioni dettagliate su come attivare un flusso di lavoro, sulle best practice e su come utilizzare le API di Campaign sono disponibili nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/it/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example).

Segui questi passaggi per configurare l&#39;attività **External signal** e attivarne l&#39;esecuzione:

1. Aggiungi un&#39;attività **External signal** al flusso di lavoro.

1. Completa la configurazione del flusso di lavoro e avviane l’esecuzione. L&#39;attività **[!UICONTROL External Signal]** viene visualizzata come &quot;In sospeso&quot; in attesa di essere attivata.

   ![La schermata mostra l&#39;attività External Signal in uno stato in sospeso.](../assets/external-signal-pending.png)

1. Recupera le seguenti informazioni:

   * Il nome interno del flusso di lavoro **&#x200B;**, visualizzato accanto alla relativa etichetta.

     +++Visualizza esempio

     ![La schermata mostra il nome interno del flusso di lavoro accanto alla relativa etichetta.](../assets/external-signal-workflow-name.png)

     +++

   * Il nome dell&#39;attività **External signal**, visualizzato nelle **[!UICONTROL opzioni di esecuzione]** del flusso di lavoro.

     +++Visualizza esempio

     ![La schermata mostra il nome dell&#39;attività External Signal nelle opzioni di esecuzione.](../assets/external-signal-name.png)

     +++

1. Per attivare il workflow, eseguire la funzione JavaScript `PostEvent`. Questa funzione ti consente di trasmettere le variabili con i valori desiderati e di utilizzarle nel flusso di lavoro attivato.

   La funzione `PostEvent` può essere eseguita da un altro flusso di lavoro o da una chiamata API.

   * Per attivare un&#39;attività **[!UICONTROL External signal]** da un flusso di lavoro, eseguire la funzione PostEvent dal riquadro **[!UICONTROL Script di inizializzazione]**, accessibile dalle **[!UICONTROL opzioni di esecuzione]** dell&#39;attività. Per l&#39;attività **[!UICONTROL Codice JavaScript]**, eseguire la funzione dallo script dell&#39;attività.

     La sintassi è la seguente:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Visualizza esempio

   In questo esempio, viene attivata l&#39;attività &quot;signal1&quot; External signal. È stato aggiunto al flusso di lavoro con il nome interno &quot;WKF12345&quot;. Una variabile denominata &quot;customID&quot; viene passata con il valore &quot;123456&quot;.

   ![La schermata mostra un esempio di attivazione dell&#39;attività External Signal tramite la funzione PostEvent.](../assets/external-signal-sample.png)

   +++

   * Per attivare un&#39;attività **[!UICONTROL External signal]** da una chiamata API, segui i passaggi descritti nella documentazione API di Campaign. [Scopri come utilizzare il metodo `PostEvent` statico](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=it).