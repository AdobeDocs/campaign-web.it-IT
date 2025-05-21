---
title: Introduzione ai profili
description: Scopri come monitorare e gestire i profili in Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 14%

---

# Introduzione ai profili {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profili"
>abstract="Un profilo è un record da usare come target per ricevere i messaggi inviati da Adobe Campaign. Da questo elenco, in base alle tue autorizzazioni, puoi visualizzare i dettagli dei profili. Utilizza le opzioni di filtro per sfogliare l’elenco. Puoi modificare e aggiornare un piccolo set di attributi dei profili."

## Che cos’è un profilo? {#what}

Un **profilo**, noto anche come &quot;destinatario&quot; nella console client, rappresenta un record archiviato nel database di Campaign. Funge da componente chiave per [creare tipi di pubblico](create-audience.md) per le consegne e [aggiungere dati di personalizzazione](../personalization/personalize.md) al contenuto. Adobe Campaign consente di gestire in modo semplice i profili, inclusa la creazione di nuove voci e l’accesso a una visualizzazione completa degli attributi di tutti i profili e degli abbonamenti ai servizi, tramite l’interfaccia utente web di Campaign.

Inoltre, **[!UICONTROL profili di test]**, identificati come &quot;profili di seed&quot; nella console client, consentono il targeting di destinatari aggiuntivi che non corrispondono ai criteri di targeting di una determinata consegna. Questi profili contengono informazioni di contatto fittizie o informazioni di contatto controllate dal mittente. I profili di test sono destinatari di bozze utilizzati per testare i messaggi inviando bozze. [Scopri come utilizzare i profili di test](test-profiles.md)

Sia i profili che i profili di test sono utili per testare le consegne prima che raggiungano il pubblico previsto. Questo consente di visualizzare in anteprima il contenuto e la personalizzazione dei messaggi, inviare bozze per il test e la convalida, valutare il rendering delle e-mail su varie piattaforme e dispositivi e testare le pagine di destinazione. [Scopri come visualizzare in anteprima e verificare le consegne](../preview-test/preview-test.md)

➡️ [Guarda il video su questa funzione](#video)

## Accedere all’elenco dei profili {#access}

I profili sono accessibili e modificabili in Adobe Campaign Web dalla voce **[!UICONTROL Gestione clienti]** > **Profili** nella barra di navigazione a sinistra. È inoltre possibile accedervi nella visualizzazione **[!UICONTROL Explorer]** dal nodo **[!UICONTROL Profili e destinazioni]** > **[!UICONTROL Destinatari]**. Da qui, sfogliare, creare e gestire cartelle o sottocartelle, nonché verificare le autorizzazioni associate. [Scopri come creare le cartelle](../get-started/permissions.md#folders).

>[!NOTE]
>
>A seconda delle autorizzazioni, potresti non avere accesso all’elenco completo dei profili memorizzati nel database. [Ulteriori informazioni sulle autorizzazioni](../get-started/permissions.md)

Filtra l&#39;elenco **[!UICONTROL Profili]** utilizzando il campo di ricerca o i filtri disponibili nel pulsante **Mostra filtri**. Limita i risultati a una [cartella](../get-started/permissions.md#folders) specifica utilizzando l&#39;elenco a discesa oppure aggiungi regole utilizzando [modeler query](../query/query-modeler-overview.md).

![Filtri disponibili nell&#39;elenco dei profili](assets/profiles-list-filters.png){zoomable="yes"}

Per accedere ai dettagli di un profilo, fai clic sul nome dall’elenco. Viene visualizzata una vista dettagliata del profilo, che consente di esplorarne gli attributi e i servizi a cui è abbonato. [Scopri come esplorare i dettagli dei profili](create-profile.md)

Per eliminare un profilo, seleziona l&#39;opzione corrispondente dal menu **[!UICONTROL Altre azioni]**.

## Video dimostrativo {#video}

Scopri come accedere, gestire ed esplorare i profili tramite l’interfaccia utente web di Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3448372?quality=12&captions=ita)