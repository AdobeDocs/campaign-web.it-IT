---
title: Gestisci account esterno
description: Scopri come configurare gli account esterni
exl-id: 99648377-112b-428a-8faf-5268d730f19a
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 1%

---

# Account esterni per l’integrazione delle soluzioni Adobe {#integration-external-account}

A seconda del tipo di account esterno Adobe Solution Integration selezionato, segui i passaggi seguenti per configurare le impostazioni di connessione e account per un’integrazione perfetta con i servizi Adobe.

## Adobe Experience Cloud

Per connettersi alla console Adobe Campaign utilizzando un Adobe ID, è necessario configurare l’account esterno Adobe Experience Cloud (MAC).

![Schermata che mostra i campi di configurazione dell&#39;account esterno Adobe Experience Cloud MAC.](assets/external-MAC.png)

Per configurare l&#39;account esterno **[!UICONTROL Adobe Experience Cloud]**, compilare i campi seguenti:

* **[!UICONTROL Server IMS]**

  URL del server IMS. Assicurati che le istanze di stage e produzione puntino allo stesso endpoint di produzione IMS.

* **[!UICONTROL Ambito IMS]**

  Gli ambiti definiti qui devono essere un sottoinsieme di quelli per i quali è stato eseguito il provisioning da IMS.

* **[!UICONTROL Identificatore client IMS]**

  ID del client IMS.

* **[!UICONTROL Segreto client IMS]**

  Credenziali del segreto client IMS.

* **[!UICONTROL Server di richiamata]**

  URL di accesso dell’istanza di Adobe Campaign.

* **[!UICONTROL ID organizzazione IMS]**

  ID della tua organizzazione. Per trovare il tuo ID organizzazione, fai riferimento a [questa pagina](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=it){target=_blank}.

* **[!UICONTROL Maschera di associazione]**

  Sintassi che consentirà la sincronizzazione dei nomi di configurazione nel dashboard di Enterprise con i gruppi in Adobe Campaign.

* **[!UICONTROL Server]**

  URL dell’istanza di Adobe Experience Cloud.

* **[!UICONTROL Tenant]**

  Nome del tenant Adobe Experience Cloud.
