---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro AND-join
description: Scopri come utilizzare l’attività del flusso di lavoro AND-join
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 1%

---


# Attività AND-join {#join}

Il **And-join** l&#39;attività è un **Controllo del flusso** attività. Consente di sincronizzare più rami di esecuzione di un flusso di lavoro.

Questa attività attiva solo la relativa transizione in uscita dopo che tutte le transizioni in entrata vengono attivate, in altre parole, dopo che tutte le attività precedenti sono state completate. Questo ti consente di verificare che alcune attività siano state completate prima di continuare a eseguire il flusso di lavoro.

## Configurazione

Per configurare il **Unione AND** attività:

1. Aggiungi più attività, ad esempio attività canale, per formare almeno due rami di esecuzione diversi.
1. Aggiungi un **Unione AND** ad uno qualsiasi dei rami.
1. In **Opzioni di unione** , controlla tutte le attività precedenti a cui desideri partecipare.
1. In **Set primario** , scegli il gruppo di transizione in entrata da mantenere. La transizione in uscita può contenere solo una delle popolazioni di transizione in entrata.

## Esempio

L’esempio seguente mostra due rami del flusso di lavoro con una consegna e-mail e SMS. L’unione AND viene attivata quando sono abilitate entrambe le transizioni in entrata. Le notifiche push verranno quindi inviate solo al termine di entrambe le consegne.

![](../assets/workflow-andjoin-example.png)