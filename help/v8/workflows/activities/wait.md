---
audience: end-user
title: Utilizzare l’attività Attendi nei flussi di lavoro
description: Scopri come utilizzare l’attività Attendi nei flusso di lavoro
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: ht
source-wordcount: '162'
ht-degree: 100%

---


# Attendi {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Attività attendi"
>abstract="L’attività **Attendi** viene utilizzata per ritardare la transizione da un’attività a un’altra."

L’attività **Attendi** è un’attività di **Controllo del flusso**. Questa attività viene utilizzata per lasciare che trascorra un certo periodo di tempo tra due attività in corso. Ad esempio, per attendere diversi giorni dopo un’attività di consegna e-mail, quindi analizzare le aperture e i clic generati durante questo periodo prima di eseguire eventuali operazioni di follow-up (e-mail di promemoria, creazione di un pubblico, ecc.).

## Configurazione{#wait-configuration}

Per configurare l’attività **Attendi**, segui questi passaggi:

1. Aggiungi un’attività **Attendi** nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra le transizioni in entrata e in uscita.

1. Seleziona l’unità di tempo nel campo **Periodi**: secondi, minuti, ore.

## Esempio{#wait-example}

L’esempio seguente illustra l’attività **Attendi** in un caso d’uso tipico. Viene inviata un’e-mail di invito a un evento. 24 ore dopo l’invio, viene inviata una consegna SMS alla stessa popolazione.

![](../assets/workflow-wait-example.png)
