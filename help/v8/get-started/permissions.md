---
audience: end-user
title: Gestione delle autorizzazioni nell’interfaccia utente di Campaign Web
description: Ulteriori informazioni sulle autorizzazioni nell’interfaccia utente di Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 18%

---


# Autorizzazioni {#permissions}

Ogni utente in Adobe Campaign ha le proprie autorizzazioni e restrizioni nell’applicazione. L’utente può far parte del gruppo di operatori ed ereditare le autorizzazioni del gruppo.

In base alle relative autorizzazioni, un operatore può:

* Accesso a determinate funzionalità
* Accesso a determinati dati
* Accesso a determinate azioni (creazione, modifica, eliminazione)

La procedura dettagliata per impostare le autorizzazioni in Adobe Campaign è disponibile nella [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Autorizzazioni per le cartelle {#folder-permissions}

In base ai tuoi diritti, puoi visualizzare e gestire le autorizzazioni per le cartelle nelle **[!UICONTROL Impostazioni cartella]**.

Di seguito è riportato un esempio su una cartella di consegna:

![](assets/folder_settings.png){zoomable="yes"}

Nella sezione **[!UICONTROL Protezione]** delle **[!UICONTROL Impostazioni cartella]** è possibile visualizzare e gestire (aggiungere o eliminare) gli operatori o i gruppi che possono accedere alla cartella.

![](assets/folder_security.png){zoomable="yes"}

Puoi fare clic direttamente sulle autorizzazioni e modificarle **[!UICONTROL Consentite]** o **[!UICONTROL Negate]**.

![](assets/folder_security_denied.png){zoomable="yes"}

Se è attiva l’opzione **[!UICONTROL Propaga]**, tutte le autorizzazioni definite per una cartella vengono applicate a tutte le relative sottocartelle. Queste autorizzazioni possono essere caricate per ogni sottocartella.

Se l&#39;opzione **[!UICONTROL Cartella di sistema]** è selezionata, l&#39;accesso è consentito a tutti gli operatori, indipendentemente dalle relative autorizzazioni.

È inoltre possibile [gestire le autorizzazioni per le cartelle nella console Adobe Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Tutte le autorizzazioni nell’interfaccia utente di Campaign Web sono sincronizzate con le autorizzazioni della console client di Campaign.
