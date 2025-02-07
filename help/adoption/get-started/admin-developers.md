---
title: Introduzione ad Adobe Campaign v8 per amministratori e sviluppatori.
description: Questo tutorial offre una panoramica delle funzionalità chiave di amministrazione e gestione dati di Campaign v8. È destinato agli amministratori e all’addetto marketing tecnico che eseguono la migrazione da Campaign Standard a Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
exl-id: 1554f85f-22e1-4b51-a916-194ea0d24816
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '2657'
ht-degree: 8%

---

# Introduzione per amministratori e sviluppatori {#acs-gs-admin}

Questa pagina offre una panoramica delle principali funzionalità di amministrazione e gestione dati di Campaign v8. È destinato agli amministratori e agli esperti di marketing tecnico che passano da Campaign Standard a Campaign v8.

La principale modifica riguarda l’introduzione della console client, l’applicazione nativa che comunica con il server applicazioni di Adobe Campaign.

La console client di Campaign centralizza tutte le funzionalità e le impostazioni. È sincronizzato con l’interfaccia utente di Campaign Web, per garantire la coerenza in entrambi gli ambienti.

![](assets/client_console.png){zoomable="yes"}

[Ulteriori informazioni sull&#39;interfaccia utente della console client di Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"} .

## Architettura di Campaign v8 {#acs-gs-admi-archi}

L’architettura di Campaign è descritta nella documentazione di Campaign v8 (console). Scopri le nozioni di base in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Collegamento utile per iniziare:

* I componenti Adobe Campaign e l&#39;architettura globale sono descritti in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Consulta [Introduzione all&#39;architettura di Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} per comprendere l&#39;architettura di Campaign prima di iniziare a strutturare l&#39;istanza.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* La messaggistica transazionale (Message Center) è il modulo di Campaign v8 progettato per la gestione dei messaggi attivati. Si basa su un modello di architettura specifico descritto in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}.

## Console client di Campaign {#acs-gs-console}

### Installare la console client {#acs-gs-admin-console}

Le attività di amministrazione e configurazione vengono eseguite nella console client. Il primo passaggio consiste nella configurazione dell’ambiente.

La console client di Campaign è un’applicazione nativa che comunica con il server applicazioni Adobe Campaign tramite protocolli Internet standard, come SOAP e HTTP. La console client di Campaign centralizza tutte le funzionalità e le impostazioni e richiede una larghezza di banda minima in quanto si basa su una cache locale. Progettata per una facile distribuzione, la console client di Campaign può essere distribuita da un browser Internet, aggiornata automaticamente e non richiede alcuna configurazione di rete specifica in quanto genera solo traffico HTTP(S).

Nel video seguente viene illustrato come scaricare e installare Adobe Campaign Client Console e gestire la connessione all’istanza.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

Per ulteriori informazioni, vedere [Connetti a Campaign con la console client](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect){target="_blank"}.

La console client deve essere installata in un ambiente supportato. Ulteriori informazioni nella [Matrice di compatibilità di Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

### Scopri l’interfaccia della console client  {#acs-gs-ui}

Scopri l’interfaccia utente di Adobe Campaign V8 e come esplorare le funzioni principali con questo video di esercitazione.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

Per ulteriori dettagli, vedere [Utilizzare la console client](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"}.

## Amministrare l’ambiente {#acs-gs-admin-env}

Dopo aver installato la console client, seguire i passaggi descritti in questa documentazione per creare la connessione al server applicazioni: [Connessione alla documentazione del server applicazioni](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

Le procedure di sicurezza sono profondamente radicate nei nostri processi e strumenti interni di sviluppo e gestione del software e sono rigorosamente seguite dai nostri team interfunzionali per prevenire, rilevare e rispondere agli incidenti in modo rapido. Ulteriori informazioni sono disponibili in [Best practice per la sicurezza di Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Diritti di accesso e autorizzazioni {#acs-gs-admin-rights}

Adobe Campaign ti consente di definire e gestire i diritti assegnati agli utenti. Queste autorizzazioni vengono definite combinando le autorizzazioni del gruppo di operatori, i diritti denominati e le autorizzazioni per le cartelle.

In qualità di utente Campaign Standard che passa a Campaign v8, le autorizzazioni e i diritti di accesso rimangono gli stessi. I gruppi di sicurezza sono stati spostati da Adobe nei gruppi di operatori di Campaign v8 e le autorizzazioni per unità organizzative sono state trasferite nelle autorizzazioni della cartella. Utenti di Campaign   utilizza il proprio Adobe ID per connetterti a Campaign v8 e quindi può utilizzare gli stessi login e password di Campaign Standard.

Le [cartelle](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} della campagna sono nodi nella struttura dell&#39;elenco delle cartelle della console client. In base al tipo, contengono determinati tipi di dati. I programmi vengono materializzati dalle cartelle in Campaign v8. Puoi creare cartelle e gestirne le autorizzazioni per limitarne l’accesso. [Ulteriori informazioni](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Ulteriori informazioni sono disponibili nella [documentazione sulle autorizzazioni utente](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Pannello di controllo Campaign {#acs-gs-admin-cp}

Per quanto riguarda Campaign Standard, puoi utilizzare il Pannello di controllo Campaign per amministrare l’ambiente. Tieni presente che per v8, il Pannello di controllo Campaign fornisce funzionalità aggiuntive.

Consentendoti di gestire le impostazioni e di tenere traccia dell’utilizzo di ciascuna istanza, il Pannello di controllo Campaign ti aiuta a migliorare l’efficienza del tuo lavoro di amministratore di prodotto di Adobe Campaign. L’interfaccia intuitiva consente di monitorare facilmente l’utilizzo delle risorse chiave, nonché di eseguire attività amministrative come l’inserimento di indirizzi IP nell’elenco Consentiti, il monitoraggio dell’archiviazione SFTP, la gestione delle chiavi e altro ancora.

Ulteriori informazioni sono disponibili nelle [esercitazioni del Pannello di controllo](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} e nella [documentazione del Pannello di controllo](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=it){target="_blank"}.

* **Aggiungi indirizzi IP** - Il Pannello di controllo Campaign Campaign ti consente di impostare nuove connessioni alle istanze aggiungendo intervalli di indirizzi IP all&#39;elenco consentiti. Ulteriori informazioni nella [documentazione sull&#39;inserimento di IP nell&#39;elenco Consentiti](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Configurazione del sottodominio** - Puoi configurare una sottosezione del tuo dominio (tecnicamente una &quot;zona DNS&quot;) per l&#39;utilizzo con Adobe Campaign.
Ulteriori informazioni nella [documentazione sulla delega del sottodominio](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **Gestione dei server SFTP**: nel Pannello di controllo Campaign puoi interagire con tutti i server SFTP connessi alle istanze di Campaign a cui hai accesso. Ulteriori informazioni nella [documentazione sulla gestione SFTP](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Audit trail {#acs-gs-admin-audit-trail}

Come già disponibile in Campaign Standard, è possibile utilizzare Audit trail in Campaign v8 per accedere alla cronologia completa delle modifiche apportate all’interno dell’istanza.

Nell’interfaccia utente di Adobe Campaign Web, la funzionalità Audit trail offre agli utenti piena visibilità di tutte le modifiche apportate a entità importanti all’interno dell’istanza, in genere quelle che influiscono in modo significativo sul corretto funzionamento dell’istanza. Ulteriori informazioni sono disponibili nella [documentazione di Audit Trail](../../v8/reporting/audit-trail.md)

### Pacchetti di dati {#acs-gs-admin-audit-packages}

Analogamente a quanto si può ottenere in Campaign Standard, gli amministratori possono definire pacchetti per lo scambio di risorse tra diverse istanze di Adobe Campaign tramite file XML strutturati. Si può trattare di parametri di configurazione o dati.

Puoi utilizzare i pacchetti di dati per esportare e importare le impostazioni e i dati personalizzati della piattaforma. Un pacchetto può contenere diversi tipi di configurazioni e componenti, filtrati o meno. Scopri come utilizzare i pacchetti dati in Campaign v8 in [questa documentazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### Personalizzazione dell’interfaccia utente {#acs-gs-admin-ui}

Sono disponibili diverse opzioni per personalizzare l’interfaccia utente nella console client, ad esempio:

* **Visualizzazione elenchi e dati** - Le linee guida per la gestione delle impostazioni dell&#39;interfaccia utente, ad esempio elenchi, unità o visualizzazione dati, sono disponibili in questo documento: [Documentazione delle impostazioni dell&#39;interfaccia utente](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Gestione cartelle** - Le cartelle sono oggetti in Adobe Campaign che consentono di organizzare i componenti e i dati. Vengono inoltre utilizzati per gestire le autorizzazioni. Scopri come [utilizzare le cartelle](../../v8/get-started/work-with-folders.md).

* **Campi personalizzati** - I campi personalizzati sono attributi aggiuntivi aggiunti agli schemi predefiniti tramite la console Adobe Campaign. Questi campi personalizzati vengono visualizzati in varie schermate, ad esempio nei dettagli di un profilo o di un profilo di test. Ulteriori informazioni sono disponibili nella [documentazione di configurazione dei campi personalizzati](../../v8/administration/custom-fields.md).

## Configurare il branding {#acs-gs-admin-branding}

Ogni azienda dispone di linee guida per il brand che definiscono sia gli elementi visivi che i dettagli tecnici. Per quanto riguarda Adobe Campaign Standard, Adobe Campaign v8 ti consente di gestire queste linee guida a livello centrale, in modo da poter presentare ai clienti un’immagine del brand coerente in tutte le attività, dai loghi nelle e-mail agli URL e ai domini utilizzati nelle campagne. In qualità di amministratore tecnico, puoi creare e gestire più marchi all’interno di Adobe Campaign.

Ulteriori informazioni nella [documentazione sul branding](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Comprendere la creazione di modelli di dati {#acs-gs-admin-data-model-creation}

Analogamente a Campaign Standard, Adobe Campaign v8 viene fornito con il suo modello dati predefinito. Adobe Campaign si basa su un database Cloud contenente tabelle collegate tra loro. Ulteriori informazioni sono disponibili nella [documentazione del modello dati](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

Uno schema è un documento XML associato a una tabella di database. Definisce la struttura dati e descrive la definizione SQL della tabella. Consulta la [documentazione sulla creazione di schemi](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Scopri come creare uno schema ed estendere uno schema esistente in Campaign v8 in questo video:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Simile alle funzionalità disponibili in Campaign Standard, puoi creare risorse personalizzate. IN Campaign v8, le risorse personalizzate sono **schemi** personalizzati o estesi.

* Scopri come utilizzare lo schema in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Scopri come estendere uno schema esistente in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Scopri come creare un nuovo schema in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* Quando si crea o si estende uno schema, è necessario creare o modificare i moduli di input associati per rendere tali modifiche visibili agli utenti finali. Un modulo di input consente di modificare un’istanza associata a uno schema di dati dalla console client di Adobe Campaign. Il modulo è identificato dal nome e dallo spazio dei nomi. Consulta la [documentazione sulla creazione di moduli di input](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Flussi di lavoro e gestione dati {#acs-gs-admin-data-management}

Come Adobe Campaign Standard, Adobe Campaign v8 include un modulo del flusso di lavoro che ti consente di orchestrare l’intera gamma di processi e attività tra i diversi moduli del server applicazioni. Questo ambiente grafico completo ti consente di progettare processi inclusi segmentazione, esecuzione di campagne, elaborazione di file, partecipazione di utenti, ecc. Il motore del flusso di lavoro esegue e tiene traccia di questi processi. Scopri come iniziare a utilizzare i flussi di lavoro in Campaign v8 in [questa documentazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}.

Di seguito sono riportati i collegamenti ad altre risorse utili:

* Scopri le dimensioni di targeting e le tabelle di lavoro e come Adobe Campaign gestisce i dati tra diverse origini dati in questo video:

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Campaign ti aiuta ad aggiungere contatti al database Cloud. È possibile caricare un file, pianificare e automatizzare più aggiornamenti dei contatti, raccogliere dati sul Web o immettere le informazioni del profilo direttamente nella tabella dei destinatari.  Ulteriori informazioni sono disponibili nella [documentazione sull&#39;importazione di dati (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}.

* Puoi esportare facilmente i diversi rapporti in formato PDF o CSV, per condividerli, manipolarli o stamparli. Ulteriori informazioni nella [documentazione sull&#39;esportazione dei dati](../../v8/reporting/export-reports.md).

## API REST {#acs-gs-admin-apis}

Le API REST di Campaign mirano a creare integrazioni per Adobe Campaign e a creare il proprio ecosistema interfacciando Adobe Campaign con il pannello di tecnologie utilizzato.

In qualità di utente Campaign Standard che passa a Campaign v8, puoi accedere alle API REST.

Ulteriori informazioni sono disponibili nella [documentazione API REST](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Tieni presente che alcune raccomandazioni e limitazioni si applicano alle API REST durante la transizione da Campaign Standard a Campaign v8. Sono elencati in [questa pagina](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}. Restrizioni specifiche si applicano anche durante la transizione a Campaign v8 come elencato nella nota sulla disponibilità seguente:

>[!AVAILABILITY]
>
>* I valori PKEY cambiano tra l’istanza Campaign Standard esistente e l’istanza Campaign v8 migrata. Nel caso in cui le PKEY siano memorizzate in un database esterno, l’implementazione deve cambiare in modo tale da dover chiamare le API principali di Adobe Campaign v8, che fornisce collegamenti pkey/hrefs con le PKEY, e le chiamate API successive devono essere formate in modo dinamico consumando le pkey /hrefs dalle chiamate API precedenti&#x200B;
>
>* In Campaign v8, per lo stesso corpo in cui il veicolo è collegato al profilo&#x200B; viene visualizzato un errore La proprietà firstName non è valida per `cusVehicle`, ma un corpo della richiesta con solo gli attributi senza collegamento funziona correttamente. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* Il fuso orario viene mostrato all&#39;utente come parte della chiamata API REST `profileAndServicesExt/profile` e non della chiamata API REST `profileAndServices/profile` poiché viene aggiunto in uno schema esteso come parte della migrazione dei dati. &#x200B;
>
>* `ccpaOptOut` viene mostrato all&#39;utente solo come parte della chiamata API REST `profileAndServicesExt/profile` e non come chiamata API REST `profileAndServices/profile` poiché viene aggiunto in uno schema esteso come parte della migrazione dei dati.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Servizi di iscrizione {#acs-gs-admin-sub}

Come in Campaign Standard, in qualità di amministratore puoi creare servizi di abbonamento e gli esperti di marketing possono inviare messaggi ai loro abbonati. I concetti chiave e i passaggi di implementazione sono allineati con Campaign Standard. Di seguito sono riportati collegamenti e video utili.

Scopri come impostare e gestire gli abbonamenti e avere come target gli abbonati.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* Consulta la [documentazione sull&#39;interfaccia utente Web dei servizi di abbonamento](../../v8/audience/manage-subscribers.md).

* Consulta anche la documentazione per impostare i servizi di abbonamento nella console client in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}.

## Messaggi e consegne{#acs-gs-msg}

### Configurare i canali di consegna {#acs-gs-admin-channels}

In qualità di Campaign Standard, Adobe Campaign v8 ti consente di inviare campagne cross-channel tra cui e-mail, SMS, notifiche push e direct mail; inoltre, misura la loro efficacia utilizzando vari rapporti dedicati. Questi messaggi sono progettati e inviati tramite le consegne e possono essere personalizzati per ogni destinatario. Le funzionalità di base includono il targeting, la definizione e la personalizzazione dei messaggi, l’esecuzione delle comunicazioni e i relativi rapporti operativi. Il punto di accesso funzionale principale è l’assistente alla consegna. Permette di sfruttare diverse funzionalità incluse in Adobe Campaign.

In qualità di amministratore, devi definire le configurazioni del canale. Per ulteriori informazioni, fai riferimento ai collegamenti riportati di seguito.

* **E-mail** - Le impostazioni delle e-mail sono tutte dettagliate in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}.
* **SMS** - Scopri come configurare il tuo canale SMS in [questa documentazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.
* **Notifiche push** - I passaggi per configurare il canale delle notifiche push sono descritti in dettaglio [in questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
* **Messaggistica transazionale** - I passaggi per configurare [Messaggistica transazionale](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} in Campaign v8 sono descritti in dettaglio [in questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Account esterni {#acs-gs-ext-accounts}

In qualità di amministratore, sei responsabile della configurazione e della manutenzione degli account esterni di Campaign. Come in Campaign Standard, gli account esterni vengono utilizzati da processi tecnici come flussi di lavoro tecnici o flussi di lavoro per campagne.

Il processo di transizione a Campaign v8 si occupa degli account esterni Campaign Standard esistenti.

Ulteriori informazioni sono disponibili nella [documentazione dell&#39;account esterno](../../v8/administration/external-account.md).


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Contenuto dinamico {#acs-gs-dyn-content}

Utilizza Campaign per creare contenuti dinamici e inviare messaggi personalizzati. Le funzionalità di personalizzazione possono essere combinate per migliorare i messaggi e creare un’esperienza utente personalizzata.

Con Campaign v8, in qualità di amministratore, puoi definire blocchi di contenuto dinamici e come utilizzarli per personalizzare il contenuto della consegna e-mail in questo video:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Collegamenti utili:

* [Introduzione alla personalizzazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [Usa blocchi di personalizzazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [Crea contenuto condizionale](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Origini dati Personalization](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Modelli di consegna {#acs-gs-templates}

L’utilizzo dei modelli di consegna è un requisito in Campaign v8, come in Campaign Standard.

Per un processo di progettazione accelerato e migliorato, crea modelli di consegna per riutilizzare facilmente contenuti e impostazioni personalizzati nelle campagne. Questa funzionalità consente di standardizzare l’aspetto creativo per velocizzare l’esecuzione e il lancio delle campagne. Scopri come creare modelli di consegna nell’interfaccia utente web di [Campaign](../../v8/msg/delivery-template.md). Vedi anche come creare modelli di consegna nella console client in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Regole di tipologia {#acs-gs-admin-rules}

In qualità di amministratore, sei responsabile della creazione e della gestione delle regole di tipologia per le consegne. Come in Adobe Campaign Standard, in Campaign v8, le regole di tipologia sono regole aziendali che ti consentono di eseguire controlli e filtrare il messaggio prima di inviarlo.

Durante la transizione a Campaign v8 da un ambiente Campaign Standard, le regole di tipologia vengono spostate in Campaign v8.

In Campaign v8, le regole di tipologia sono dotate di un’opzione di ottimizzazione campagna specifica. Questo modulo consente di controllare, filtrare e monitorare l’invio delle consegne. Per evitare conflitti tra campagne, Adobe Campaign può sottoporre a test diverse combinazioni applicando specifiche regole di vincolo. Ciò garantisce che i messaggi inviati soddisfino le esigenze e le aspettative dei clienti e le politiche di comunicazione aziendali. Ulteriori informazioni sono disponibili nella [documentazione sulle regole di tipologia](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}.

### Gestione della quarantena {#acs-gs-admin-quarantine}

Tutti gli indirizzi e le regole di quarantena messi in quarantena sono stati migrati dall’ambiente Campaign Standard a Campaign v8. Non è necessaria alcuna azione specifica per la gestione della quarantena.

In qualità di amministratore, impara a gestire la quarantena in Campaign v8 a partire da [questa pagina](../../v8/audience/quarantine.md). Consulta anche la documentazione dettagliata della console client sulla gestione della quarantena in [questa sezione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}.


## Gestire le integrazioni Adobe Campaign {#acs-gs-integrations}

Puoi collegare la tua istanza di Campaign con le soluzioni Adobe Experience Cloud per combinare le funzionalità. Adobe Campaign è dotato di diversi connettori che consentono di comunicare con applicazioni esterne, connettersi ai motori di database, condividere e sincronizzare i dati. Scopri come combinare le tue soluzioni in [questa documentazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"}.

In qualità di utente Campaign Standard che migra a Campaign v8, ti vale quanto segue:

* Se utilizzi queste integrazioni con Campaign Standard, le configurazioni e i dati di **Adobe Analytics** e **Audience Manager** sono stati migrati da Adobe.
* Se l&#39;ambiente Campaign Standard è stato integrato con **Adobe Experience Manager**, Adobe consiglia di passare a **Adobe Experience Manager as a Cloud Service** in modo da poter utilizzare questa funzionalità durante la progettazione delle e-mail nell&#39;interfaccia utente di Campaign Web e facilitare la gestione semplificata dei contenuti e dei moduli di consegna e-mail direttamente nell&#39;ambiente Adobe Experience Manager. Ulteriori informazioni in [questa pagina](../../v8/integrations/aem-content.md).
Campaign può essere integrato anche con Adobe Experience Manager 6.5. Per configurare questa integrazione, consulta [questa documentazione](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Se l&#39;ambiente Campaign Standard è stato integrato con **Triggers**, è necessario configurare questa integrazione in Campaign v8 come descritto in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}.
* Se l&#39;ambiente Campaign Standard è stato integrato con **Adobe Target**, è necessario configurare questa integrazione in Campaign v8 come descritto in [questa pagina](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}.
