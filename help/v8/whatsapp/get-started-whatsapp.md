---
audience: end-user
title: Introduzione ai messaggi WhatsApp
description: Scopri come creare e inviare messaggi WhatsApp con l’interfaccia utente web di Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%
---
# Introduzione ai messaggi WhatsApp {#get-started-whatsapp}

Puoi inviare messaggi WhatsApp dall&#39;**interfaccia utente Web di Adobe Campaign** utilizzando la [API cloud](https://developers.facebook.com/docs/whatsapp/cloud-api/) di Meta. Utilizza WhatsApp nelle consegne autonome, nei flussi di lavoro delle campagne o all’interno delle campagne di marketing, insieme agli altri canali.

* **[!UICONTROL Consegne]**: nell&#39;interfaccia utente Web di Adobe Campaign, crea una consegna WhatsApp autonoma dal menu **[!UICONTROL Consegne]** nella barra a sinistra, simile a SMS o push. [Ulteriori informazioni](create-whatsapp.md).

* **[!UICONTROL Campagne]**: nell&#39;interfaccia utente Web di Adobe Campaign, apri una campagna e aggiungi una consegna WhatsApp dalla scheda **[!UICONTROL Consegne]** oppure orchestra gli invii con un flusso di lavoro associato alla campagna. [Ulteriori informazioni](../campaigns/create-campaigns.md).

* **[!UICONTROL Flussi di lavoro]**: nell&#39;area di lavoro del flusso di lavoro dell&#39;interfaccia utente Web di Adobe Campaign, aggiungi un&#39;attività di canale **[!UICONTROL WhatsApp]**, scegli un modello di consegna, quindi definisci il contenuto e le impostazioni nel dashboard di consegna. Ulteriori informazioni sulle attività dei canali in [questa sezione](../workflows/activities/channels.md).

## Prerequisiti {#prereq}

L&#39;integrazione di WhatsApp richiede quanto segue:

* Account Meta Business Manager
* [Account aziendale WhatsApp con nome mittente e numero di telefono verificati](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Token di autorizzazione utente con le autorizzazioni appropriate](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Modelli Meta approvati](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Prima di procedere, è inoltre necessario riconoscere quanto segue:

* [Regole di contenuto WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Conformità con le direttive Meta](https://www.whatsapp.com/legal)
* [Limiti di conversazione 24 ore](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


