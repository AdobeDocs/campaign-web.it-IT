---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Fork
description: Scopri come utilizzare l’attività del flusso di lavoro Fork
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# Attività Fork {#fork}

Il **Fork** l&#39;attività è un **Controllo del flusso** attività. Consente di creare transizioni in uscita per avviare più attività in contemporanea.

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

