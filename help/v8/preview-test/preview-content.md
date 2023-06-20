---
audience: end-user
title: Anteprima del contenuto della consegna
description: Scopri come visualizzare in anteprima i contenuti della consegna con l’interfaccia web di Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha"
source-git-commit: a653fe4329f449a94f8056e4b5f2247bd839b87a
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 40%

---


# Anteprima del contenuto della consegna {#preview-content}

Utilizza il [!DNL Campaign] funzionalità di simulazione dei contenuti per visualizzare in anteprima il contenuto del messaggio prima di inviarlo. Questo ti consente di controllare la personalizzazione e di verificarne la modalità di visualizzazione ai destinatari.

Per visualizzare in anteprima il contenuto della consegna, segui i passaggi indicati di seguito.

1. Passa alla schermata per la modifica del contenuto della consegna.

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. Fai clic sul pulsante **[!UICONTROL Simula contenuto]**.

   ![](assets/simulate-button.png)

1. Per selezionare i profili da utilizzare per l’anteprima dei contenuti personalizzati, utilizza:

   * **[!UICONTROL Aggiungi profili di test]** per visualizzare in anteprima le consegne e-mail e SMS

   * **[!UICONTROL Aggiungi sottoscrittori]** per visualizzare in anteprima le notifiche push

1. Puoi combinare profili di test e profili per visualizzare in anteprima il messaggio e-mail o SMS.

   * La scheda **[!UICONTROL Profili di test]** contiene tutti gli indirizzi seed, che sono destinatari aggiuntivi e fittizi nel database.

     >[!NOTE]
     >
     >I profili di test possono essere creati nella console [!DNL Campaign] nella cartella **[!UICONTROL Risorse]** > **[!UICONTROL Gestione delle campagne]** > **[!UICONTROL Indirizzi seed]**. Ulteriori informazioni sono disponibili nella [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=it){target="_blank"}.

   * La scheda **[!UICONTROL Profili]** elenca tutti i destinatari memorizzati nella cartella **[!UICONTROL Profili e destinazioni]** dalla console di [!DNL Campaign] Ulteriori informazioni sono disponibili nella [documentazione Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html?lang=it){target="_blank"}.

   ![](assets/simulate-select-profiles.png)

1. Clic **[!UICONTROL Seleziona]** per confermare la selezione.

   Nel riquadro a destra della sezione viene visualizzata un’anteprima del contenuto della consegna **[!UICONTROL Simula]** schermo. Gli elementi personalizzati vengono sostituiti dai dati del profilo selezionato nel riquadro a sinistra.

   ![](assets/simulate-preview.png)

1. Se hai aggiunto più profili, puoi passare da uno all’altro nell’elenco per visualizzare in anteprima il contenuto di consegna corrispondente. Puoi anche aggiungere altri profili di test e cancellare la selezione utilizzando i pulsanti corrispondenti nel riquadro a sinistra.

1. Per le consegne e-mail, puoi regolare il **[!UICONTROL Livello di zoom]** e visualizzare l’anteprima dei contenuti su un desktop o un dispositivo mobile utilizzando l’icona dedicata nell’angolo in alto a destra.

1. Dalla schermata **[!UICONTROL Simula]** puoi anche:
   * Inviare consegne di test a destinatari specifici per la convalida - [Ulteriori informazioni](proofs.md)
   * Accedere ai registri delle consegne di test inviate - [Ulteriori informazioni](proofs.md#access-proofs)
   * Solo per la posta elettronica, controlla il rendering del contenuto dei messaggi nei client e-mail più diffusi - [Ulteriori informazioni](email-rendering.md)



