---
audience: end-user
title: Matrice di funzionalità dell’interfaccia utente/console client di Campaign Web
description: Elenco delle funzioni supportate nell’interfaccia utente di Campaign Web
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 50%

---

# Console client di Campaign Web e Campaign {#capabilities-matrix}

Le funzionalità chiave di Campaign sono disponibili nell’interfaccia utente di Campaign Web. Questa interfaccia è progettata principalmente per consentire agli addetti al marketing di pianificare, avviare e misurare le campagne di marketing. Tutte le funzionalità sono elencate [in questa pagina](../rn/whats-new.md).

La personalizzazione della piattaforma Campaign in base alle esigenze aziendali e di dati e la connessione ad altri sistemi viene gestita nella console client di Campaign. Di conseguenza, alcune impostazioni e funzionalità sono accessibili, create o gestite solo dalla console client di Campaign. Alcuni saranno disponibili in un successivo aggiornamento dell’interfaccia utente di Campaign Web.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Gestione delle campagne {#campaign-mgt-capabilities}

Con l’interfaccia utente di Campaign Web, puoi creare campagne cross-channel come descritto [in questa sezione](../campaigns/gs-campaigns.md). Le seguenti funzionalità sono disponibili solo nella console client di Campaign. Non sono accessibili nell&#39;interfaccia utente di Campaign Web, ma alcuni possono essere visualizzati dal menu [Explorer](user-interface.md#user-interface-explorer).

Utilizza i collegamenti forniti per consultare la documentazione di Campaign v8 (console client) e scopri come utilizzare queste funzionalità.

* **Calendario di marketing**. Il calendario della campagna mostra tutti i programmi, i piani, le campagne e le consegne in una sequenza temporale globale. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=it#campaign-calendar){target="_blank"}
* **Programmi e piani**. Ogni campagna appartiene a un programma, che appartiene a un piano. Nell’interfaccia utente di Campaign Web, tutte le campagne sono associate a un piano e a un programma predefiniti. Puoi creare e gestire piani e programmi solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=it#work-with-plan-and-program){target="_blank"}
* **Provider, budget e gestione costi**. Puoi configurare i provider di servizi coinvolti nei processi eseguiti all’interno delle campagne, incluse le strutture dei costi, e gestire i budget all’interno di ogni programma e campagna. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=it){target="_blank"}
* **Marketing distribuito** (marketing centrale/locale) Adobe Campaign offre un’app di marketing distribuito per l’implementazione di campagne di cooperazione tra enti centrali (sedi centrali, dipartimenti di marketing e altri) ed enti locali (punti vendita, agenzie regionali e altri). Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=it){target="_blank"}
* **Gestione delle risorse marketing** (MRM), controllo di obiettivi, simulazioni e costi. Adobe Campaign offre un’app di gestione delle risorse di marketing (MRM) che consente di controllare le azioni di marketing in modalità collaborativa tramite la gestione completa e il tracciamento in tempo reale delle attività, dei budget e delle risorse di marketing coinvolte. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=it){target="_blank"}
* **Gestione attività**. Come parte dell’app MRM, le attività di Campaign possono essere create, assegnate, tracciate e monitorate dalla dashboard della campagna. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=it){target="_blank"}

## Canali di comunicazione {#channels-capabilities}

Con l’interfaccia utente di Campaign Web, puoi creare, progettare e inviare **e-mail**, **SMS**, **notifiche push**, **direct mailing** e misurarne l’impatto utilizzando vari rapporti dedicati, come descritto in [questa sezione](../msg/gs-messages.md). Tuttavia, i seguenti canali **non** sono attualmente disponibili: in-app, LINE, call center/canale personalizzato, social marketing con X (Twitter).

Utilizza i collegamenti forniti per sfogliare la documentazione di Campaign v8 (console client) e scoprire ulteriori informazioni su questi canali.

* **Messaggistica LINE**. LINE è un&#39;applicazione per la messaggistica istantanea gratuita, voce e videochiamate, disponibile su tutti i dispositivi mobili e su PC. Adobe Campaign consente di inviare messaggi LINE solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=it){target="_blank"}
* **Call center e canali personalizzati**. Nell’ambiente Campaign è possibile implementare il call center e altri canali personalizzati. Questi canali possono essere disponibili solo nella console client. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=it#other-channels){target="_blank"}
* **Social marketing** con X (Twitter). Interagisci con la clientela tramite X (Twitter) pubblicando e inviando messaggi diretti. Questa funzionalità, disponibile con il componente aggiuntivo Social Marketing, è disponibile solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=it){target="_blank"}

## Pagine di destinazione e applicazioni web {#Webapps-capabilities}

Adobe Campaign consente di creare, progettare e condividere pagine di destinazione. L’esperienza delle pagine di destinazione è stata interamente riprogettata nella nuova interfaccia. Scopri come creare, progettare e pubblicare pagine di destinazione nell’interfaccia utente di Campaign Web [in questa sezione](../landing-pages/get-started-lp.md).

Di conseguenza, nella console client di Campaign non è possibile modificare, aggiornare o modificare una pagina di destinazione creata nell’interfaccia web e viceversa. I seguenti tipi di applicazioni web non sono disponibili nell’interfaccia utente di Campaign Web. Tuttavia, sono visibili nell’elenco delle pagine di destinazione. Utilizza i collegamenti forniti per sfogliare la documentazione di Campaign Classic v7 e scoprire ulteriori informazioni su queste app web:

* **Applicazioni web**. Adobe Campaign consente di creare e pubblicare applicazioni web dinamiche e interattive con dati precaricati dal database e contenuto adattato ai diritti dell’utente connesso. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=it){target="_blank"}
* **Moduli web**. Le pagine web e di destinazione progettate nella console client sono visibili nell’interfaccia utente di Campaign Web ma non possono essere modificate. Alcune opzioni possono differire tra il designer della pagina web della console client e il designer della pagina di destinazione fornito con l’interfaccia utente di Campaign Web. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=it){target="_blank"}
* **Sondaggi online**. Puoi creare sondaggi online e raccogliere risposte solo dalla console client. Questa funzionalità non è disponibile nell’interfaccia utente di Campaign Web. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=it){target="_blank"}

## Profili, profili di test e tipi di pubblico {#profiles-audiences-capabilities}

Puoi creare, gestire e aggiornare profili e profili di test sia nella console client di Campaign che nell’interfaccia utente di Campaign Web. Tutte le modifiche eseguite in un’interfaccia sono visibili nell’altra. Tuttavia, alcune impostazioni specifiche del destinatario e alcuni parametri avanzati potrebbero non essere presenti nella nuova interfaccia utente web di Campaign.

Nella nuova interfaccia utente web, il termine &quot;destinatario&quot; è stato modificato in &quot;profilo&quot; e gli &quot;indirizzi seed&quot; ora sono &quot;Profili di test&quot;.

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Tutti i tipi di pubblico creati nella console client di Campaign o in Adobe Experience Platform sono disponibili nell’interfaccia utente di Campaign Web.

I processi di importazione/esportazione one-shot descritti nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=it#import-jobs){target="_blank"} non sono disponibili nell&#39;interfaccia utente di Campaign Web. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## Progettazione dei contenuti {#content-capabilities}

Il nuovo E-mail Designer in arrivo con l’interfaccia utente di Adobe Campaign Web consente di creare e-mail accattivanti e personalizzate tramite un’intuitiva interfaccia con funzioni di trascinamento della selezione. Indipendentemente dal fatto che si inizi da una lavagna vuota, importando contenuto esistente o sfruttando i modelli esistenti, è possibile progettare e perfezionare tutto il contenuto per ogni e-mail. [Ulteriori informazioni](../email/edit-content.md)

Con questa nuova interfaccia utente, puoi gestire la sincronizzazione dei modelli e-mail da Adobe Experience Manager e integrarli con Adobe Experience Manager as a Cloud Service.

Tieni presente che le seguenti funzionalità non sono per il momento disponibili nell’interfaccia utente di Campaign Web. Utilizza i collegamenti forniti per sfogliare la documentazione di Campaign v8 (console client) e scoprire ulteriori informazioni su queste funzioni.

* **Creazione di blocchi di personalizzazione personalizzati**. Oltre ai blocchi di personalizzazione predefiniti, puoi creare blocchi personalizzati dalla console client. Questa funzionalità non è disponibile nell’interfaccia utente di Campaign Web. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=it#create-custom-personalization-blocks){target="_blank"}
* **Contenuto da moduli personalizzati**. Il modulo Gestione dei contenuti consente di creare e gestire moduli per assistere gli utenti nella creazione di contenuti in Campaign. Questa funzionalità è disponibile solo con la console client. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=it){target="_blank"}
* **AMP per e-mail**. Il formato AMP per e-mail consente di includere componenti AMP nei messaggi e di migliorare l’esperienza e-mail con contenuti avanzati e fruibili. Questa funzionalità è disponibile solo nella console client. [Ulteriori informazioni sono disponibili nella documentazione di Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=it){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Tipologie e regole di tipologia {#rules-capabilities}

Le tipologie sono set di regole di tipologia che vengono eseguite durante la fase di preparazione per applicare facilmente più regole di filtro a una consegna. Consentono agli esperti di marketing di standardizzare le pratiche aziendali su tutte le consegne controllando, filtrando e dando priorità all’invio delle consegne.

È possibile selezionare le regole di tipologia per una consegna o un modello di consegna nell&#39;interfaccia utente di Campaign Web, come descritto [in questa sezione](../advanced-settings/delivery-settings.md#typology). Tuttavia, la creazione, la gestione e la personalizzazione delle regole e delle regole di tipologia sono disponibili solo nella console client di Campaign.

Utilizza i collegamenti forniti per consultare la documentazione di Campaign v8 (console client) e scopri ulteriori informazioni sulle regole di tipologia:

* Creazione di regole di controllo. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=it){target="_blank"}
* Creazione di regole di affaticamento/pressione. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=it){target="_blank"}
* Creazione di regole di filtro. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=it){target="_blank"}
* Gestione delle regole di tipologia. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=it){target="_blank"}
* Simulazione della campagna. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=it){target="_blank"}
* Codifica JavaScript per la creazione di regole di tipologia. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=it#use-cases-on-pressure-rules){target="_blank"}

## Flussi di lavoro {#wf-capabilities}

La nuova interfaccia utente di Campaign Web include un’interfaccia dell’area di lavoro del flusso di lavoro riprogettata per progettare e gestire i processi. Le attività chiave del flusso di lavoro sono già disponibili nel nuovo design e alcune saranno disponibili in un aggiornamento futuro. Ulteriori informazioni sulle funzionalità del flusso di lavoro, inclusi guardrail e limitazioni, [in questa sezione](../get-started/guardrails.md).

Tieni presente che le seguenti funzionalità sono disponibili solo nella console client di Campaign:

* Scripting nei flussi di lavoro
* Attività ETL: esportazione, modifica schema, caricamento dati, estrazione dati, codice SQL

Ulteriori informazioni sulle attività del flusso di lavoro sono disponibili nella documentazione del flusso di lavoro di Adobe Campaign v8 (console) [qui](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=it){target="_blank"}.

## Gestione delle offerte {#offer-capabilities}

Puoi inviare le offerte nelle consegne create nell’interfaccia utente di Adobe Campaign Web. È necessario creare queste offerte nella console client utilizzando il modulo **[!UICONTROL Interazione]**. La progettazione dell’offerta, le regole di idoneità e la gestione delle offerte sono disponibili solo nella console client di Campaign. [Ulteriori informazioni](../msg/offers.md)

Scopri come gestire un catalogo delle offerte nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=it){target="_blank"}.

## Integrazioni con le soluzioni Adobe Experience Cloud {#exc-capabilities}

La nuova interfaccia utente moderna di Campaign semplifica la progettazione e la consegna delle campagne di marketing e introduce maggiore coerenza con altre soluzioni Adobe, tra cui Adobe Experience Platform e Adobe Experience Manager.

Le seguenti integrazioni sono disponibili dalla console client di Adobe Campaign e non sono ancora disponibili nell’interfaccia utente di Campaign Web. Utilizza i collegamenti forniti per sfogliare la documentazione di Campaign v8 (console client) e scoprire ulteriori informazioni su queste integrazioni:

* Utilizzo dei dati e condivisione dei KPI di Adobe Analytics. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=it){target="_blank"}
* Condivisione del pubblico con Adobe Experience Cloud (Adobe Audience Manager). [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=it){target="_blank"}
* Integrazione con Adobe Target. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=it){target="_blank"}
* Integrazioni con i trigger di Adobe Experience Cloud. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=it){target="_blank"}

## Reportistica {#reporting-capabilities}

La nuova interfaccia utente di Campaign Web include una serie di nuovi rapporti e KPI per tutti i canali: rapporti di consegna, rapporti sulle campagne e rapporti globali. Per ulteriori informazioni, consulta [questa sezione](../reporting/gs-reports.md)

Alcune funzionalità sono disponibili solo dalla console client. Sfoglia i collegamenti forniti alla documentazione di [Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=it){target="_blank"} e scopri di più.

* Rapporti di consegna e rendering della casella in entrata incorporati. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=it){target="_blank"}
* Personalizzazioni della reportistica. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=it){target="_blank"}
* Analisi descrittiva. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=it){target="_blank"}
* Analisi della campagna/Rapporti cubo. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=it){target="_blank"}
* Condivisione di rapporti secondo la pianificazione come PDF e CSV, o collegamento. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=it){target="_blank"}

## Modellazione e acquisizione dei dati {#data-capabilities}

L’interfaccia utente di Campaign Web non presenta le seguenti funzionalità. Sono disponibili solo nella console client:

### Account esterni {#external}

Adobe Campaign è dotato di un set di account esterni predefiniti per la connessione con i sistemi esterni. In qualità di amministratore di sistema di Campaign, puoi creare e gestire gli account esterni. [Ulteriori informazioni](../administration/external-account.md)

### Creazione ed estensione di uno schema {#schema}

La creazione, la modifica e l’estensione degli schemi sono riservate agli utenti avanzati. Queste funzionalità sono disponibili solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=it){target="_blank"}

### Funzionalità di gestione dei dati dei flussi di lavoro {#data}

La Gestione dei dati combina una serie di attività che risolvono problemi di targeting complessi offrendo strumenti più efficienti e flessibili come il caricamento dei dati, l’estrazione (file), l’aggiornamento dei dati, la modifica dello schema o i flussi di lavoro tecnici per l’importazione o l’esportazione. [Scopri le funzionalità di gestione dei dati dei flussi di lavoro nella console client](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=it#data-management){target="_blank"}

>[!NOTE]
>
>Alcune di queste attività sono disponibili solo nella console client, mentre altre sono disponibili nell&#39;interfaccia utente di Campaign Web, ad esempio le attività **Arricchimento**, **Caricamento file**, **Modifica origine dati** o **Modifica dimensione**. [Ulteriori informazioni sulle attività di targeting e gestione dati nell&#39;interfaccia utente di Campaign Web](../workflows/activities/about-activities.md#targeting)

### Configurazione Federated Data Access (FDA) {#fda}

La configurazione e la connessione di Campaign a sistemi esterni sono limitate agli utenti avanzati e sono disponibili solo dalla console client. [Ulteriori informazioni](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=it){target="_blank"}

## Approvazioni {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="Gestione delle approvazioni"
>abstract="La gestione delle approvazioni è disponibile solo dalla console client. "

L’interfaccia utente di Campaign Web non presenta una gestione dell’approvazione per contenuti, consegne, flussi di lavoro, campagne e destinazioni. Sono disponibili solo nella console client.

Scopri come gestire le approvazioni nel flusso di lavoro nella [documentazione di Campaign v8 (client console)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=it){target="_blank"}.

Scopri come gestire le approvazioni di consegna, contenuto e destinazione nelle campagne nella [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=it){target="_blank"}.

## Autorizzazioni {#permissions-capabilities}

Gli utenti di Campaign possono accedere all’interfaccia utente di Campaign Web solo con il proprio Adobe ID, tramite Adobe Identity Management System (IMS). Le autorizzazioni concesse agli utenti si applicano anche nell’interfaccia utente di Campaign Web.

Le autorizzazioni sono definite nella console client di Adobe Admin Console e Adobe Campaign, come descritto [in questa sezione](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=it). Dall’interfaccia utente web di Adobe Campaign non è possibile eseguire alcuna azione sulle autorizzazioni.

## Monitoraggio {#monitoring-capabilities}

Le funzionalità di monitoraggio della piattaforma Campaign sono disponibili solo nella console client e nel pannello di controllo Campaign. Non compaiono nell’interfaccia utente di Campaign Web.

Per ulteriori informazioni, consulta i collegamenti forniti alla documentazione di Campaign v8 (console client) e al Pannello di controllo di Campaign.

* [Monitoraggio del flusso di lavoro](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=it){target="_blank"}
* [Mappa termica del flusso di lavoro](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=it){target="_blank"}
* [Monitoraggio delle prestazioni](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=it){target="_blank"}
* [Monitoraggio del recapito messaggi](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=it){target="_blank"}