---
audience: end-user
title: Scopri l’interfaccia
description: Interfaccia utente di Campaign Web v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: a875ba89417e5c50f7a1e767bf3430147fa7c4c0
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 78%

---

# Scopri l’interfaccia {#user-interface}

La nuova interfaccia di Campaign Web v8 offre un’esperienza utente moderna e intuitiva per semplificare la progettazione e la consegna delle campagne di marketing. Questa nuova interfaccia è integrata con le app e le soluzioni di Adobe Experience Cloud.


>[!NOTE]
>
>Questa documentazione viene spesso aggiornata per riflettere le recenti modifiche apportate all’interfaccia utente del prodotto. Tuttavia, alcune schermate possono risultare leggermente diverse dall’interfaccia utente che visualizzi.


## Menu di navigazione a sinistra {#user-interface-left-nav}

Sfoglia i collegamenti a sinistra per accedere alle funzionalità di Campaign Web v8. Diversi collegamenti presentano elenchi di oggetti che possono essere ordinati e filtrati. Puoi anche configurare le colonne per visualizzare tutte le informazioni che ti servono. Consulta questa [sezione](#list-screens). Alcune schermate di elenco sono di sola lettura. Gli elementi visualizzati nel menu di navigazione a sinistra e negli elenchi dipendono dalle autorizzazioni utente. Ulteriori informazioni sulle autorizzazioni sono disponibili in [questa sezione](permissions.md).

![](assets/home.png)

### Home {#user-interface-home}

Questa schermata include collegamenti chiave e risorse che permettono di accedere rapidamente alle funzionalità principali di Campaign Web v8.

L’elenco **Recenti** fornisce collegamenti alle consegne create e modificate di recente. Questo elenco ne mostra il canale, lo stato, il proprietario, le date di creazione e modifica.

Gli **Indicatori chiave di performance** consentono di verificare l’efficacia della piattaforma tramite KPI comuni. Ulteriori informazioni su questi KPI sono disponibili in [questa pagina](../reporting/kpis.md).

Puoi accedere alle principali pagine della guida di Campaign Web v8 dalla sezione **Apprendimento** della pagina home.

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Il menu **Explorer** mostra tutti i componenti e gli oggetti di Campaign con la stessa gerarchia di cartelle di quella presente nella console client. Sfoglia tutti i componenti, le cartelle e gli schemi di Campaign v8, controlla le autorizzazioni associate e crea cartelle e sottocartelle da questo menu."

Il menu **Explorer** mostra tutte le risorse e gli oggetti di Campaign con la stessa gerarchia di cartelle di quella presenti nella console client. Sfoglia tutti i componenti, le cartelle e gli schemi di Campaign v8 e crea consegne, flussi di lavoro e campagne.

Gli elementi visualizzati in **Explorer** dipendono dalle autorizzazioni utente. Se disponi dei diritti appropriati, è possibile inoltre aggiungere cartelle e sottocartelle. Ulteriori informazioni sulle autorizzazioni sono disponibili in [questa sezione](permissions.md).

Puoi configurare le colonne per personalizzare la visualizzazione e visualizzare tutte le informazioni necessarie. Consulta questa [sezione](#list-screens). Puoi anche aggiungere cartelle e sottocartelle, come descritto in [questa sezione](permissions.md#folders).

Per ulteriori informazioni sulla funzione Explorer di Campaign, la gerarchia di cartelle e risorse, consulta questa [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=it#ac-explorer-ui){target="_blank"}.

### Gestione delle campagne {#user-interface-campaign-management}

Nella sezione GESTIONE DELLE CAMPAGNE, puoi accedere a campagne di marketing, consegne e flussi di lavoro.

* **Campagne**: questo è l’elenco delle campagne e dei modelli di campagna. Per impostazione predefinita, per ogni campagna puoi visualizzare le date di inizio/fine/creazione/ultima modifica, lo stato corrente e il nome dell’operatore della campagna che l’ha creata. Puoi filtrare l’elenco per stato, date di inizio/fine, cartella oppure creare un filtro avanzato per definire criteri di filtro personalizzati. Per ulteriori informazioni sulle campagne, consulta [questa sezione](../campaigns/gs-campaigns.md).

* **Consegne**: scorri l’elenco delle consegne. Per impostazione predefinita, puoi visualizzarne lo stato, la data dell’ultima modifica e i KPI chiave. Puoi filtrare l’elenco per stato, data di contatto o canale. Fai clic su una consegna e-mail per aprire la relativa dashboard e ottenere una panoramica dei dettagli della consegna. Le consegne su altri canali sono di sola lettura. Per ulteriori informazioni sulle consegne, consulta [questa sezione](../msg/gs-messages.md).

  Per eliminare o duplicare una consegna, utilizza il pulsante **Altre azioni**.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Flussi di lavoro**: in questa schermata, è possibile accedere all’elenco completo dei flussi di lavoro e dei modelli di flusso di lavoro. Puoi controllarne lo stato, le date dell’ultima/successiva esecuzione e creare un nuovo flusso di lavoro o un nuovo modello di flusso di lavoro. È possibile filtrare l’elenco con gli stessi criteri degli altri oggetti. Inoltre, puoi filtrare i flussi di lavoro che appartengono o meno a una campagna. Per ulteriori informazioni sui flussi di lavoro, consulta [questa sezione](../workflows/gs-workflows.md).


### Gestione clienti {#user-interface-customer-management}

Nella sezione GESTIONE CLIENTI puoi visualizzare destinatari, tipi di pubblico e iscrizioni. Questi elenchi sono di sola lettura.

* **Destinatari**: accedi al database dei destinatari. Per impostazione predefinita, puoi visualizzarne l’indirizzo e-mail, il nome e il cognome. Per ulteriori informazioni sui destinatari, consulta [questa sezione](../audience/about-recipients.md).
* **Tipi di pubblico**: questo è l’elenco di tipi di pubblico. Per impostazione predefinita, puoi visualizzarne il tipo, l’origine, le date di creazione e ultima modifica e l’etichetta. È possibile filtrare l’elenco in base all’origine. Per ulteriori informazioni sui tipi di pubblico e gli elenchi, consulta [questa sezione](../audience/about-recipients.md).
* **Iscrizioni**: sfoglia gli elenchi delle iscrizioni. Per impostazione predefinita, puoi visualizzarne il tipo, la modalità e l’etichetta. Scopri come gestire le iscrizioni e il relativo annullamento nella [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=it){target="_blank"}.

### Gestione delle decisioni {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offerte"
>abstract="Sfoglia gli elenchi di offerte e modelli di offerta creati nella console utilizzando il modulo **Interazione**. Questi elenchi sono di sola lettura."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=it" text="Aggiungere offerte a una consegna"

Nella sezione GESTIONE DELLE DECISIONI, puoi visualizzare le offerte e i modelli di offerta. Questi elenchi sono di sola lettura.

* **Offerte**: sfoglia l’elenco delle offerte e i modelli di offerta creati nella console utilizzando il modulo **Interazione**. Per impostazione predefinita, puoi visualizzarne lo stato, le date di inizio e fine e l’ambiente. Puoi filtrare l’elenco per stato e per date di inizio e fine. Sono disponibili anche modelli di offerta.

Per scoprire come creare e inviare offerte tramite e-mail e SMS consulta [questa sezione](../content/offers.md).



## Guida contestuale {#user-interface-help}

Nell’interfaccia è disponibile una guida contestuale. Quando è disponibile, fai clic sull’icona `?` per visualizzare le informazioni della guida e i relativi collegamenti alla documentazione.

![](assets/context-help.png){width="40%" align="left"}

Con la nuova versione beta, il **Knowledge Assistant con Generazione basata sull’intelligenza artificiale**, incorporato nella guida contestuale, rivoluziona la ricerca della documentazione e le risposte alle domande relative alle procedure, esaminando attentamente gli archivi di documentazione con l’individuazione immediata e precisa delle informazioni necessarie.

Grazie alle funzionalità della Generazione basata sull’intelligenza artificiale di Campaign, questo assistente trasforma la tua esperienza, rendendo estremamente semplice il recupero delle informazioni e la risoluzione dei problemi. Sia che tu stia cercando assistenza in un’attività complessa o esplorando una vasta documentazione, il Knowledge Assistant con Generazione basata sull’intelligenza artificiale è lo strumento ideale che fornisce efficienza e precisione uniche in ogni interazione.

Per ulteriori informazioni, consulta [questa sezione](using-ai.md).



## Ulteriori informazioni {#learn-more}

Scopri come sfogliare, cercare e filtrare gli elenchi disponibili nell’ambiente Campaign [in questa pagina](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Autorizzazione necessaria"
>abstract="Prima di poter creare un segmento, l’amministratore deve concederti l’autorizzazione."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Autorizzazione necessaria"
>abstract="Prima di poter creare un segmento, l’amministratore deve concederti l’autorizzazione."

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Invio di rapporti globali"
>abstract="In questa schermata sono visibili le metriche di tracciamento della generazione di rapporti"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Tracciamento dei rapporti globale"
>abstract="In questa schermata sono visibili le metriche di tracciamento della generazione di rapporti"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Elenco dei flussi di lavoro in una campagna"
>abstract="Elenco dei flussi di lavoro in una campagna"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Creazione di destinatari"
>abstract="Creazione di destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Dettagli dei destinatari"
>abstract="Dettagli dei destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Informazioni di contatto dei destinatari"
>abstract="Informazioni di contatto dei destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Indirizzo destinatario"
>abstract="Indirizzo destinatario"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Account destinatari"
>abstract="Account destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campi personalizzati dei destinatari"
>abstract="Campi personalizzati dei destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Panoramica sulla scheda Destinatari"
>abstract="Panoramica sulla scheda Destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Punti di contatto dei destinatari"
>abstract="Punti di contatto dei destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Elenco iscrizioni destinatari"
>abstract="Elenco iscrizioni destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Selezione sottoscrizioni destinatari"
>abstract="Selezione sottoscrizioni destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Elenco idonei per le offerte dei destinatari"
>abstract="Elenco idonei per le offerte dei destinatari"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Anteprima delle offerte dei destinatari"
>abstract="Anteprima delle offerte dei destinatari"





>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Modello di consegna delle sottoscrizioni"
>abstract="Modello di consegna delle sottoscrizioni"





>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Pagine di destinazione"
>abstract="Pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Proprietà delle pagine di destinazione"
>abstract="Proprietà delle pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Pagine di destinazione"
>abstract="Pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Pianificazione delle pagine di destinazione"
>abstract="Pianificazione delle pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Pagina principale delle pagine di destinazione"
>abstract="Pagina principale delle pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Iscrizione alle pagine di destinazione"
>abstract="Iscrizione alle pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Invito all’azione per le pagine di destinazione"
>abstract="Invito all’azione per le pagine di destinazione"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulazione pagine di destinazione"
>abstract="Simulazione pagine di destinazione"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Attività non modificabile"
>abstract="Attività non modificabile"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Frammenti"
>abstract="Frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Salvataggio di frammenti"
>abstract="Salvataggio di frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Creazione di frammenti"
>abstract="Creazione di frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Proprietà dei frammenti"
>abstract="Proprietà dei frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo di frammenti"
>abstract="Tipo di frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Elenco frammenti"
>abstract="Elenco frammenti"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Dettagli dei frammenti"
>abstract="Dettagli dei frammenti"




>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Modello di contenuto"
>abstract="Modello di contenuto"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Proprietà del modello di contenuto"
>abstract="Proprietà del modello di contenuto"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Progettazione modello di contenuto"
>abstract="Progettazione modello di contenuto"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Selezione del modello di contenuto"
>abstract="Selezione del modello di contenuto"






>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Attività di caricamento file"
>abstract="Attività di caricamento file"






>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Attività Reconciliation"
>abstract="Attività Reconciliation"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Reconciliation targeting"
>abstract="Reconciliation targeting"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regole di riconciliazione"
>abstract="Regole di riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Dimensione targeting riconciliazione"
>abstract="Dimensione targeting riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Campo di selezione riconciliazione"
>abstract="Campo di selezione riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Attributo selezione riconciliazione"
>abstract="Attributo selezione riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condizione di creazione riconciliazione"
>abstract="Condizione di creazione riconciliazione"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Riconciliazione genera complemento"
>abstract="Riconciliazione genera complemento"





>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filtro di salvataggio del contenuto condizionale"
>abstract="Filtro di salvataggio del contenuto condizionale"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filtro di selezione del contenuto condizionale"
>abstract="Filtro di selezione del contenuto condizionale"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Contenuto condizionale nella riga dell’oggetto"
>abstract="Contenuto condizionale nella riga dell’oggetto"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Condizione oggetto contenuto condizionale"
>abstract="Condizione oggetto contenuto condizionale"




>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Proprietà pubblico"
>abstract="Proprietà pubblico"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Conteggio del pubblico"
>abstract="Conteggio del pubblico"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simulare profili di test"
>abstract="Simulare profili di test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simulare la selezione dei profili di test"
>abstract="Simulare la selezione dei profili di test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simulare l’invio di profili di test"
>abstract="Simulare l’invio di profili di test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simula registro e-mail"
>abstract="Simula registro e-mail"


>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Numero totale di abbonamenti"
>abstract="Numero totale di abbonamenti"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Iscrizioni nel periodo"
>abstract="Iscrizioni nel periodo"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Evoluzione complessiva delle sottoscrizioni"
>abstract="Evoluzione complessiva delle sottoscrizioni"
