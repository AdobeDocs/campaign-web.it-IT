---
audience: end-user
title: Utilizzare l’attività Attendi nei flussi di lavoro
description: Scopri come utilizzare l’attività Attendi nei flusso di lavoro
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 39%

---

# Attendi {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Attività attendi"
>abstract="L&#39;attività **Wait** viene utilizzata per ritardare la transizione da un&#39;attività all&#39;altra."

L’attività **Attendi** è un’attività di **Controllo del flusso**. Consente di trascorrere un certo periodo di tempo tra l’esecuzione di due attività. Ad esempio, può essere utilizzato per attendere diversi giorni dopo un’attività di consegna e-mail, quindi per analizzare le aperture e i clic generati durante questo periodo prima di eseguire operazioni di follow-up, ad esempio l’invio di un promemoria e-mail o la creazione di un pubblico.

## Configurazione {#wait-configuration}

Per configurare l’attività **Attendi**, segui questi passaggi:

1. Aggiungi un’attività **Attendi** nel flusso di lavoro.

1. Specifica la **Durata** dell’attesa tra le transizioni in entrata e in uscita.

1. Selezionare l&#39;unità di tempo nel campo **Periodi**: secondi, minuti, ore o giorni.

## Esempio {#wait-example}

L’esempio seguente illustra l’attività **Attendi** in un caso d’uso tipico. Viene inviata un’e-mail di invito a un evento. Dopo 24 ore, una consegna SMS viene inviata alla stessa popolazione.

![Esempio di flusso di lavoro che utilizza l&#39;attività Attendi per inviare un SMS 24 ore dopo un invito e-mail.](../assets/workflow-wait-example.png)