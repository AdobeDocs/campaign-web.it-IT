---
audience: end-user
title: Gestione delle autorizzazioni nell’interfaccia utente di Campaign Web
description: Ulteriori informazioni sulle autorizzazioni nell’interfaccia utente di Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 14%

---

# Autorizzazioni {#permissions}

Ogni utente di Adobe Campaign dispone di autorizzazioni e restrizioni specifiche nell’applicazione. L’utente può appartenere a un gruppo di operatori ed ereditare le autorizzazioni del gruppo.

In base alle loro autorizzazioni, un operatore può:

* Accedere ad alcune funzionalità
* Accedere a determinati dati
* Accedere ad alcune azioni (creare, modificare, eliminare)

Una procedura dettagliata per la configurazione delle autorizzazioni in Adobe Campaign è disponibile nella [documentazione di Adobe Campaign v8 (console)](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Autorizzazioni sulle cartelle {#folder-permissions}

In base ai tuoi diritti, puoi visualizzare e gestire le autorizzazioni per le cartelle nelle **[!UICONTROL Impostazioni cartella]**.

Di seguito è riportato un esempio di cartella di consegna:

![Esempio di impostazioni cartella in Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

Nella sezione **[!UICONTROL Protezione]** delle **[!UICONTROL Impostazioni cartella]** è possibile visualizzare e gestire (aggiungere o eliminare) gli operatori o i gruppi che possono accedere alla cartella.

![Esempio di impostazioni di protezione delle cartelle in Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Puoi fare clic direttamente sulle autorizzazioni e modificarle in **[!UICONTROL Consentite]** o **[!UICONTROL Negate]**.

![Esempio di autorizzazioni negate nelle impostazioni di protezione delle cartelle](assets/folder_security_denied.png){zoomable="yes"}

Se l&#39;opzione **[!UICONTROL Propagate]** è abilitata, tutte le autorizzazioni definite per una cartella verranno applicate a tutte le relative sottocartelle. Queste autorizzazioni possono essere ignorate per ogni sottocartella.

Se è selezionata l&#39;opzione **[!UICONTROL Cartella di sistema]**, l&#39;accesso è consentito a tutti gli operatori, indipendentemente dalle relative autorizzazioni.

È inoltre possibile [gestire le autorizzazioni per le cartelle nella console di Adobe Campaign](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Tutte le autorizzazioni nell’interfaccia utente di Campaign Web vengono sincronizzate con le autorizzazioni della console client di Campaign.