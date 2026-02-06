---
audience: end-user
title: Utilizzare un’attività del flusso di lavoro di consegna continua
description: Scopri come utilizzare l’attività del flusso di lavoro Consegna continua
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 3%

---

# Consegna continua {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Attività di consegna continua"
>abstract="Ora puoi aggiungere nuovi destinatari a una consegna esistente. Questo tipo di consegna evita di dover creare ogni volta una nuova consegna, rendendola più efficiente per gli avvisi o le notifiche a basso volume inviate in base alle esigenze."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"

L&#39;attività **Consegna continua** ti consente di aggiungere nuovi destinatari a una consegna esistente. Questo tipo di consegna evita di dover creare ogni volta una nuova consegna, rendendola più efficiente per gli avvisi o le notifiche a basso volume inviate in base alle esigenze.

Una consegna continua crea una singola istanza di consegna. Tutti i registri di consegna (broadLog) e di tracciamento fanno riferimento a questa consegna, semplificandone il monitoraggio e il reporting.

## Configurare l’attività Consegna continua {#configure}

1. Aggiungi un&#39;attività **Consegna continua** all&#39;area di lavoro del flusso di lavoro.

   ![Schermata che mostra l&#39;attività Consegna continua](../assets/continuous-delivery.png){zoomable="yes"}

1. Immettere un&#39;etichetta **[!UICONTROL Label]** personalizzata per l&#39;attività (facoltativo). Per impostazione predefinita, è etichettato come &quot;Consegna continua&quot;.

1. Accanto al campo **[!UICONTROL Modello]**, fai clic sull&#39;icona di ricerca per selezionare un modello di consegna. Solo i modelli (non le consegne standard) sono disponibili per la selezione. Il modello definisce il canale di consegna, il contenuto e la configurazione.

1. Nelle **[!UICONTROL opzioni di targeting]**, scegli come viene definita la popolazione target:

   * **[!UICONTROL Specificato dagli eventi in entrata]**: la destinazione proviene dalla transizione in entrata (da attività a monte come Genera pubblico o Query incrementale). Questa è l’opzione più comune.

   * **[!UICONTROL Specificato nel modello di consegna]**: la destinazione è definita nel modello stesso.

   * **[!UICONTROL File specificato nell&#39;evento di input]**: la destinazione viene fornita tramite un file passato tramite il flusso di lavoro.

L’attività di consegna continua genera automaticamente una transizione in uscita per continuare il flusso di lavoro.

## Argomenti correlati {#related}

* [Informazioni sulle attività dei flussi di lavoro](about-activities.md)
* [Attività di e-mail, SMS, push e direct mail](channels.md)
* [Modelli di consegna](../../msg/delivery-template.md)
