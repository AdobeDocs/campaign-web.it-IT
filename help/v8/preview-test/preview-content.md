---
audience: end-user
title: Anteprima del contenuto della consegna
description: Scopri come visualizzare in anteprima i contenuti della consegna con l’interfaccia utente web di Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 8667de1d86428427edd9a2718218de9801b0922d
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 54%

---


# Visualizzare in anteprima il contenuto del messaggio {#preview-content}

Utilizza la funzionalità di simulazione dei contenuti di [!DNL Campaign] per visualizzare in anteprima il contenuto del messaggio prima di inviarlo. Questa consente di controllare la personalizzazione e di verificare come verrà presentata ai destinatari.

Per visualizzare l’anteprima del contenuto della consegna, segui i passaggi indicati di seguito.

1. Passa alla schermata di modifica del contenuto della consegna o alla [E-mail Designer](../email/get-started-email-designer.md).

1. Fai clic sul pulsante **[!UICONTROL Simula contenuto]**.

   ![](assets/simulate-button.png){zoomable=&quot;yes&quot;}

1. Seleziona i profili da utilizzare per visualizzare in anteprima il contenuto. A questo scopo, fai clic su **[!UICONTROL Aggiungi profili di test]** (per e-mail e SMS) o **[!UICONTROL Aggiungi sottoscrittori]** (per le notifiche push).

1. Puoi combinare profili e profili di test per visualizzare in anteprima il messaggio e-mail o SMS.

   * Il **[!UICONTROL Profili di test]** La scheda elenca tutti i profili di test, che sono destinatari aggiuntivi e fittizi nel database. [Scopri come utilizzare i profili di test](../audience/test-profiles.md)

   * Il **[!UICONTROL Profili]** Questa scheda elenca tutti i profili memorizzati nel database. [Scopri come utilizzare i profili](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable=&quot;yes&quot;}

1. Quando esplori il profilo di test o gli elenchi di profili, puoi utilizzare i filtri per perfezionare la ricerca. Ad esempio, puoi definire una regola per trovare tutti i profili di test con **[!UICONTROL Potenziale cliente]** stato. [Scopri come aggiungere regole utilizzando Query Modeler](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Fai clic su **[!UICONTROL Seleziona]** per confermare la selezione.

   Viene visualizzata un’anteprima del contenuto della consegna nel riquadro a destra della schermata **[!UICONTROL Simula]**. Gli elementi personalizzati vengono sostituiti dai dati del profilo selezionato nel riquadro a sinistra.

   ![](assets/simulate-preview.png){zoomable=&quot;yes&quot;}

1. Se hai aggiunto più profili, puoi passare da un profilo all’altro nell’elenco per visualizzare in anteprima il contenuto della consegna corrispondente. Puoi anche aggiungere altri profili di test e cancellare la selezione utilizzando i pulsanti corrispondenti nel riquadro a sinistra.

1. Per le consegne e-mail, puoi regolare il **[!UICONTROL Livello zoom]** e visualizzare l’anteprima dei contenuti su un computer desktop o un dispositivo mobile utilizzando l’icona dedicata nell’angolo in alto a destra.

1. Dalla schermata **[!UICONTROL Simula]** puoi anche eseguire le seguenti operazioni:
   * Inviare consegne di test a destinatari specifici per la convalida - [Ulteriori informazioni](test-deliveries.md)
   * Accedere ai registri delle consegne di test inviate - [Ulteriori informazioni](test-deliveries.md#access-test-deliveries)
   * Solo per le e-mail: controllare il rendering del contenuto dei messaggi nei client e-mail più diffusi - [Ulteriori informazioni](email-rendering.md)



