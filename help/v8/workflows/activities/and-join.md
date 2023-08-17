---
audience: end-user
title: Utilizzare l’attività Unione AND nei flussi di lavoro
description: Scopri come utilizzare l’attività Unione AND nei flussi di lavoro
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 100%

---


# Unione AND {#join}

L’attività **Unione AND** è un’attività di **Controllo del flusso**. Consente di sincronizzare più rami di esecuzione di un flusso di lavoro.

Questa attività attiva la relativa transizione in uscita solo dopo che tutte le transizioni in entrata sono state attivate, in altre parole, dopo che tutte le attività precedenti sono state completate. Questo consente di verificare che alcune attività siano state completate prima di continuare a eseguire il flusso di lavoro.

## Configurazione

Per configurare l’attività **Unione AND**, segui questi passaggi:

1. Aggiungi più attività, come le attività del canale, per creare almeno due rami di esecuzione diversi.
1. Aggiungi un’attività **Unione AND** a uno dei rami.
1. Nella sezione **Opzioni di unione**, seleziona tutte le attività precedenti che desideri unire.
1. Nel menu a discesa **Set primario**, scegli la popolazione di transizione in entrata da mantenere. La transizione in uscita può contenere solo una delle popolazioni di transizione in entrata.

## Esempio

L’esempio seguente mostra due rami del flusso di lavoro con consegna e-mail e SMS. L’Unione AND verrà attivata quando sono abilitate entrambe le transizioni in entrata. Le notifiche push verranno quindi inviate solo al termine di entrambe le consegne.

![](../assets/workflow-andjoin-example.png)