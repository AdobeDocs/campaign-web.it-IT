---
audience: end-user
title: Utilizzare l’attività Fork nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 58%

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
