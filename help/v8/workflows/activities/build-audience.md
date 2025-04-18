---
audience: end-user
title: Utilizzare l’attività Crea pubblico nei flussi di lavoro
description: Scopri come utilizzare l’attività Crea pubblico nei flussi di lavoro
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 62%

---

# Creazione del pubblico {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Attività Crea pubblico"
>abstract="L’attività **Creazione del pubblico** consente di definire il pubblico che sarà inserito nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro, il pubblico del messaggio non è definito nell’attività del canale, ma nell’attività **Creazione del pubblico**."

L’attività **Crea pubblico** è un’attività di **targeting**. Questa attività consente di definire il pubblico che sarà inserito nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro, il pubblico del messaggio non è definito nell’attività del canale, ma nell’attività **Creazione del pubblico**.

Per definire la popolazione del pubblico, puoi eseguire le seguenti operazioni:

* Seleziona un pubblico esistente, creato come elenco nella console client.
* Seleziona un pubblico di Adobe Experience Platform.
* Crea un nuovo pubblico con Query Modeler definendo e combinando criteri di filtro.

>[!NOTE]
>
>I tipi di pubblico caricati da un file non possono essere targetizzati utilizzando un’attività Genera pubblico. A tale scopo, è necessario utilizzare un&#39;attività **Load file** seguita da un&#39;attività **Reconciliation**. [Ulteriori informazioni](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurare l’attività Creazione del pubblico {#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_audienceselector"
>title="Pubblico"
>abstract="Seleziona il pubblico nello stesso modo in cui utilizzi un pubblico durante la progettazione di una nuova consegna."

Per configurare l’attività **Crea pubblico**, segui questi passaggi:

![Schermata che mostra l&#39;interfaccia di configurazione del pubblico del flusso di lavoro.](../assets/workflow-audience.png)

1. Aggiungi un’attività **Crea pubblico**.
1. Definisci un’etichetta.
1. Definisci il tipo di pubblico: **Crea una query personalizzata** o **Leggi pubblico**.
1. Configura il pubblico seguendo i passaggi descritti nelle schede seguenti.

>[!BEGINTABS]

>[!TAB Crea il tuo (query)]

Per creare una query personalizzata, effettua le seguenti operazioni:

1. Seleziona **Crea una query personalizzata**.
1. Scegli la **Dimensione targeting**. La dimensione di targeting consente di definire la popolazione target dell’operazione, ad esempio destinatari, beneficiari del contratto, operatori o abbonati. Per impostazione predefinita, il target viene selezionato dai destinatari. [Ulteriori informazioni sulle dimensioni di targeting](../../audience/about-recipients.md#targeting-dimensions)
1. Fai clic su **Continua**.
1. Utilizza il modellatore di query per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. [Scopri come utilizzare Query Modeler](../../query/query-modeler-overview.md)

>[!TAB Read audience]

Per selezionare un pubblico esistente, segui questi passaggi:

1. Seleziona **Leggi pubblico**.
1. Fai clic su **Continua**.
1. Seleziona il pubblico nello stesso modo in cui utilizzi un pubblico durante la progettazione di una nuova consegna. Consulta questa [sezione](../../audience/add-audience.md).

>[!ENDTABS]

## Esempi {#build-audience-examples}

Di seguito è riportato un esempio di un flusso di lavoro con due attività **Crea pubblico**. Il primo esegue il targeting di un pubblico di giocatori di poker, seguito da una consegna e-mail. Il secondo quello di un pubblico di clienti VIP, seguito da una consegna SMS.

![Schermata che mostra un flusso di lavoro di esempio con due attività Genera pubblico indirizzate a tipi di pubblico diversi.](../assets/workflow-audience-example.png)