---
title: Introduzione a Adobe Campaign v8 per gli esperti di marketing
description: Scopri le funzionalità chiave di Campaign v8. È destinato agli addetti al marketing che eseguono la migrazione da Campaign Standard a Campaign v8.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 19%

---

# Introduzione per i marketer {#acs-gs-marketers}

Questa guida offre una panoramica delle funzionalità chiave di Campaign v8, per gli esperti di marketing che passano da Campaign Standard a Campaign v8.

Puoi accedere a Adobe Campaign v8 tramite la console client o l’interfaccia utente web. L’interfaccia web consente di creare, gestire ed eseguire azioni di marketing chiave. La nuova interfaccia di Adobe Campaign Web offre un’esperienza utente moderna e intuitiva per semplificare la progettazione e la consegna delle campagne di marketing. [Ulteriori informazioni](../../v8/get-started/user-interface.md).

Con la migrazione, tutti i dati da Campaign Standard vengono importati in Campaign v8, garantendo una transizione senza problemi con interruzioni minime delle operazioni in corso.

Puoi continuare a utilizzare le credenziali esistenti per accedere e connettersi alla nuova istanza di Adobe Campaign v8. Una volta effettuato l’accesso, puoi trovare tutti i profili e i flussi di lavoro di cui stai eseguendo la migrazione, consentendoti di continuare a lavorare sulle campagne.

La differenza principale risiede nell’interfaccia utente. Di seguito è riportato un confronto tra lo stesso flusso di lavoro nelle due interfacce:

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> I rilasci dell’interfaccia utente web di Adobe Campaign funzionano secondo un modello di distribuzione continua che consente un approccio più scalabile e graduale alla distribuzione delle funzioni. Controlla regolarmente le [Note sulla versione](../../v8/rn/release-notes.md) per ottenere gli ultimi aggiornamenti.

## Scopri l’interfaccia utente di Campaign Web {#acs-gs-marketers-ui}

Nel video seguente, scopri come accedere e navigare nell’interfaccia utente di Campaign Web e come personalizzare gli elenchi di inventario.

>[!VIDEO](https://video.tv.adobe.com/v/3453430?quality=12&learn=on&captions=ita){transcript=true}

Per ulteriori informazioni, consulta la documentazione seguente:

1. [Scopri l’interfaccia utente di Campaign Web](../../v8/get-started/user-interface.md)

1. [Sfoglia e filtra elenchi](../../v8/get-started/list-filters.md)


## Creare e gestire profili e pubblico {#acs-gs-marketers-profiles-and-audiences}

I concetti generali per la creazione e la gestione di profili e tipi di pubblico in Campaign v8 sono gli stessi di Adobe Campaign Standard. Scopri come iniziare con profili e pubblico in [questa sezione](../../v8/audience/gs-audiences-recipients.md).

Di seguito sono riportati alcuni collegamenti utili con cui iniziare.

### Gestire i profili {#acs-gs-marketers-profiles}

In Adobe Campaign, un profilo è un record memorizzato nel database che funge da componente chiave per la creazione di tipi di pubblico per le consegne e l’aggiunta di dati di personalizzazione al contenuto.

1. Scopri come accedere, gestire ed esplorare i profili utilizzando l’interfaccia utente di Campaign Web in questo video:

   >[!VIDEO](https://video.tv.adobe.com/v/3448372?quality=12&learn=on&captions=ita){transcript=true}

   Ulteriori informazioni sono disponibili nella [Guida introduttiva ai profili](../../v8/audience/about-recipients.md).

1. Scopri come [creare e gestire profili di test](../../v8/audience/test-profiles.md) in Campaign v8.

### Gestire i tipi di pubblico {#acs-gs-marketers-audiences}

I tipi di pubblico sono insiemi di profili che condividono comportamenti e/o caratteristiche simili. Questa raccolta di persone può essere generata, selezionata o caricata. Una volta creati, i tipi di pubblico possono essere utilizzati come popolazione target delle consegne.

Scopri come creare e gestire i tipi di pubblico, come selezionare i tipi di pubblico per una consegna e definire gruppi di controllo, in questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3453210?quality=12&learn=on&captions=ita){transcript=true}

Per ulteriori informazioni, consulta [Introduzione a Audiences](../../v8/audience/manage-audience.md){target="_blank"}.

Come in Campaign Standard, puoi aggiungere un gruppo di controllo alla consegna. Puoi definire un gruppo di controllo per evitare di inviare messaggi a una parte del pubblico e confrontare il comportamento successivo alla consegna rispetto al target principale. Questa opzione consente di misurare l’impatto della campagna.
Scopri come [impostare un gruppo di controllo](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Tutti i tipi di pubblico creati tramite l’attività Query di Campaign Standard vengono trasformati in un filtro predefinito in Campaign v8 durante la transizione. Campaign v8 supporta anche l’attività Query.
>
>* Il pubblico di lettura viene trasformato in attività di query con [filtro predefinito](../../v8/query/build-query.md)
>
>* Il filtro predefinito accetta solo il valore più recente dopo la migrazione del pubblico a Campaign v8.
>
>* I tipi di pubblico di tipo file in Campaign Standard vengono migrati come tipi di elenco senza dimensioni.

### Gestire le iscrizioni {#acs-gs-marketers-sub}

È possibile gestire e creare i servizi, ad esempio le newsletter, e controllare gli abbonamenti o i loro annullamenti. I passaggi chiave sono globalmente gli stessi di Campaign Standard. Per ulteriori informazioni, consulta le pagine seguenti:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Non frequente" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Creare servizi di iscrizione</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Non frequente" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Gestisci abbonati<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Convalida" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Inviare messaggi agli abbonati di un servizio</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Utilizzare piani, programmi e campagne {#acs-gs-marketers-plans}

Adobe Campaign v8 consente di configurare la gerarchia di cartelle per i piani e i programmi di marketing. Le funzionalità di piani, programmi e campagne sono simili a quelle di Campaign Standard e Campaign v8.

Per ulteriori informazioni, consulta la [documentazione dei piani e dei programmi](../../v8/administration/plans-programs.md).

Di seguito sono riportati alcuni collegamenti utili con cui iniziare. Le modifiche che possono influire sull’esperienza utente sono evidenziate nelle note sulla disponibilità.


### Creare una campagna {#acs-gs-marketers-campaign}

Adobe Campaign consente di orchestrare facilmente le iniziative di marketing mirate, utilizzando la funzionalità integrata di gestione delle campagne. Grazie alla possibilità di definire una pianificazione, puoi pianificare la durata e la tempistica delle campagne in modo da allinearle agli obiettivi strategici e massimizzare il coinvolgimento del pubblico.

![Flusso della campagna](assets/campaign-flow.png)

Per ulteriori informazioni sulle campagne, consulta la documentazione seguente:

1. [Introduzione alle campagne](../../v8/campaigns/gs-campaigns.md)
1. [Accedere alle campagne e gestirle](../../v8/campaigns/manage-campaigns.md)
1. [Creare la prima campagna](../../v8/campaigns/create-campaigns.md)


### Creare un flusso di lavoro {#acs-gs-marketers-wf}

L’interfaccia utente del flusso di lavoro è stata completamente ripensata nell’interfaccia utente di Campaign Web per facilitarne l’utilizzo, la configurazione, l’esecuzione e la risoluzione dei problemi. Come hai già fatto in Campaign Standard, con i flussi di lavoro puoi orchestrare l’intera gamma di processi e attività, migliorare la velocità e la scala di ogni aspetto delle campagne di marketing, dalla creazione di segmenti e preparazione dei messaggi alla consegna. Inoltre, i canali possono essere sincronizzati in un’unica interfaccia di facile utilizzo per l’orchestrazione delle campagne.

Scopri come funzionano i flussi di lavoro e come creare un flusso di lavoro di targeting in questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3453980?quality=12&learn=on&captions=ita){transcript=true}

Ulteriori dettagli sono disponibili nella [documentazione del flusso di lavoro](../../v8/workflows/gs-workflows.md).

L’interfaccia utente web di Adobe Campaign dispone di un modellatore di query nei flussi di lavoro che semplifica il processo di filtraggio del database in base a vari criteri. [Ulteriori informazioni su Query Modeler](../../v8/query/query-modeler-overview.md)

Per comprendere lo scopo e la funzionalità di ogni attività all&#39;interno del flusso di lavoro, esplora le informazioni dettagliate disponibili sulle [attività del flusso di lavoro](../../v8/workflows/activities/about-activities.md)

Ottimizza l&#39;efficienza del flusso di lavoro esaminando i [guardrail e limitazioni per i flussi di lavoro](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* La cronologia e i registri dell&#39;esecuzione del flusso di lavoro [&#x200B; sono disponibili in Adobe Campaign v8.](../../v8/workflows/start-monitor-workflows.md#logs-tasks)
>
>* I registri cronologici dei flussi di lavoro eseguiti nell’istanza Campaign Standard non vengono migrati a Campaign v8.
>
>* Le unità organizzative sono mappate al concetto di cartella per la mappatura e per garantire un controllo degli accessi simile.
>

## Creare e gestire le consegne {#acs-gs-marketers-deliveries}

Con l’interfaccia utente di Campaign Web, in qualità di addetto al marketing, puoi creare consegne autonome dal menu a sinistra **Consegne** oppure nel contesto di un flusso di lavoro, incluse o meno in una campagna. I passaggi chiave sono allineati con la tua esperienza precedente in Campaign Standard. Scopri come creare una consegna nella sezione seguente: [Documentazione sulla creazione e la gestione della consegna](../../v8/msg/gs-deliveries.md).

Collegamenti utili:

* **Modelli di consegna** - Per un processo di progettazione accelerato e migliorato, puoi creare modelli di consegna per riutilizzare contenuti e impostazioni facilmente personalizzati nelle campagne. Questa funzionalità ti consente di standardizzare l&#39;aspetto creativo, per essere più rapido nell&#39;esecuzione e nel lancio di campagne/ Ulteriori informazioni nella pagina [Modello di consegna](../../v8/msg/delivery-template.md).

* **Impostazioni di consegna** - Le impostazioni di consegna sono parametri tecnici di consegna definiti nel modello di consegna. Possono essere sovraccarichi per ogni consegna. Queste impostazioni sono disponibili dal pulsante Impostazioni disponibile quando si modifica una consegna o un modello di consegna. Per ulteriori informazioni, consulta la sezione [Impostazioni di consegna](../../v8/advanced-settings/delivery-settings.md).

* **Contenuto dinamico** - Le funzionalità di contenuto dinamico Web di Adobe Campaign ti consentono di personalizzare il contenuto in base alle informazioni raccolte sui destinatari. Utilizzando i contenuti dinamici, potrai assicurarti che le tue attività di marketing siano più rilevanti, evitando marketing di prodotti o servizi indesiderati o non necessari. Ulteriori informazioni nella sezione [Contenuto dinamico](../../v8/personalization/gs-personalization.md).

* **Test e bozze** - Una volta definito il contenuto della consegna, puoi utilizzare profili e profili di test per visualizzarlo in anteprima e testarlo prima di inviare il messaggio. Questo passaggio è fondamentale per garantirne l’accuratezza, ma è anche privo di errori nelle impostazioni di contenuto e personalizzazione. Vedi [Anteprima e test](../../v8/preview-test/preview-test.md).

* **Pianificazione** - Puoi impostare la data e l&#39;ora esatta per l&#39;invio dei messaggi. Scegliendo l’orario più appropriato per il messaggio di marketing, puoi ottimizzare i tassi di apertura.

   * Scopri come [pianificare una consegna autonoma](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Scopri come [pianificare una consegna in un flusso di lavoro](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **Aggiungi offerte** - Puoi aggiungere offerte alle consegne nell&#39;interfaccia utente Web di Adobe Campaign. Queste offerte sono disponibili dal menu a sinistra Offerte, che consente di accedere all’elenco delle offerte.  Scopri come [aggiungere offerte ai messaggi](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* È stata effettuata la migrazione delle consegne in stato bozza o terminato.
>
>* Le consegne con uno dei seguenti stati sono state migrate ad Adobe Campaign v8, ma devono essere preparate di nuovo: In transito / In corso / Annullato / Nuovo tentativo in corso / Errore di preparazione.
>
>* Le consegne con uno dei seguenti stati sono state migrate come consegne annullate: Per annullato / nuovo tentativo in corso.
>
>* I collegamenti di tracciamento, i collegamenti URL delle pagine mirror, i collegamenti di abbonamento/annullamento dell’abbonamento funzionano come in Campaign Standard.
>
>Vedere anche le sezioni seguenti: [Tracciamento e monitoraggio](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Branding](https://experienceleague.adobe.com/it/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} in Adobe Campaign.

### Consegna e-mail {#acs-gs-marketers-email}

Scopri come creare una consegna e-mail da zero, definire il pubblico, progettare il contenuto, simulare l’anteprima e inviare una bozza in questo video:

>[!VIDEO](https://video.tv.adobe.com/v/3454013?quality=12&learn=on&captions=ita){transcript=true}

Scopri come creare la tua prima e-mail mirata nella [Documentazione sulla creazione della prima e-mail](../../v8/email/create-email.md)

In Campaign v8, i passaggi dettagliati per la creazione, il test e l’invio di una consegna e-mail sono simili a quelli di Campaign Standard.

1. **Progetta e definisci il contenuto**

   La finestra di progettazione e-mail di Campaign v8 è simile a quella disponibile in Campaign Standard. Alcuni anni fa, l&#39;editor di posta elettronica legacy di Campaign Standard[è stato dichiarato obsoleto](https://experienceleague.adobe.com/it/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}. Dovresti aver già effettuato la transizione a Campaign E-mail Designer per creare e personalizzare il contenuto delle e-mail.

   Scopri come navigare in E-mail Designer. Scopri come strutturare e progettare un’e-mail da zero, come personalizzare e testare l’e-mail nel video seguente:

   >[!VIDEO](https://video.tv.adobe.com/v/3453573?quality=12&learn=on&captions=ita){transcript=true}

   E-mail Designer consente di creare e-mail accattivanti e personalizzate tramite un’interfaccia intuitiva con funzionalità di trascinamento della selezione. Ulteriori informazioni sono disponibili nella [documentazione di E-mail Designer](../../v8/email/get-started-email-designer.md)

   Scopri come creare un’e-mail caricando HTML, come renderla compatibile con il Designer e-mail e come convertirla in un modello in questo video:

   >[!VIDEO](https://video.tv.adobe.com/v/3447040?quality=12&learn=on&captions=ita){transcript=true}

   Un frammento di contenuto è un componente riutilizzabile a cui è possibile fare riferimento in uno o più messaggi. Ulteriori informazioni su [Frammenti di contenuto](../../v8/content/fragments.md) per semplificare la creazione della consegna di e-mail.

   Per accelerare e migliorare il processo di progettazione, puoi creare modelli autonomi per riutilizzare facilmente i contenuti personalizzati in Adobe Campaign. Vedi [Creare modelli e-mail](../../v8/content/create-email-templates.md)

1. **Anteprima e test**

   Scopri come visualizzare in anteprima il contenuto e la personalizzazione dei messaggi e-mail, inviare le consegne di test (bozze) e controllare il rendering delle e-mail nei client desktop, mobili e basati su web più diffusi, in questo video:

   >[!VIDEO](https://video.tv.adobe.com/v/3450345?quality=12&learn=on&captions=ita){transcript=true}

1. **Invia e-mail e controlla i registri**

   Una volta definiti il contenuto, il pubblico e la pianificazione, puoi preparare la consegna delle e-mail. Per ulteriori informazioni, consulta le sezioni seguenti:

   * [Preparare e inviare un’e-mail](../../v8/monitor/prepare-send.md)
   * [Monitorare i registri di consegna](../../v8/monitor/delivery-logs.md)


### Consegna SMS {#acs-gs-marketers-sms}

Le consegne SMS offrono un modo pratico ed efficiente per inviare messaggi di testo ai dispositivi mobili della clientela. Grazie a questa funzione è possibile creare, personalizzare e visualizzare in anteprima i messaggi basati su testo per una comunicazione efficace.

In Campaign v8, i passaggi dettagliati per la creazione, il test e l’invio di una consegna SMS sono simili a quelli di Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Lead" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/create-sms"><strong>Creare una consegna SMS</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Non frequente" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/content-sms"><strong>Progettare una consegna SMS<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Convalida" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/sms/send-sms"><strong>Anteprima e invio di una consegna SMS</strong></a>
</div>
<p>
</td>
</tr></table>

### Notifiche push {#acs-gs-marketers-push}

Le notifiche push sono essenziali per contattare gli utenti delle app mobili, anche quando non utilizzano attivamente l’app. Hanno scopi diversi come fornire aggiornamenti, promuovere azioni specifiche e inviare notifiche sulle offerte.

In Campaign v8, i passaggi dettagliati per la creazione, il test e l’invio di una notifica push sono simili a quelli di Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/create-push">
<img alt="Lead" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/create-push"><strong>Creare una consegna push</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/content-push">
<img alt="Non frequente" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/content-push"><strong>Progettare una consegna push<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/send-push">
<img alt="Convalida" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/msg/push/send-push"><strong>Anteprima e invio di una consegna push</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8 supporta sia il canale push Android che iOS. Per la transizione dei flussi di lavoro e delle consegne esistenti tramite il canale push, connettiti con il tuo Adobe Campaign Transition Manager. Ulteriori informazioni su [Configurazione canale](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* SDK V4 per applicazioni mobili è stato [dichiarato obsoleto in Campaign Standard](https://experienceleague.adobe.com/it/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} alcuni anni fa. Dovresti aver già effettuato la transizione a Adobe Experience Platform SDK, lo stesso utilizzato in Campaign v8.
> 

### Direct mail {#acs-gs-marketers-direct-mail}

Direct mail è un canale offline che consente di creare file per consegnare in massa lettere personalizzate alla clientela, come cartoline, volantini o cataloghi. Durante la creazione di una consegna direct mail, Adobe Campaign genera automaticamente un file di estrazione contenente tutti i profili target e i dati selezionati, come gli indirizzi postali e gli attributi del profilo.

In Campaign v8, i passaggi dettagliati per la creazione, il test e l’invio di una consegna direct mailing sono simili a quelli di Campaign Standard.


1. [Creare la consegna Direct Mail](../../v8/direct-mail/create-direct-mail.md)
1. [Definisci il file di estrazione](../../v8/direct-mail/content-direct-mail.md)
1. [Anteprima e invio](../../v8/direct-mail/send-direct-mail.md)

### Canale in-app {#acs-gs-marketers-in-app}

Il canale in-app non è disponibile in Campaign v8. Se devi inviare una notifica in-app, contatta il tuo rappresentante Adobe.

## Creare e gestire pagine di destinazione {#acs-gs-marketers-lp}

L’interfaccia utente di Adobe Campaign v8 per il web è dotata di un’esperienza utente rinnovata per le pagine di destinazione. Campaign ti consente di creare, progettare e condividere pagine di destinazione. Le pagine di destinazione consentono di indirizzare gli utenti a moduli online in cui possono aggiornare i dati, acconsentire o rinunciare alla ricezione delle comunicazioni o iscriversi a un servizio specifico, ad esempio una newsletter.

In qualità di utente di Campaign Standard che passa a Campaign v8, le pagine di destinazione esistenti sono state migrate all’interfaccia utente web di Campaign. Puoi accedere alla stessa gamma di funzionalità.

Per ulteriori informazioni sulle pagine di destinazione, consulta le sezioni seguenti:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Lead" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/create-lp"><strong>Creare pagine di destinazione</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Convalida" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/lp-content"><strong>Progettare pagine di destinazione</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Convalida" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/it/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Utilizzare i modelli di pagina di destinazione</strong></a>
</div>
<p>
</td>
</tr></table>


## Reporting {#acs-gs-marketers-reporting}

Adobe Campaign fornisce un set di [strumenti di reporting](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. In qualità di amministratore, puoi creare e configurare i rapporti da condividere con altri utenti di Campaign.

La suite di strumenti di reporting di Adobe Campaign fornisce informazioni utili sull’efficacia delle attività di marketing, consentendoti di ottimizzare le campagne per il massimo impatto. Ulteriori informazioni sono disponibili nella [documentazione sul reporting](../../v8/reporting/gs-reports.md).

Inoltre, in linea con l’esperienza Adobe Campaign Standard, il Reporting dinamico è disponibile in Campaign v8, per le consegne e-mail. Fornisce rapporti completamente personalizzabili e in tempo reale per misurare l’impatto delle attività di marketing. Consente di accedere ai dati del profilo, abilitando l’analisi demografica per dimensioni di profilo, come genere, città ed età, oltre ai dati funzionali delle campagne e-mail come aperture e clic. Ulteriori informazioni sono disponibili nella [documentazione di Reporting dinamico](https://experienceleague.adobe.com/it/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

>[!AVAILABILITY]
>
>* [Il reporting dinamico](https://experienceleague.adobe.com/it/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} può essere utilizzato per il reporting di consegne e-mail, campagne con consegne e-mail e messaggi transazionali. È inoltre disponibile l’analisi demografica per dimensione di profilo.
>
> * [La funzionalità di reporting per l&#39;interfaccia utente Web di Adobe Campaign](../../v8/reporting/campaign-reports.md) è disponibile anche per tutti gli utenti che passano da Adobe Campaign Standard ad Adobe Campaign v8.

Adobe Campaign offre tre diversi rapporti:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Convalida" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Rapporti sulla campagna</strong></a>
</div>
<p>
<div>
<p>Fornisci informazioni dettagliate su prestazioni, efficacia e risultati delle singole consegne, fornendo una panoramica completa.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Lead" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Rapporti sulle consegne</strong>
</div>
<p>
<div>
<p>Offri un’analisi approfondita delle prestazioni di ogni consegna, per canale: tassi di successo, coinvolgimento del pubblico e altre metriche essenziali. Ti consentono di valutare l’efficacia e l’impatto complessivi della campagna.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Rapporti globali" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong>Rapporti globali</strong></a>
</div>
<p>
<div>
<p>Offri un riepilogo consolidato complessivo delle metriche di traffico e coinvolgimento per ciascun canale all’interno dell’istanza Campaign. Questi rapporti sono costituiti da vari widget, ciascuno dei quali offre una prospettiva distinta sulle prestazioni della campagna o della consegna.</p>
</div>
<p>
</td>
</tr>
</table>
