---
audience: end-user
title: Utilizzare l’attività Fork nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 71%

---


# Fork {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Attività Fork"
>abstract="Il **Fork** l&#39;attività è un **Controllo del flusso** attività. Consente di creare transizioni in uscita per avviare più attività in contemporanea."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Attività Fork"
>abstract="L’attività Fork consente di creare transizioni in uscita per avviare più attività contemporaneamente."

Il **Fork** l&#39;attività è un **Controllo del flusso** attività. Consente di creare transizioni in uscita per avviare più attività in contemporanea.

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

