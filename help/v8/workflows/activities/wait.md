---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Attendi
description: Scopri come utilizzare l’attività del flusso di lavoro Attendi
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 42%

---


# Attività Wait {#wait}

Il **Wait** l’attività sospende momentaneamente l’esecuzione di una parte di un flusso di lavoro. Attiva la relativa transizione in uscita dopo un ritardo che può variare da pochi secondi a diversi mesi, che esegue le attività inserite in seguito.

Il **Wait** L’attività viene utilizzata per consentire il trascorrere di un certo periodo di tempo tra due attività eseguite. Ad esempio, per attendere diversi giorni dopo un’attività di consegna e-mail, quindi per analizzare le aperture e i clic generati durante questo periodo prima di eseguire eventuali operazioni di follow-up (promemoria e-mail, creazione di un pubblico, ecc.).

## Configurazione

Per configurare il **Wait** attività:

1. Aggiungi un **Wait** attività nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra l’attivazione delle transizioni in entrata e in uscita dell’attività.

1. Seleziona l’unità di tempo **Periodo**: secondi, minuti, ore.

## Esempio


