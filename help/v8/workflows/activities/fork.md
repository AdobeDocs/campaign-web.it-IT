---
audience: end-user
title: Utilizzare l’attività Fork nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
badge: label="Alfa"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 100%

---


# Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Attività Fork"
>abstract="L’attività Fork consente di creare transizioni in uscita per avviare più attività contemporaneamente."

## Configurazione

Per configurare l’attività **Fork** segui questi passaggi:

1. Aggiungi un’attività **Fork** al flusso di lavoro.
1. Fai clic su **Aggiungi transizione** per aggiungere una nuova transizione in uscita. Per impostazione predefinita sono definite due transizioni.
1. Aggiungi un’etichetta a ciascuna delle transizioni.

## Esempio

Nell’esempio seguente vengono utilizzate due attività **Fork**:

* Una prima delle due query, per eseguirle contemporaneamente.
* Una dopo l’intersezione, per inviare contemporaneamente un’e-mail e un SMS alla popolazione target.

![](../assets/workflow-fork-example.png)

