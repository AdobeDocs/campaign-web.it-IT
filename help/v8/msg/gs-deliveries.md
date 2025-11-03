---
product: campaign
title: Accedere alle consegne
description: Scopri come accedere e gestire le consegne in Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 36%

---

# Accedere alle consegne {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Consegne"
>abstract="Una consegna è una comunicazione inviata a un pubblico su un canale specifico: e-mail, SMS o Push. In questa schermata puoi modificare, duplicare ed eliminare le consegne esistenti. Puoi visualizzare anche i rapporti delle consegne completate. Fai clic sul pulsante **Crea consegna** per aggiungere una nuova consegna."

## Accedere alle consegne {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Destinazione aggiuntiva"
>abstract="Questi regole possono essere modificate solo nella console client."

Le consegne sono accessibili dal menu **[!UICONTROL Consegne]** nella navigazione a sinistra. In questo elenco vengono visualizzate tutte le consegne create dalla console client o dall’interfaccia utente Web. Da questa schermata, puoi monitorare tutte le consegne esistenti, duplicarle, eliminarle o crearne di nuove.

![Elenco delle consegne visualizzate nell&#39;interfaccia](assets/deliveries-list.png)

Per aprire una consegna, fai clic sul nome nell’elenco. La consegna si apre e consente di eseguire varie azioni, come modificare i parametri, controllarne l’esecuzione o monitorarne le prestazioni utilizzando rapporti dedicati.

![Schermata dei dettagli della consegna con parametri e report](assets/delivery-details.png)

Se apri una consegna creata nella console client, è possibile che vengano visualizzate due nuove sezioni per il pubblico. Questi parametri possono essere modificati solo nella console.

* **[!UICONTROL Destinazione aggiuntiva]**: indica che sono state configurate più destinazioni per questa consegna.

* **[!UICONTROL Destinazione bozza aggiuntiva]**: indica che è stata definita una condizione dinamica per le destinazioni bozza in questa consegna.

![Messaggio di avviso sulla configurazione di destinazione aggiuntiva](assets/target-warning-audience.png){zoomable="yes"}

## Duplicare una consegna {#delivery-duplicate}

Puoi creare una copia di una consegna esistente dall’elenco o dal dashboard delle consegne.

Per duplicare una consegna dall’elenco delle consegne, effettua le seguenti operazioni:

1. Fai clic sul pulsante con i tre puntini a destra, accanto al nome della consegna da duplicare.
1. Seleziona **[!UICONTROL Duplica]**.
1. Conferma la duplicazione. La nuova dashboard di consegna si apre nella schermata centrale.

Per duplicare una consegna dal dashboard, effettua le seguenti operazioni:

1. Apri la consegna e fai clic sul pulsante **[!UICONTROL ...More]** nella sezione superiore della schermata.
1. Seleziona **[!UICONTROL Duplica]**.
1. Conferma la duplicazione. La nuova consegna sostituisce la consegna corrente nella schermata centrale.

## Eliminare una consegna {#delivery-delete}

Le consegne vengono eliminate dall’elenco di consegna, dalla voce di consegna principale nella barra a sinistra o dall’elenco di consegna di una campagna.

Per eliminare una consegna dall’elenco delle consegne, segui questi passaggi:

1. Fai clic sul pulsante tre punti a destra, accanto al nome della consegna da eliminare.
1. Selezionare **[!UICONTROL Elimina]**.
1. Conferma l’eliminazione.

![Eliminazione di una consegna dall&#39;interfaccia dell&#39;elenco di consegna](assets/delete-delivery-from-list.png)

In questi elenchi sono presenti tutte le consegne, tuttavia le consegne create in un flusso di lavoro non possono essere eliminate da un elenco di consegne. Per eliminare una consegna creata nel contesto di un flusso di lavoro, elimina l’attività di consegna dal flusso di lavoro.

Per eliminare una consegna da un flusso di lavoro, segui questi passaggi:

1. Seleziona l’attività di consegna.
1. Fai clic sull&#39;icona **[!UICONTROL Elimina]** nel pannello di destra.
1. Conferma l’eliminazione. Se la consegna ha nodi secondari, scegli di eliminarli anche loro o di mantenerli.

![Eliminazione di un&#39;attività di consegna in un flusso di lavoro](assets/delete-delivery-from-wf.png)