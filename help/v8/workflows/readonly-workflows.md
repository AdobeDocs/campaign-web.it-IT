---
audience: end-user
title: Informazioni sui flussi di lavoro di sola lettura
description: Scopri perché i flussi di lavoro sono in modalità di sola lettura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 4%

---

# Informazioni sui flussi di lavoro di sola lettura {#readonly-workflows}

>[!CONTEXTUALHELP]
>
Alcuni flussi di lavoro sono di sola lettura. I flussi di lavoro tecnici incorporati sono sempre di sola lettura, ma questa limitazione può essere applicata anche ad altri tipi di flussi di lavoro.

Gli utenti di Campaign potrebbero avere un accesso limitato ai dati di Adobe Campaign. Un amministratore di Campaign può concedere loro il diritto di visualizzare determinate funzioni, ma non di modificarle o modificarle. Le autorizzazioni utente sui dati sono essenziali per garantire la sicurezza dei dati e dei processi. Ulteriori informazioni sulla gestione delle autorizzazioni in Campaign sono disponibili in [questa sezione](../get-started/permissions.md).

Quando un workflow è in modalità di sola lettura:

* La menzione **[!UICONTROL Sola lettura]** viene visualizzata accanto al pulsante **[!UICONTROL Impostazioni]**.
* I pulsanti di azione non sono accessibili.

![Interfaccia del flusso di lavoro di sola lettura con il pulsante delle impostazioni e i pulsanti di azione disattivati.](assets/readonly-workflow.png){zoomable="yes"}

Gli utenti non possono modificare elementi in un flusso di lavoro di sola lettura. Non possono modificare le impostazioni delle attività.

![Interfaccia dell&#39;utilità di pianificazione in modalità di sola lettura, con opzioni di impostazioni disabilitate.](assets/scheduler-readonly.png){zoomable="yes"}

Gli utenti non possono eliminare il workflow.

![Interfaccia con diritti limitati per l&#39;eliminazione dei flussi di lavoro.](assets/readonly-rights.png){zoomable="yes"}

## Tipi di flussi di lavoro di sola lettura {#readonly-workflow-types}

La modalità di sola lettura può variare a seconda del tipo di flusso di lavoro.

### Flussi di lavoro della campagna {#readonly-campaign-wf}

In un flusso di lavoro di sola lettura per una campagna, l’utente non può accedere al pulsante di monitoraggio.

![Interfaccia del flusso di lavoro di Campaign in modalità di sola lettura, con le opzioni di monitoraggio disattivate.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Flussi di lavoro tecnici {#readonly-tech-wf}

I flussi di lavoro tecnici incorporati sono di sola lettura per tutti gli utenti di Campaign, inclusi gli amministratori. Tuttavia, gli utenti possono **sospendere** o **interrompere** se necessario. Queste sono le uniche azioni consentite.

![Interfaccia del flusso di lavoro tecnico in modalità di sola lettura, con le opzioni per sospendere o arrestare i flussi di lavoro.](assets/readonly-technical-workflow.png){zoomable="yes"}

Ulteriori informazioni sui flussi di lavoro tecnici in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).