---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Attendi
description: Scopri come utilizzare l’attività del flusso di lavoro Attendi
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '147'
ht-degree: 100%

---


# Attendi {#wait}

L’attività **Attendi** è un’attività di **Controllo del flusso**. L’attività viene utilizzata per consentire il trascorrere di un certo periodo di tempo tra due attività in corso. Ad esempio, per attendere diversi giorni dopo un’attività di consegna e-mail, quindi per analizzare le aperture e i clic generati durante questo periodo prima di eseguire eventuali operazioni di follow-up (promemoria e-mail, creazione di un pubblico, ecc.).

## Configurazione

Per configurare l’attività **Attendi**, segui questi passaggi:

1. Aggiungi un’attività **Attendi** nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra le transizioni in entrata e in uscita.

1. Seleziona l&#39;unità di tempo nel campo **Periodi**: secondi, minuti, ore.

## Esempio

L’esempio seguente illustra l’attività **Attendi** in un caso d’uso tipico. Viene inviata un’e-mail di invito a un evento. 24 ore dopo l’invio, viene inviata una consegna SMS alla stessa popolazione.

![](../assets/workflow-wait-example.png)
