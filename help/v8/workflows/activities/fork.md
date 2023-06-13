---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Fork
description: Scopri come utilizzare l’attività del flusso di lavoro Fork
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 18%

---


# Attività Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Attività Fork"
>abstract="L’attività Fork ti consente di creare transizioni in uscita per avviare più attività contemporaneamente."

## Configurazione

Per configurare il **Fork** attività:

1. Aggiungi un **Fork** al flusso di lavoro.
1. Clic **Aggiungi transizione** per aggiungere una nuova transizione in uscita. Per impostazione predefinita sono definite due transizioni.
1. Aggiungi un’etichetta a ciascuna delle transizioni.

## Esempio

Nell’esempio seguente vengono utilizzati due **Fork** attività:

* Una prima delle due query, per eseguirle contemporaneamente.
* Uno dopo l’intersezione, per inviare contemporaneamente un’e-mail e un SMS alla popolazione target.

![](../assets/workflow-fork-example.png)

