---
audience: end-user
title: Utilizzare l’attività Fork nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
TQID: https://experienceleague.adobe.com/a6KZ9gWNyGRY2D5vYKVJ-MP6WB4H-weR5RZTMbD71vA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 53%

---

# Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Attività Fork"
>abstract="L’attività **Fork** consente di creare transizioni in uscita per avviare più attività contemporaneamente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transizioni delle attività Fork"
>abstract="Per impostazione predefinita, vengono create due transizioni con attività **Fork**. Fai clic sul pulsante **Aggiungi transizione** per definire una transizione in uscita aggiuntiva e immetterne l’etichetta."

L’attività **Fork** è un’attività di **Controllo del flusso**. Consente di creare transizioni in uscita per avviare più attività contemporaneamente.

Puoi anche creare un ramo separato utilizzando il pulsante **Aggiungi ramo** (**+**) della barra degli strumenti. Consulta [Orchestrare le attività](../orchestrate-activities.md#toolbar).

## Configurare l’attività Fork {#fork-configuration}

Per configurare l’attività **Fork** segui questi passaggi:

![Schermata di configurazione dell&#39;attività del fork del flusso di lavoro](../assets/workflow-fork.png)

1. Aggiungi un’attività **Fork** al flusso di lavoro.
1. Fai clic su **Aggiungi transizione** per aggiungere una nuova transizione in uscita. Per impostazione predefinita, sono definite due transizioni.
1. Aggiungi un’etichetta a ciascuna transizione.

## Esempio {#fork-example}

Nell&#39;esempio seguente vengono utilizzate due attività **Fork**:

* Una prima delle due query, per eseguirle simultaneamente.
* Uno dopo l’intersezione, per inviare contemporaneamente un’e-mail e un SMS alla popolazione target.

![Schermata di esempio del fork del flusso di lavoro](../assets/workflow-fork-example.png)
