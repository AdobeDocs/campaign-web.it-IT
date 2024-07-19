---
title: Introduzione ai profili
description: Scopri come monitorare e gestire i profili in Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 12%

---

# Introduzione ai profili {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profili"
>abstract="Un profilo è un record destinato a ricevere i messaggi inviati da Adobe Campaign. Da questo elenco, in base alle tue autorizzazioni, puoi visualizzare i dettagli dei profili. Utilizza le opzioni di filtro per sfogliare l’elenco. Puoi modificare e aggiornare un piccolo set di attributi dei profili."

## Che cos’è un profilo? {#what}

Un **profilo**, noto anche come &quot;destinatario&quot; nella console client, rappresenta un record archiviato nel database di Campaign e funge da componente chiave per [creare tipi di pubblico](create-audience.md) per le consegne e [aggiungere dati di personalizzazione](../personalization/personalize.md) al contenuto. Adobe Campaign consente di gestire facilmente i profili, dalla creazione di nuove voci all’accesso a una visualizzazione completa di tutti gli attributi e gli abbonamenti ai servizi dei profili, il tutto tramite l’interfaccia utente web di Campaign.

Inoltre, i **[!UICONTROL profili di test]**, identificati come &quot;profili di seed&quot; nella console client, ti consentono di eseguire il targeting di altri destinatari che non corrispondono ai criteri di targeting di una determinata consegna. Questi profili contengono informazioni di contatto fittizie o informazioni di contatto controllate dal mittente. I profili di test sono destinatari di bozze: vengono utilizzati per testare i messaggi inviando bozze. [Scopri come utilizzare i profili di test](test-profiles.md)

Sia i profili che i profili di test possono essere utilizzati per testare le consegne prima che raggiungano il pubblico previsto. In questo modo puoi visualizzare in anteprima il contenuto e la personalizzazione del messaggio, inviare bozze per il test e la convalida, valutare il rendering delle e-mail su varie piattaforme e dispositivi e verificare le pagine di destinazione. [Scopri come visualizzare in anteprima e verificare le consegne](../preview-test/preview-test.md)

➡️ [Scopri questa funzione nel video](#video)

## Accedere all’elenco dei profili {#access}

I profili sono accessibili e modificabili in Adobe Campaign Web dalla voce **[!UICONTROL Gestione clienti]** > **Profili** nella barra di navigazione a sinistra. Puoi anche accedervi nella visualizzazione **[!UICONTROL Explorer]** dal nodo **[!UICONTROL Profili e destinazioni]** > **[!UICONTROL Destinatari]**. Da qui è possibile sfogliare, creare e gestire cartelle o sottocartelle, nonché verificare le autorizzazioni associate. [Scopri come creare le cartelle](../get-started/permissions.md#folders)

>[!NOTE]
>
>A seconda delle autorizzazioni, potresti non avere accesso all’elenco completo dei profili memorizzati nel database. [Ulteriori informazioni sulle autorizzazioni](../get-started/permissions.md).

Puoi filtrare l&#39;elenco **[!UICONTROL Profili]** utilizzando il campo di ricerca o i filtri disponibili nel pulsante **Mostra filtri**. È possibile limitare i risultati a una [cartella](../get-started/permissions.md#folders) specifica utilizzando l&#39;elenco a discesa oppure aggiungere regole utilizzando [modeler query](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

Per accedere ai dettagli di un profilo, fai clic sul nome dall’elenco. Viene visualizzata una vista dettagliata del profilo, che consente di esplorarne gli attributi e i servizi a cui si è abbonato. [Scopri come esplorare i dettagli dei profili](create-profile.md)

Per eliminare un profilo, seleziona l&#39;opzione corrispondente dal menu **[!UICONTROL Altre azioni]**.

## Video dimostrativo {#video}

Scopri come accedere, gestire ed esplorare i profili tramite l’interfaccia utente web di Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
