---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Creazione del pubblico
description: Scopri come utilizzare l’attività del flusso di lavoro Creazione del pubblico
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '312'
ht-degree: 100%

---


# Creazione del pubblico {#build-audience}

L’attività **Creazione del pubblico** è un’attività di **targeting**. Questa attività ti consente di definire il pubblico che sarà inserito nel flusso di lavoro. Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico del messaggio non è definito nell’attività del canale, ma nell’attività **Creazione del pubblico**.

Per definire la popolazione di pubblico, puoi:

* Selezionare un pubblico esistente, creato come elenco nella console client.
* Selezionare un pubblico di Adobe Experience Platform.
* Creare un nuovo pubblico con il generatore di regole definendo e combinando criteri di filtro.

>[!NOTE]
>
>In questo contesto, non è possibile caricare un pubblico da un file. A questo scopo, devi creare una consegna autonoma. [Ulteriori informazioni](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurazione

Per configurare l’attività **Creazione del pubblico**, segui questi passaggi:

1. Aggiungi un’attività **Creazione del pubblico**.
1. Definisci un’etichetta.
1. Definisci il tipo di pubblico: **Crea nuovo** o **Leggi pubblico**.

Per creare una query personalizzata, segui questi passaggi aggiuntivi:

1. Seleziona **Crea nuovo (query)**.
1. Scegli la **dimensione targeting**. La dimensione targeting consente di definire la popolazione target dell’operazione: destinatari, beneficiari del contratto, operatore, abbonati, ecc. Per impostazione predefinita, il target viene selezionato dai destinatari. Consulta la [documentazione di v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=it#targeting-and-filtering-dimensions){target="_blank"}.
1. Fai clic su **Continua**.
1. Utilizza il generatore di regole per definire la query, nello stesso modo in cui crei un pubblico durante la progettazione di una nuova e-mail. Consulta questa [sezione](../../audience/segment-builder.md).

Per selezionare un pubblico esistente, segui questi passaggi:

1. Seleziona **Leggi pubblico**.
1. Fai clic su **Continua**.
1. Seleziona il pubblico nello stesso modo in cui utilizzi un pubblico durante la progettazione di una nuova e-mail. Consulta questa [sezione](../../audience/add-audience.md).

## Esempio

Di seguito è riportato un esempio di un flusso di lavoro con due attività di **Creazione del pubblico**. Il primo esegue il targeting di un pubblico di giocatori di poker, seguito da una consegna e-mail. Il secondo quello di un pubblico di clienti VIP, seguito da una consegna SMS.

![](../assets/workflow-audience-example.png)