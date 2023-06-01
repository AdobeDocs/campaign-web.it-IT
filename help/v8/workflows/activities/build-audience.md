---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Crea pubblico
description: Scopri come utilizzare l’attività del flusso di lavoro Crea pubblico
badge: label="Alpha" type="Positive"
source-git-commit: 9b639a533e75822570d6cc2b9752fc9380d069dd
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 14%

---


# Creazione del pubblico {#build-audience}

Questa attività ti consente di definire un pubblico. Puoi selezionare un pubblico esistente o utilizzare il generatore di regole per definire una query personalizzata.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurazione

Per configurare il **Creare un pubblico** attività:

1. Aggiungi un’attività di generazione del pubblico.
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

Ecco un esempio di flusso di lavoro con due **Creare un pubblico** attività. Il primo si rivolge al pubblico dei giocatori di poker, seguito da una consegna e-mail. Il secondo prende di mira il pubblico dei clienti VIP, seguito da una consegna SMS.

![](../assets/workflow-audience-example.png)