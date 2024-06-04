---
audience: end-user
title: Informazioni sui flussi di lavoro di sola lettura
description: Scopri perché i flussi di lavoro sono in modalità di sola lettura
source-git-commit: 6985e8cb11f12ab7818cc71441a4d3b41f1a0493
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 13%

---

# Informazioni sui flussi di lavoro di sola lettura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Questo flusso di lavoro è di sola lettura"
>abstract="Impossibile modificare questo flusso di lavoro a causa dei diritti o del tipo di flusso di lavoro."

Alcuni flussi di lavoro possono essere in modalità di sola lettura. Puoi visualizzarlo con:

- La menzione **[!UICONTROL ** Sola lettura **]**  vicino al **[!UICONTROL Impostazioni]** pulsante
- Pulsanti di azione non accessibili

![](assets/readonly-workflow.png){zoomable="yes"}

Non è possibile modificare elementi in un flusso di lavoro di sola lettura. Non ti è consentito modificare le impostazioni delle attività.


![](assets/scheduler-readonly.png){zoomable="yes"}


Non si dispone anche dei diritti per eliminare il flusso di lavoro.

![](assets/readonly-rights.png){zoomable="yes"}

## Perché i flussi di lavoro di sola lettura

La modalità di sola lettura è riservata agli utenti che non dispongono di autorizzazioni e diritti di accesso per modificare tali flussi di lavoro. [Fai clic qui per ulteriori informazioni](../get-started/permissions.md)

Un utente della campagna può avere restrizioni sui dati a cui può accedere in Adobe Campaign. L’amministratore può dargli la possibilità di visualizzare alcune funzioni ma non di lavorarci.

## Tipi di flussi di lavoro di sola lettura

A seconda del tipo di flusso di lavoro, la modalità di sola lettura può essere diversa.

### Flussi di lavoro della campagna

Nel caso di un flusso di lavoro di sola lettura per una campagna, l’utente non può accedere al pulsante di monitoraggio.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Flussi di lavoro tecnici

I flussi di lavoro tecnici sono in modalità di sola lettura per gli utenti delle campagne.
I flussi di lavoro tecnici incorporati sono in modalità di sola lettura per tutti, anche per gli utenti amministratori. Ma l’utente può **pausa** o **stop** se necessario. Queste sono le uniche azioni consentite. [Fai clic qui per ulteriori informazioni](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}