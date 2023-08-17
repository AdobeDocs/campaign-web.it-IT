---
audience: end-user
title: Utilizzare l’attività Attendi nei flussi di lavoro
description: Scopri come utilizzare l’attività Attendi nei flusso di lavoro
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 100%

---


# Attendi {#wait}

L’attività **Attendi** è un’attività di **Controllo del flusso**. Questa attività viene utilizzata per lasciare che trascorra un certo periodo di tempo tra due attività in corso. Ad esempio, per attendere diversi giorni dopo un’attività di consegna e-mail, quindi analizzare le aperture e i clic generati durante questo periodo prima di eseguire eventuali operazioni di follow-up (e-mail di promemoria, creazione di un pubblico, ecc.).

## Configurazione

Per configurare l’attività **Attendi**, segui questi passaggi:

1. Aggiungi un’attività **Attendi** nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra le transizioni in entrata e in uscita.

1. Seleziona l’unità di tempo nel campo **Periodi**: secondi, minuti, ore.

## Esempio

L’esempio seguente illustra l’attività **Attendi** in un caso d’uso tipico. Viene inviata un’e-mail di invito a un evento. 24 ore dopo l’invio, viene inviata una consegna SMS alla stessa popolazione.

![](../assets/workflow-wait-example.png)
