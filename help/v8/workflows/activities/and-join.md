---
audience: end-user
title: Utilizzare l’attività Unione AND nei flussi di lavoro
description: Scopri come utilizzare l’attività Unione AND nei flussi di lavoro
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 50%

---

# AND-join {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Attività AND-join"
>abstract="L’attività **And-join** consente di sincronizzare più rami di esecuzione di un flusso di lavoro. Viene attivata al termine di tutte le attività precedenti. Questo garantisce che determinate attività vengano completate prima di continuare a eseguire il flusso di lavoro."

L’attività **Unione AND** è un’attività di **Controllo del flusso**. Sincronizza più rami di esecuzione di un flusso di lavoro.

Questa attività attiva la relativa transizione in uscita solo dopo l’attivazione di tutte le transizioni in entrata. In altre parole, si attiva una volta completate tutte le attività precedenti. In questo modo, determinate attività vengono completate prima di continuare a eseguire il flusso di lavoro.

## Configurare l’attività And-join {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Opzioni di unione"
>abstract="Seleziona le attività che vuoi unire. Nel menu a discesa **Set primario**, scegli la popolazione di transizione in entrata da mantenere."

Per configurare l’attività **Unione AND**, segui questi passaggi:

![Schermata che mostra l&#39;interfaccia di configurazione per l&#39;attività AND-join.](../assets/workflow-andjoin.png)

1. Aggiungi più attività, ad esempio attività canale, per formare almeno due rami di esecuzione diversi.
1. Aggiungi un’attività **Unione AND** a uno dei rami.
1. Nella sezione **Opzioni di unione**, seleziona tutte le attività precedenti a cui desideri partecipare.
1. Nell&#39;elenco a discesa **Set primario**, scegliere il gruppo di transizione in entrata da mantenere. La transizione in uscita può contenere solo una delle popolazioni di transizione in entrata.

## Esempio {#and-join-example}

L’esempio seguente mostra due rami del flusso di lavoro con consegna e-mail e SMS. L’unione AND viene attivata quando sono abilitate entrambe le transizioni in entrata. Le notifiche push vengono inviate solo dopo il completamento di entrambe le consegne.

![Esempio di flusso di lavoro con due rami che mostra la consegna di e-mail e SMS seguita da notifiche push.](../assets/workflow-andjoin-example.png){zoomable="yes"}