---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi sulla consegna.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 9%

---

# Introduzione all’avviso di consegna {#gs-delivery-alerting}


Avvisi di consegna è un sistema di gestione degli avvisi che consente ai gruppi di utenti di ricevere automaticamente le notifiche e-mail con le informazioni sulle esecuzioni della propria consegna. I destinatari possono monitorare le consegne in corso elaborate da Adobe Campaign e intraprendere azioni appropriate in caso di problemi.

Le notifiche possono essere personalizzate in base a criteri di avviso specifici definiti tramite l’interfaccia utente web di Adobe Campaign.

Per ulteriori informazioni su come gestire gli errori di consegna, consulta la [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Contenuti delle notifiche e-mail {#content}

Le notifiche e-mail includono le sezioni seguenti:

* **Riepilogo**: visualizza il numero di consegne che soddisfano i criteri definiti, con etichette e colori per ogni criterio.
* **Dettagli**: elenca tutti i criteri di consegna definiti per il dashboard e le consegne corrispondenti per ciascun criterio.

![](assets/alerting-email.png)

## Impostare gli avvisi di consegna {#set-up}

Per facilitare la configurazione di questi avvisi, l’interfaccia utente di Campaign Web consente di creare e gestire:

* **Dashboard di avvisi sulla consegna**: specifica i destinatari, imposta i criteri di avviso da includere nel dashboard e accedi alla cronologia degli avvisi inviati. [Scopri come utilizzare i dashboard](../msg/delivery-alerting-dashboards.md)
* **Criteri di avviso consegna**: l&#39;interfaccia utente di Campaign Web fornisce criteri di avviso predefiniti (consegne con bassa velocità effettiva, consegne la cui preparazione non è riuscita...) che puoi aggiungere al dashboard. Puoi anche creare criteri personalizzati in base alle tue esigenze. [Scopri come utilizzare i criteri](../msg/delivery-alerting-criteria.md)

Supponiamo che tu voglia avvisare gli utenti con diritti di amministrazione solo in merito alle consegne non riuscite e gli utenti di marketing in merito alle consegne con un elevato rapporto di errori di mancato recapito non permanenti. A questo scopo, crea due dashboard separate con i criteri appropriati per ogni gruppo di destinatari.

>[!NOTE]
>
>Per accedere e configurare dashboard e criteri di avviso, è necessario disporre di **diritti di amministrazione** o far parte del gruppo di sicurezza **Supervisori consegna**. Gli utenti standard non possono accedere alle dashboard nell’interfaccia di Adobe Campaign, ma possono ricevere notifiche di avviso. [Ulteriori informazioni su accesso e autorizzazioni](../get-started/permissions.md)
