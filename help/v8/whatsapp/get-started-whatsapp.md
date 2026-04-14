---
audience: end-user
title: Introduzione ai messaggi WhatsApp
description: Scopri come creare e inviare messaggi WhatsApp con l’interfaccia utente web di Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
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
* [Token di autorizzazione utente con autorizzazioni appropriate](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Modelli Meta approvati](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Prima di procedere, è inoltre necessario riconoscere quanto segue:

* [Regole contenuto WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Conformità con i criteri di Meta](https://www.whatsapp.com/legal)
* [Limiti di conversazione di 24 ore](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


