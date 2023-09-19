---
audience: end-user
title: Utilizzare l’attività Fork nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 66%

---


# Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Attività Fork"
>abstract="L’attività **Fork** consente di creare transizioni in uscita per avviare più attività contemporaneamente."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transizioni delle attività Fork"
>abstract="Per impostazione predefinita, vengono create due transizioni con **Fork** attività. Fai clic su **Aggiungi transizione** per definire una transizione in uscita aggiuntiva e immetterne l’etichetta."

Il **Fork** l&#39;attività è un **Controllo del flusso** attività. Consente di creare transizioni in uscita per avviare più attività in contemporanea.

## Configurare l’attività Fork{#fork-configuration}

Per configurare l’attività **Fork** segui questi passaggi:

![](../assets/workflow-fork.png)

1. Aggiungi un’attività **Fork** al flusso di lavoro.
1. Fai clic su **Aggiungi transizione** per aggiungere una nuova transizione in uscita. Per impostazione predefinita sono definite due transizioni.
1. Aggiungi un’etichetta a ciascuna delle transizioni.

## Esempio{#fork-example}

Nell’esempio seguente vengono utilizzate due attività **Fork**:

* Una prima delle due query, per eseguirle contemporaneamente.
* Una dopo l’intersezione, per inviare contemporaneamente un’e-mail e un SMS alla popolazione target.

![](../assets/workflow-fork-example.png)

