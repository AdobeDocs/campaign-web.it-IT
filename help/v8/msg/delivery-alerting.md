---
audience: end-user
title: Avvisi di consegna
description: Scopri come utilizzare gli avvisi sulla consegna.
badge: label="Disponibilità limitata"
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: a28bc98d1735232d8aa0b0daaeca3969913e548c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 8%

---

# Introduzione all’avviso di consegna {#gs-delivery-alerting}

Gli avvisi sulla consegna sono un sistema di gestione degli avvisi che consente ai gruppi di utenti di ricevere automaticamente le notifiche e-mail con le informazioni sulle esecuzioni della consegna. I destinatari monitorano le consegne in corso elaborate da Adobe Campaign e intraprendono azioni appropriate in caso di problemi.

Le notifiche sono personalizzate in base a criteri di avviso specifici definiti tramite l’interfaccia utente web di Adobe Campaign.

Per ulteriori informazioni sulla gestione degli errori di consegna, consulta la [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

>[!AVAILABILITY]
>
>Questa funzionalità è a disponibilità limitata (LA). È limitata ai clienti che eseguono la migrazione **da Adobe Campaign Standard ad Adobe Campaign v8** e non possono essere distribuiti in nessun altro ambiente.

## Contenuti delle notifiche e-mail {#content}

Le notifiche e-mail includono le sezioni seguenti:

* **Riepilogo**: visualizza il numero di consegne che soddisfano i criteri definiti, con etichette e colori per ogni criterio.
* **Dettagli**: elenca tutti i criteri di consegna definiti per il dashboard e le consegne corrispondenti per ciascun criterio.

![Descrizione: questa schermata mostra il layout delle notifiche e-mail, incluse le sezioni di riepilogo e dettagli.](assets/alerting-email.png)

## Impostare gli avvisi di consegna {#set-up}

Per impostare questi avvisi, l’interfaccia utente di Campaign Web consente di creare e gestire:

* **Dashboard di avvisi sulla consegna**: specifica i destinatari, imposta i criteri di avviso da includere nel dashboard e accedi alla cronologia degli avvisi inviati. [Scopri come utilizzare le dashboard](../msg/delivery-alerting-dashboards.md).
* **Criteri di avviso consegna**: l&#39;interfaccia utente di Campaign Web fornisce criteri di avviso predefiniti, ad esempio consegne con bassa velocità effettiva o consegne la cui preparazione non è riuscita. Puoi aggiungere questi criteri alla dashboard o creare criteri personalizzati in base alle tue esigenze. [Scopri come utilizzare i criteri](../msg/delivery-alerting-criteria.md).

Ad esempio, notifica agli utenti con diritti di amministrazione solo le consegne non riuscite e avvisa gli utenti marketing delle consegne con un elevato rapporto di errori di mancati recapiti non permanenti. A questo scopo, crea due dashboard separate con i criteri appropriati per ogni gruppo di destinatari.

>[!NOTE]
>
>Per accedere e configurare dashboard e criteri di avviso, è necessario disporre di **diritti di amministrazione** o far parte del gruppo di sicurezza **Supervisori consegna**. Gli utenti standard non possono accedere alle dashboard nell’interfaccia di Adobe Campaign, ma possono ricevere notifiche di avviso. [Ulteriori informazioni su accesso e autorizzazioni](../get-started/permissions.md).