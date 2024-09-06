---
audience: end-user
title: Utilizzare l’attività Unione AND nei flussi di lavoro
description: Scopri come utilizzare l’attività Unione AND nei flussi di lavoro
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 100%

---

# AND-join {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Attività AND-join"
>abstract="L’attività **And-join** consente di sincronizzare più rami di esecuzione di un flusso di lavoro. Viene attivata al termine di tutte le attività precedenti. Questo ti consente di verificare che alcune attività siano state completate prima di continuare a eseguire il flusso di lavoro."

L’attività **Unione AND** è un’attività di **Controllo del flusso**. Consente di sincronizzare più rami di esecuzione di un flusso di lavoro.

Questa attività attiva la relativa transizione in uscita solo dopo che tutte le transizioni in entrata sono state attivate, in altre parole, dopo che tutte le attività precedenti sono state completate. Questo consente di verificare che alcune attività siano state completate prima di continuare a eseguire il flusso di lavoro.

## Configurare l’attività And-join{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Opzioni di unione"
>abstract="Seleziona le attività che vuoi unire. Nel menu a discesa **Set primario**, scegli la popolazione di transizione in entrata da mantenere."

Per configurare l’attività **Unione AND**, segui questi passaggi:

![](../assets/workflow-andjoin.png)

1. Aggiungi più attività, come le attività del canale, per creare almeno due rami di esecuzione diversi.
1. Aggiungi un’attività **Unione AND** a uno dei rami.
1. Nella sezione **Opzioni di unione**, seleziona tutte le attività precedenti che desideri unire.
1. Nel menu a discesa **Set primario**, scegli la popolazione di transizione in entrata da mantenere. La transizione in uscita può contenere solo una delle popolazioni di transizione in entrata.

## Esempio{#and-join-example}

L’esempio seguente mostra due rami del flusso di lavoro con consegna e-mail e SMS. L’Unione AND verrà attivata quando sono abilitate entrambe le transizioni in entrata. Le notifiche push verranno quindi inviate solo al termine di entrambe le consegne.

![](../assets/workflow-andjoin-example.png){zoomable="yes"}
