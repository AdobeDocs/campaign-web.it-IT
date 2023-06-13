---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Attendi
description: Scopri come utilizzare l’attività del flusso di lavoro Attendi
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 29%

---


# Attività Wait {#wait}

Il **Wait** l&#39;attività è un **Controllo del flusso** attività. Viene utilizzato per consentire il trascorrere di un certo periodo di tempo tra due attività eseguite. Ad esempio, per attendere diversi giorni dopo un’attività di consegna e-mail, quindi per analizzare le aperture e i clic generati durante questo periodo prima di eseguire eventuali operazioni di follow-up (promemoria e-mail, creazione di un pubblico, ecc.).

## Configurazione

Per configurare il **Wait** attività:

1. Aggiungi un **Wait** attività nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra le transizioni in entrata e in uscita.

1. Selezionare l&#39;unità di tempo in **Periodi** campo: secondi, minuti, ore.

## Esempio

L&#39;esempio seguente illustra **Wait** attività in un caso d’uso tipico. Viene inviato un invito e-mail a un evento. 24 ore dopo l’invio, viene inviata una consegna SMS alla stessa popolazione.

![](../assets/workflow-wait-example.png)
