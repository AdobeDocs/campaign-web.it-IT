---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Crea pubblico
description: Scopri come utilizzare l’attività del flusso di lavoro Crea pubblico
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 10%

---


# Creazione del pubblico {#build-audience}

Il **Creare un pubblico** l&#39;attività è un **Targeting** attività. Questa attività ti consente di definire il pubblico che entrerà nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico del messaggio non è definito nell’attività del canale, ma nel **Creare un pubblico** attività.

Per definire la popolazione del pubblico, puoi:

* Seleziona un pubblico esistente, creato come elenco nella console client.
* Seleziona un pubblico di Adobe Experience Platform.
* Crea un nuovo pubblico con il generatore di regole definendo e combinando criteri di filtro.

>[!NOTE]
>
>In questo contesto, non è possibile caricare un pubblico da un file. A questo scopo, devi creare una consegna autonoma. [Ulteriori informazioni](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurazione

Per configurare il **Creare un pubblico** attività:

1. Aggiungi un **Creare un pubblico** attività.
1. Definisci un’etichetta.
1. Definisci il tipo di pubblico: **Crea il tuo** o **Read audience**.

Per creare una query personalizzata, segui questi passaggi aggiuntivi:

1. Seleziona **Crea il tuo (query)**.
1. Scegli la **Dimensione targeting**. La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. Consulta la sezione [Documentazione di v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Clic **Continua**.
1. Utilizza il generatore di regole per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. Fai riferimento a questa [sezione](../../audience/segment-builder.md).

Per selezionare un pubblico esistente, effettua le seguenti operazioni:

1. Seleziona **Read audience**.
1. Clic **Continua**.
1. Seleziona il pubblico nello stesso modo in cui utilizzi un pubblico durante la progettazione di una nuova e-mail. Fai riferimento a questa [sezione](../../audience/add-audience.md).

## Esempio

Esempio di flusso di lavoro con due **Creare un pubblico** attività. Il primo si rivolge al pubblico dei giocatori di poker, seguito da una consegna e-mail. Il secondo prende di mira il pubblico dei clienti VIP, seguito da una consegna SMS.

![](../assets/workflow-audience-example.png)