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

Il **Segnale esterno** l&#39;attività è un **Controllo del flusso** attività. Consente di attivare l’esecuzione di un flusso di lavoro da un altro flusso di lavoro o da una chiamata API.

>[!NOTE]
>
>Questa pagina illustra i passaggi principali per configurare una **[!UICONTROL Segnale esterno]** nell’interfaccia utente di Campaign Web e attivarla da un altro flusso di lavoro o da una chiamata API. Informazioni dettagliate su come attivare un flusso di lavoro e le relative best practice, e come lavorare con le API di Campaign sono disponibili nella sezione [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Per configurare il **Segnale esterno** attività e attivarne l’esecuzione:

1. Aggiungi un **Segnale esterno** attività nel flusso di lavoro.

1. Completa la configurazione del flusso di lavoro e avviane l’esecuzione. Il **[!UICONTROL Segnale esterno]** L’attività viene visualizzata come &quot;In sospeso&quot;, in attesa di essere attivata.

   ![](../assets/external-signal-pending.png)

1. Recupera le informazioni seguenti:

   * Il **nome interno del workflow**, che viene visualizzato accanto alla relativa etichetta.

     +++Esempio di visualizzazione

     ![](../assets/external-signal-workflow-name.png)

+++

   * Il **Nome dell’attività del segnale esterno**, visualizzato nel file del flusso di lavoro di **[!UICONTROL Opzioni di esecuzione]**.

     +++Esempio di visualizzazione

     ![](../assets/external-signal-name.png)

+++

1. Per attivare il flusso di lavoro, è necessario eseguire `PostEvent` Funzione JavaScript. Questa funzione ti consente di trasmettere le variabili con i valori selezionati e di sfruttarle nel flusso di lavoro attivato.

   Il `PostEvent` La funzione può essere eseguita da un altro flusso di lavoro o da una chiamata API.

   * Per attivare un **[!UICONTROL Segnale esterno]** da un flusso di lavoro, eseguire la funzione PostEvent dalla **[!UICONTROL Script di inizializzazione]** , accessibile dal riquadro dell&#39;attività **[!UICONTROL Opzioni di esecuzione]**. Per **[!UICONTROL Codice JavaScript]** esegua la funzione dallo script dell’attività.

     La sintassi è la seguente:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Esempio di visualizzazione

   In questo esempio viene attivata l’attività &quot;signal1&quot; External signal che è stata aggiunta al flusso di lavoro il cui nome interno è &quot;WKF12345&quot;. Stiamo inoltre trasmettendo una variabile denominata &quot;customID&quot;, con il valore &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Per attivare un **[!UICONTROL Segnale esterno]** da una chiamata API, segui i passaggi descritti nella documentazione API di Campaign. [Scopri come utilizzare il `PostEvent` metodo](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
