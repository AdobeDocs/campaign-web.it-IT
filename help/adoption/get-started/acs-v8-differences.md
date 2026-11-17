---
title: Differenze tra Campaign Standard e Campaign v8
description: Scopri cosa cambia durante la transizione da Campaign Standard a Campaign v8 e dove trovare i dettagli
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 5a6b111d1aaa2a34ce165eaf6d1b1a997fd8bc85
workflow-type: tm+mt
source-wordcount: '1916'
ht-degree: 3%
---
# Differenze tra Campaign Standard e Campaign v8 {#acs-v8-differences}

La maggior parte dei concetti sono gli stessi in Campaign Standard e Campaign v8. Questa pagina raccoglie le differenze che ti interessano dopo la transizione e contiene i collegamenti alla pagina che spiega ciascuna. Completa le guide per [addetti al marketing](marketers.md) e per [amministratori e sviluppatori](admin-developers.md).

* Per le modifiche terminologiche, vedere [Terminologia](#terminology).
* Per i controlli da eseguire e i problemi segnalati dopo una transizione, vedere [Controlli e risoluzione dei problemi dopo la transizione](post-transition-checks.md).
* Per le funzionalità disponibili solo nella console client, vedere [Console client Campaign Web e Campaign](../../v8/get-started/capability-matrix.md).

## Terminologia {#terminology}

La maggior parte dei concetti di Adobe Campaign v8 e Adobe Campaign Standard sono simili. Tuttavia, ci sono alcune differenze, a partire dalla terminologia.

| In Campaign Standard | In Campaign v8 |
|---|---|
| Risorse personalizzate | **Schemi** |
| Messaggi | **Consegne** |
| Utenti del prodotto | **Operatori** |
| Ruoli | Configurato con **diritti denominati** |
| Gruppi di sicurezza | **Gruppi di operatori** |
| Unità organizzative | Gestito tramite **autorizzazioni cartella** |

Inoltre, in qualità di utente esistente di Campaign, tieni presente che alcuni concetti sono stati rinominati per allinearsi ai più recenti standard terminologici. Queste modifiche si applicano solo all’interfaccia utente di Campaign Web e non vengono riportate nella console client.

| In Campaign Standard | In Campaign Web | Ulteriori informazioni |
|---|---|---|
| Destinatari | **Profili** | [Profili](../../v8/audience/gs-audiences-recipients.md) |
| Indirizzi di seed | **Profili di test** | [Consegne di prova](../../v8/preview-test/test-deliveries.md) |
| Analisi della consegna | **Preparazione consegna**. Per avviare la preparazione del messaggio, fare clic sul pulsante **Prepara**. | [Prepara e invia](../../v8/monitor/prepare-send.md) |
| Anteprima e-mail | Disponibile tramite il pulsante **Simula contenuto**. | [Anteprima e test](../../v8/preview-test/preview-test.md) |
| Elenchi | **Tipi di pubblico** | [Tipi di pubblico](../../v8/audience/gs-audiences-recipients.md) |

## Canali e contenuti {#channels}

I passaggi per creare e inviare messaggi sono simili in entrambi i prodotti, come descritto nella [guida per gli addetti al marketing](marketers.md). Le differenze seguenti riguardano la disponibilità dei canali, le consegne di test, le pagine di destinazione e i flussi di lavoro di direct mailing.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| Il canale in-app non è disponibile in Campaign v8. | [Canale in-app](marketers.md#acs-gs-marketers-in-app) |
| Per eseguire la transizione dei flussi di lavoro e delle consegne push esistenti, contatta il tuo Adobe Campaign Transition Manager. | [Notifiche push](marketers.md#acs-gs-marketers-push) |
| In Campaign Standard, un profilo di test potrebbe essere contrassegnato come **Abbondanza** per ricevere l&#39;invio finale. In Campaign v8, aggiungi un **gruppo di trap** nelle impostazioni Pubblico della consegna. | [Gruppo di trap](../../v8/audience/trap-group.md) |
| Le pagine di destinazione create nell’interfaccia utente di Campaign Web non supportano campi di input nascosti o JavaScript personalizzato. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
| In Campaign Standard, anche la transizione in uscita di un’attività di direct mailing trasportava il file generato. In Campaign v8, porta solo la popolazione target. Per inviare il file a un server, aggiungi un&#39;attività **Estrazione dati**, quindi un&#39;attività **Trasferimento file**. | [Direct mail](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Tipi di pubblico, flussi di lavoro e consegne {#data-and-workflows}

Queste differenze interessano i tipi di pubblico e i flussi di lavoro migrati da Campaign Standard, alcune opzioni di consegne ricorrenti e dell&#39;attività **Trasferimento file** e l&#39;ambito del reporting dinamico.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| I tipi di pubblico creati con l&#39;attività Query in Campaign Standard diventano [filtri predefiniti](../../v8/query/build-query.md) in Campaign v8. Campaign v8 supporta anche l’attività Query. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| Un’attività Read audience diventa un’attività Query con un filtro predefinito. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| Un filtro predefinito accetta solo il valore più recente dopo la migrazione del pubblico. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| I tipi di pubblico di tipo file diventano tipi di pubblico di tipo elenco senza dimensioni. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| I registri cronologici dei flussi di lavoro eseguiti in Campaign Standard non vengono migrati. | [Creare un flusso di lavoro](marketers.md#acs-gs-marketers-wf) |
| In Campaign Standard, puoi selezionare il periodo di aggregazione di un’e-mail ricorrente. Questa opzione non è disponibile in Campaign v8. | [Attività del canale](../../v8/workflows/activities/channels.md) |
| Il reporting dinamico riguarda le consegne di e-mail, le campagne con le consegne di e-mail e i messaggi transazionali. | [Reportistica](marketers.md#acs-gs-marketers-reporting) |

## Accesso e sicurezza {#access}

I gruppi di sicurezza, i ruoli e le unità organizzative di Campaign Standard vengono mappati ai gruppi di operatori, ai diritti denominati e alle autorizzazioni delle cartelle durante la transizione. Rivedi i punti seguenti, in particolare se alcuni utenti hanno diritti più ampi o più limitati rispetto a prima.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| I gruppi di sicurezza, i ruoli e le unità organizzative sono associati a gruppi di operatori, diritti denominati e autorizzazioni per le cartelle. I ruoli personalizzati non vengono migrati. | [Gestione degli accessi utente](user-management-acs.md) |
| Gli utenti con ruolo **Modello dati** ma non con ruolo **Amministrazione** ottengono l&#39;accesso **Amministrazione**. | [Gestione degli accessi utente](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Gli utenti assegnati a gruppi di sicurezza con unità organizzative parallele possono avere un accesso più ampio in Campaign v8. | [Assegnazione unità organizzativa parallela](user-management-acs.md#parallel-assignments) |
| L’accesso alle API transazionali dall’istanza di esecuzione richiede un nuovo profilo di prodotto. | [Mappatura profilo prodotto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Le richieste di accesso a dati personali possono pervenire sia in Campaign Standard che in Campaign v8 durante il periodo in cui l’ambiente Campaign Standard rimane attivo. | [Privacy e consenso](admin-developers.md#privacy-and-consent) |

## API e integrazioni {#apis-and-integrations}

Queste differenze influiscono sulle integrazioni che chiamano Campaign tramite l’API REST e sulle integrazioni con altre soluzioni e strumenti di Adobe.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| I valori PKEY cambiano dopo la migrazione. Se memorizzi le PKEY al di fuori di Campaign, segui invece gli href restituiti dall’API. | [Utilizzo chiave](#key-usage) |
| Alcuni campi del profilo migrati, come fuso orario e `ccpaOptOut`, vengono restituiti solo dall&#39;API `profileAndServicesExt/profile`. | [Fuso orario profilo e ccpaOptOut](#profile-timezone) |
| Adobe esegue la migrazione delle configurazioni di Adobe Analytics e Audience Manager. Devi configurare nuovamente le integrazioni Triggers e Adobe Target. | [Gestione integrazioni Adobe Campaign](admin-developers.md#acs-gs-integrations) |

## Raccomandazioni e limitazioni REST API {#rest-api-limitations}

I consigli e le limitazioni riportati di seguito si applicano alle API REST durante la transizione da Campaign Standard a Campaign v8.

### Autorizzazioni e sicurezza {#permissions}

#### Mappatura dei profili di prodotto {#rest-product-profiles}

In Campaign Standard, ti era stato concesso l’accesso alle API con un ruolo di amministratore elevato, indipendentemente dal profilo di prodotto assegnato. Campaign v8 introduce un diverso set di profili di prodotto, che richiede la mappatura dai profili di prodotto di Campaign Standard a Campaign v8.

Con la migrazione, due profili di prodotto vengono aggiunti agli account tecnici esistenti o precreati: Amministratore e Centro messaggi (per accedere alle API transazionali). Rivedi la mappatura del profilo di prodotto e assegna il profilo di prodotto necessario se non desideri che il profilo di prodotto Amministratore sia mappato con il tuo account tecnico.

#### ID tenant

Dopo la migrazione, per eventuali integrazioni future, si consiglia di utilizzare l&#39;ID tenant **Campaign v8** negli URL REST, sostituendo l&#39;ID tenant Campaign Standard precedente.

#### Utilizzo chiave

La gestione dei valori PKey varia tra Campaign Standard e Campaign v8. Se memorizzi le PKeys con Campaign Standard, assicurati che l’implementazione formi dinamicamente le successive chiamate API utilizzando le PKeys o gli href ottenuti da precedenti chiamate API.

### API disponibili {#available-apis}

Per il momento, è possibile utilizzare le API REST elencate di seguito:

* **Profili**
* **Servizi e abbonamenti**
* **Risorse personalizzate**
* **Flussi di lavoro**
* **Messaggi transazionali**

>[!AVAILABILITY]
>
>Le API REST elencate di seguito sono obsolete e non sono disponibili per l’uso:
>* Storico dei dati marketing
>* Unità organizzative
>* Gestione della privacy

### Filtro {#rest-filtering}

* Per utilizzare i filtri nei payload API REST, è necessario modificarli in Campaign v8 e fornire un nome da utilizzare nei payload. A tale scopo, accedere ai parametri aggiuntivi del filtro dalla scheda **[!UICONTROL Parametri]** e specificare il nome desiderato nel campo **[!UICONTROL Nome filtro nell&#39;API REST]**.

  ![](assets/api-filtering.png)


* Il prefisso &quot;by&quot; necessario per utilizzare i filtri personalizzati non è più necessario. Il nome del filtro deve essere utilizzato così com’è nelle richieste.

  Esempio:

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### Campi di database rilasciati {#dropped-fields}

Alcuni campi del database vengono eliminati durante la migrazione. Quando si utilizza un campo rilasciato, le API REST restituiscono valori vuoti. In futuro, tutti i campi rilasciati diventeranno obsoleti e verranno rimossi.

### PUBBLICA con risorse collegate {#post-linked}

Quando si utilizza il seguente formato del corpo della richiesta, con &quot;vehicleOwner&quot; che rappresenta il collegamento a &quot;nms:recipient&quot;:

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

Le informazioni sul collegamento vengono ignorate. Di conseguenza, viene generato un nuovo record in &quot;cusVehicle&quot; contenente solo i valori &quot;vehicleNumber&quot; e &quot;vehicleName&quot;. Tuttavia, il collegamento rimane nullo, con conseguente impostazione di &quot;vehicleOwner&quot; su null.

In Campaign v8, quando si utilizza la stessa struttura del corpo della richiesta e il &quot;veicolo&quot; è collegato a un profilo, si verifica un errore. Questo errore si verifica perché la proprietà &quot;firstName&quot; non è riconosciuta come valida per &quot;cusVehicle&quot;. Tuttavia, un corpo della richiesta che include solo gli attributi senza il collegamento funziona senza alcun problema.

### Operazioni PATCH {#patch}

* Campaign v8 non supporta PATCH con un corpo di richiesta vuoto: restituisce lo stato 204 Nessun contenuto.
* Sebbene Campaign Standard supporti PATCH per gli elementi/attributi all’interno di uno schema, le operazioni PATCH sulla posizione non sono supportate in Campaign v8. Il tentativo di eseguire un PATCH nel percorso genera un errore interno del server 500 con un messaggio di errore che indica che la proprietà &#39;zipCode&#39; non è valida per la risorsa &#39;profile&#39;.

### Risposte REST {#rest-responses}

La sezione seguente elenca le differenze minori tra le risposte REST di Campaign Standard e v8.

* Per singoli record GET, la risposta include il href nella risposta.
* Quando viene eseguita una query con l’attributo, Campaign v8 fornisce il conteggio e la paginazione nella risposta.
* Dopo le operazioni POST, i valori delle risorse collegate vengono restituiti nella risposta.

### Codici di errore e messaggi {#rest-errors}

La sezione seguente elenca le differenze tra i codici di errore e i messaggi di Campaign Standard e Campaign v8.

| Scenario | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| Usa una chiave PKey non valida nel corpo della richiesta | 500 - Attributo &#39;O5iRp40EGA&#39; sconosciuto (vedere la definizione dello schema &#39;Profiles (nms:recipient)&#39;). XTK-170036 Impossibile analizzare l’espressione &quot;@id = @O5iRp40EGA&quot;. | 404 - Impossibile decrittografare PKey. (PKey=@jksad) |
| Usa una chiave PKey non valida nell&#39;URI | 500 - Attributo &#39;O5iRp40EGA&#39; sconosciuto (vedere la definizione dello schema &#39;Profiles (nms:recipient)&#39;). XTK-170036 Impossibile analizzare l’espressione &quot;@id = @O5iRp40EGA&quot;. | 404 - Impossibile decrittografare PKey. (PKey=@jksad) Endpoint non supportato. (endpoint=rest/profileAndServices/profile/@jksad) |
| Utilizzo di due diverse chiavi non elaborate nell’URI e nel corpo della richiesta | 500 - RST-360011 Si è verificato un errore. Contattare l&#39;amministratore. RST-360012 Operazione non coerente sulla risorsa &#39;service&#39;. Impossibile aggiornare la chiave &#39;SVC3&#39; a &#39;SVC4&#39;. | 500 - Si è verificato un errore - contatta l’amministratore. |
| Utilizzo di PKey nell’URI e di una PKey non elaborata diversa nel corpo della richiesta | 500 - Esiste già un &quot;Servizio&quot; con la stessa chiave &quot;SVC4&quot;. Errore PGS-220000 PostgreSQL: ERRORE: il valore di chiave duplicato viola il vincolo univoco &quot;nmsservice_name&quot; DETAIL: la chiave (sname)=(SVC4) esiste già. | 500 - Si è verificato un errore - contatta l’amministratore. |
| Utilizzo di un raw-id non esistente nell’URI | 404 - RST-360011 Si è verificato un errore. Contattare l&#39;amministratore. Impossibile trovare il documento con il percorso &quot;Servizio&quot; dalla chiave &quot;adobe_nl:0&quot; (documento con schema &quot;servizio&quot; e nome &quot;adobe_nl&quot;) | 404 - Impossibile trovare il documento con il percorso &quot;Service&quot; dalla chiave &quot;adobe_nl&quot; (documento con schema &quot;service&quot; e nome &quot;adobe_nl&quot;) |
| Utilizzo di un raw-id non esistente nel corpo della richiesta | 404 - RST-360011 Si è verificato un errore. Contattare l&#39;amministratore. Impossibile trovare il documento con il percorso &quot;Servizio&quot; dalla chiave &quot;adobe_nl&quot; (documento con schema &quot;servizio&quot; e nome &quot;adobe_nl&quot;) | 404 - Impossibile trovare il documento con il percorso &quot;Service&quot; dalla chiave &quot;adobe_nl&quot; (documento con schema &quot;service&quot; e nome &quot;adobe_nl&quot;) |
| - | 500 - RST-360011 Si è verificato un errore. Contattare l&#39;amministratore. | 500 - Si è verificato un errore - contatta l’amministratore. |
| Inserisci un profilo/servizio con un valore enum di genere (o altro) non valido | 500 - RST-360011 Si è verificato un errore. Contattare l&#39;amministratore. Il valore &#39;invalid&#39; non è valido per l&#39;enumerazione &#39;nms:recipient:gender&#39; del campo &#39;@gender&#39; | 500 - Si è verificato un errore. Contattare l&#39;amministratore. |

### Fuso orario del profilo e ccpaOptOut {#profile-timezone}

Con Campaign Standard, il fuso orario viene visualizzato come parte della risposta JSON di **profileAndServices/profile** chiamate REST API.

Con Campaign v8, il fuso orario viene visualizzato all’utente solo come parte delle chiamate REST API **profileAndServicesExt/profile**. Non fa parte delle chiamate REST API di **profileAndServices/profile** poiché è in fase di aggiunta in uno schema esteso.

Lo stesso vale per il campo `ccpaOptOut`: viene visualizzato solo come parte delle chiamate REST API **profileAndServicesExt/profile**, non delle chiamate REST **profileAndServices/profile**, poiché viene aggiunto in uno schema esteso come parte della migrazione dei dati.

### Segnali esterni del flusso di lavoro {#workflow-signals}

L’API GET di Campaign Standard Workflow restituisce i nomi dei parametri, come le variabili dell’istanza del flusso di lavoro e i relativi tipi di dati (booleano, stringa, ecc.). Viene utilizzato per creare un corpo di richiesta JSON formattato in modo appropriato quando si attiva il segnale tramite una chiamata API POST.

Campaign v8 non supporta le variabili dell’istanza del flusso di lavoro per la pubblicità, ma si aspetta che gli sviluppatori sappiano di cosa si tratta. Di conseguenza, dopo la migrazione, le informazioni sui parametri nel corpo della richiesta POST dovranno essere costruite senza la disponibilità di informazioni sui parametri nella risposta API GET.
