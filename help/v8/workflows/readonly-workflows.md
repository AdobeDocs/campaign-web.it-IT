---
audience: end-user
title: Informazioni sui flussi di lavoro di sola lettura
description: Scopri perché i flussi di lavoro sono in modalità di sola lettura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 13%

---

# Informazioni sui flussi di lavoro di sola lettura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Questo flusso di lavoro è di sola lettura"
>abstract="Impossibile modificare questo flusso di lavoro a causa dei diritti o del tipo di flusso di lavoro."

Alcuni flussi di lavoro sono in sola lettura. I flussi di lavoro tecnici incorporati sono sempre di sola lettura, ma questa ristrutturazione può essere attivata anche su altri tipi di flusso di lavoro.

Gli utenti di Campaign potrebbero avere un accesso limitato ai dati di Adobe Campaign. Un amministratore di Campaign può concedere loro il diritto di visualizzare alcune funzioni, ma non di modificarle o modificarle. Le autorizzazioni utente sui dati sono fondamentali per garantire la sicurezza dei dati e dei processi. Ulteriori informazioni sulla gestione delle autorizzazioni in Campaign in [questa sezione](../get-started/permissions.md)

Quando un workflow è in modalità di sola lettura:

* La menzione **[!UICONTROL Sola lettura]** accanto al pulsante **[!UICONTROL Impostazioni]**
* Pulsanti di azione non accessibili

![](assets/readonly-workflow.png){zoomable="yes"}

Gli utenti non possono modificare elementi in un flusso di lavoro di sola lettura. non possono modificare le impostazioni delle attività.

![](assets/scheduler-readonly.png){zoomable="yes"}

Gli utenti non possono eliminare il flusso di lavoro.

![](assets/readonly-rights.png){zoomable="yes"}


## Tipi di flussi di lavoro di sola lettura {#readonly-workflow-types}

A seconda del tipo di flusso di lavoro, la modalità di sola lettura può essere diversa.

### Flussi di lavoro della campagna {#readonly-campaign-wf}

Nel caso di un flusso di lavoro di sola lettura per una campagna, l’utente non può accedere al pulsante di monitoraggio.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Flussi di lavoro tecnici {#readonly-tech-wf}

I flussi di lavoro tecnici incorporati sono di sola lettura per tutti gli utenti della campagna, anche per l’amministratore. Tuttavia, gli utenti possono **sospendere** o **interrompere** se necessario. Queste sono le uniche azioni consentite.

![](assets/readonly-technical-workflow.png){zoomable="yes"}

Ulteriori informazioni sui flussi di lavoro tecnici in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)
