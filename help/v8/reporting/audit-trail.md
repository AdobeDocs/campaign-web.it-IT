---
product: campaign
title: Audit trail
description: Scopri come monitorare l’istanza con Campaign Audit trail
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%

---

# Audit trail{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Audit trail"
>abstract="La nuova funzionalità Audit trail fornisce un record dettagliato e cronologico di tutte le azioni e di tutti gli eventi eseguiti nell’istanza di Adobe Campaign in tempo reale."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=it" text="Consulta le note sulla versione"


Nell’interfaccia utente di Adobe Campaign Web, il **[!UICONTROL Audit trail]** Questa funzione offre agli utenti piena visibilità su tutte le modifiche apportate ad entità importanti all’interno dell’istanza, in genere quelle che influiscono in modo significativo sul regolare funzionamento dell’istanza.

>[!IMPORTANT]
>
>* L’interfaccia utente di Adobe Campaign Web non controlla le modifiche apportate all’interno di diritti utente, modelli, personalizzazioni o campagne.
>* L’audit trail può essere gestito solo dagli amministratori dell’istanza.

**[!UICONTROL Audit trail]** registra costantemente in tempo reale un registro dettagliato delle azioni e degli eventi che si verificano all’interno dell’istanza di Adobe Campaign. Offre un metodo comodo per accedere a un record cronologico di dati, che affronta query quali: lo stato dei flussi di lavoro, gli utenti più recenti per modificarli o le attività eseguite dagli utenti all’interno dell’istanza.

+++ Ulteriori informazioni sulle entità disponibili in Audit Trail

* **Audit trail dello schema di origine** consente di monitorare le attività e le modifiche recenti apportate agli schemi nella console client di Campaign V8.

  Per informazioni dettagliate sugli schemi, consulta [Documentazione di Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Audit trail del flusso di lavoro** consente di tenere traccia delle attività e delle modifiche recenti apportate ai flussi di lavoro, compresi i relativi stati correnti, ad esempio:

   * Inizio
   * Pausa
   * Interruzione
   * Riavvio
   * Pulizia uguale all’azione Cancella cronologia
   * Simula, che è uguale all’azione Avvia in modalità simulazione
   * Attivazione uguale all&#39;azione Esegui attività in sospeso ora
   * Arresto totale

  Per ulteriori informazioni sui flussi di lavoro, consulta questa [pagina](../workflows/gs-workflows.md).

* **Opzione audit trail** consente di monitorare le attività e le modifiche recenti apportate alle opzioni in Campaign V8.

  Per ulteriori informazioni sulle opzioni, consulta questa [pagina](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Audit trail della consegna** consente di controllare le attività e le ultime modifiche apportate alle consegne.

  Per ulteriori informazioni sulle consegne, consulta [pagina](../msg/gs-deliveries.md).

* **Account esterno** consente di verificare le modifiche apportate agli account esterni in Campaign V8, utilizzate da processi tecnici come flussi di lavoro tecnici o flussi di lavoro per campagne.

  Per ulteriori informazioni sull’account esterno, consulta questa [pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Mappatura consegna** consente di monitorare le attività e le modifiche recenti apportate alla mappatura delle consegne in Campaign V8.

  Per ulteriori informazioni sulla mappatura della consegna, consulta [pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Applicazione web** consente di verificare le modifiche apportate ai moduli web in Campaign V8 utilizzati per creare pagine con campi di input e selezione e che possono includere dati dal database.

  Per ulteriori informazioni sull’applicazione web, consulta questa [pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Offerta** consente di controllare le attività e le ultime modifiche apportate alle offerte.

  Per ulteriori informazioni sulle offerte, consulta questa [pagina](../msg/offers.md).

* **Operatore** consente di monitorare le attività e le modifiche recenti apportate agli operatori in Campaign V8.

  Per ulteriori informazioni sugli operatori, consulta questa [pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Accesso a Audit trail {#accessing-audit-trail}

Per accedere al di **[!UICONTROL Audit trail]**:

1. Sotto **[!UICONTROL Amministrazione]** menu, seleziona **[!UICONTROL Audit trail]** .

   ![](assets/audit-trail-1.png)

1. Il **[!UICONTROL Audit trail]** viene visualizzata la finestra con l&#39;elenco delle entità. L’interfaccia utente web di Adobe Campaign controlla le azioni di creazione, modifica ed eliminazione per flussi di lavoro, opzioni, consegne e schemi.

   Selezionate una delle entità per ulteriori informazioni sulle ultime modifiche.

1. Il **[!UICONTROL Entità di audit]** La finestra fornisce informazioni più dettagliate sull’entità scelta, ad esempio:

   * **[!UICONTROL Tipo]** : flusso di lavoro, opzioni, consegne o schemi.
   * **[!UICONTROL Entità]** : nome interno delle attività.
   * **[!UICONTROL Modificato da]** : nome utente dell’ultima persona che ha modificato questa entità.
   * **[!UICONTROL Azione]** : ultima azione eseguita sull’entità, Creata, Modificata o Eliminata.
   * **[!UICONTROL Data di modifica]** : data dell’ultima azione eseguita su questa entità.

   Il blocco di codice fornisce ulteriori informazioni su ciò che è stato modificato esattamente nell’entità.

   ![](assets/audit-trail-2.png)
