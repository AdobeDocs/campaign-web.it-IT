---
audience: end-user
title: Gestione delle autorizzazioni nel web di Campaign
description: Ulteriori informazioni sulle autorizzazioni in Campaign web v8
badge: label="Beta"
source-git-commit: 5c7d60b3f59de2a5176a55d9556a3f1c6d2a7651
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---


# Accesso e autorizzazioni {#access-and-permissions}

Il controllo di accesso può limitare l’accesso a oggetti e dati da elenchi principali, come consegne, destinatari o flussi di lavoro. Queste restrizioni si applicano anche nella struttura di navigazione di Explorer. È inoltre necessario disporre delle autorizzazioni per creare, eliminare, duplicare e modificare oggetti dall&#39;interfaccia utente. Il controllo degli accessi viene gestito nella console client. Tutte le autorizzazioni in Campaign Web vengono sincronizzate con le autorizzazioni della console client di Campaign. Solo gli amministratori di Campaign possono definire e modificare le autorizzazioni utente. Ulteriori informazioni sulle autorizzazioni per gli utenti in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}.

Durante la navigazione nell’interfaccia utente di Campaign Web, puoi accedere a dati, oggetti e funzionalità in base alle autorizzazioni di cui disponi. Ad esempio, se non disponi delle autorizzazioni di accesso per una cartella, non puoi visualizzarla. Le autorizzazioni influiscono anche sulla gestione di oggetti e dati. Senza le autorizzazioni di scrittura per una cartella specifica, non puoi creare una consegna in tale cartella, anche se è possibile visualizzarla nell’interfaccia utente.

## Visualizza autorizzazioni {#view-permissions}

Dalla sezione **Esplora**, è possibile sfogliare le autorizzazioni per ciascuna cartella. Queste autorizzazioni sono impostate nella console client e vengono utilizzate per organizzare e controllare l’accesso ai dati di Campaign.


Per visualizzare le autorizzazioni per una cartella, effettua le seguenti operazioni:

1. Dalla sezione **Esplora** seleziona una cartella dal menu di navigazione a sinistra.
1. Fai clic sui tre punti nell’angolo in alto a destra e seleziona **Autorizzazioni cartella**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Controlla i dettagli nella schermata, come segue:

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   Un gruppo o un operatore può disporre di autorizzazioni di lettura, scrittura e/o eliminazione per i dati memorizzati nella cartella selezionata.

   Se il **Propaga** se questa opzione è attivata, tutte le autorizzazioni definite per una cartella vengono applicate a tutte le relative sottocartelle. Queste autorizzazioni possono essere sovraccaricate per ogni sottocartella.

   Se il **Cartella di sistema** è abilitata, l’accesso è consentito a tutti gli operatori, indipendentemente dalle loro autorizzazioni.

Ulteriori informazioni sulle autorizzazioni per le cartelle in [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Utilizzare le cartelle {#folders}

Puoi creare, rinominare, riordinare e spostare cartelle per organizzare i componenti e i dati. È inoltre possibile eliminare cartelle dallo stesso menu.

>[!CAUTION]
>
>Durante l’eliminazione di una cartella, vengono eliminati anche tutti i dati in essa memorizzati.

Per creare una cartella, effettua le seguenti operazioni:

1. Dalla sezione **Esplora** seleziona una cartella dal menu di navigazione a sinistra.
1. Fai clic sui tre punti nell’angolo superiore destro e scegli **Crea nuova sottocartella**.
1. Inserisci il nome della cartella e salva.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   La cartella viene aggiunta come sottocartella della cartella corrente. Accedi alla nuova cartella per creare i componenti direttamente al suo interno. Puoi anche creare un componente da qualsiasi cartella e salvarlo in quella nuova cartella dall’ **Opzioni aggiuntive** sezione delle proprietà, come mostrato di seguito per una consegna:

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

