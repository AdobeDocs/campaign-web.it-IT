---
title: Controlli e risoluzione dei problemi dopo la transizione a Campaign v8
description: Scopri cosa controllare e come risolvere i problemi comuni dopo la transizione da Campaign Standard a Campaign v8
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%
---
# Controlli e risoluzione dei problemi dopo la transizione {#post-transition-checks}

Dopo la transizione da Campaign Standard a Campaign v8, alcune consegne, flussi di lavoro e pagine di destinazione potrebbero comportarsi in modo diverso rispetto alle aspettative. La tabella seguente elenca i sintomi segnalati dagli utenti con transizione, con la causa e le azioni da intraprendere. Per l&#39;elenco completo delle differenze, vedere [Differenze tra Campaign Standard e Campaign v8](acs-v8-differences.md).

| Sintomo | Causa e cosa fare | Ulteriori informazioni |
|---|---|---|
| I collegamenti in una consegna sono URL diretti e non vengono raccolti dati di clic. | Il tracciamento è disabilitato nella consegna o nel modello di consegna su cui si basa. Controlla che **Attiva il tracciamento** sia abilitato, in particolare sui modelli delle consegne ricorrenti. | [Impostazioni di tracciamento](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| I destinatari che hanno annullato l’abbonamento tramite il metodo &quot;mailto&quot; List-Unsubscribe non sono in quarantena. | Questo è previsto. Questi destinatari non vengono messi in quarantena. L’abbonamento al servizio associato alla consegna viene annullato oppure viene aggiunto al inserisco nell&#39;elenco Bloccati di consegna dell’se la consegna non prevede alcun servizio. Per tenere traccia di questi annullamenti di abbonamenti, controlla gli abbonamenti del servizio o la sezione **Non contattare più** del profilo. | [Quarantene](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Una pagina di destinazione non salva un valore calcolato da uno script o memorizzato in un campo nascosto. | Le pagine di destinazione create nell’interfaccia utente di Campaign Web non supportano campi di input nascosti o JavaScript personalizzato. Crea il modulo come applicazione web nella console client. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
| **Il trasferimento di file** non trova il file generato da un&#39;attività di direct mailing. | La transizione in uscita di un’attività di direct mailing porta la popolazione target, non il file di estrazione. Aggiungi un&#39;attività **Estrazione dati**, quindi l&#39;attività **Trasferimento file**. | [Direct mail](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Varie ondate di una consegna vengono inviate insieme. | Gli scaglioni sono pianificati dalla data di contatto della consegna. Se la consegna inizia dopo il tempo pianificato di alcune ondate, queste ultime vengono inviate insieme invece di essere distanziate. | [Invia con scaglioni](../../v8/advanced-settings/send-using-waves.md) |
| Una maschera di file con caratteri dopo l’asterisco non trova alcun file nell’archiviazione BLOB di Azure. | L’archiviazione BLOB di Azure filtra i file in base al prefisso del nome. È supportato solo un asterisco finale. | [Trasferisci account esterno](../../v8/administration/transfer-external-account.md) |
| Una pagina di destinazione o un blocco di contenuto che utilizza JavaScript personalizzato si comporta in modo diverso. | JavaScript personalizzato viene trasformato durante la migrazione, ma convalidato e regolato, in particolare se utilizza `queryDef`, API di Campaign JavaScript, scritture di sessioni, gestione di unità organizzative o generazione di URL personalizzati. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
| Una chiamata API REST restituisce un valore vuoto, un errore o una risposta imprevista. | Alcuni campi del database vengono eliminati durante la migrazione e restituiscono valori vuoti. Un PATCH vuoto restituisce 204 e un PATCH sulla posizione restituisce 500. Un POST con una risorsa collegata ignora il collegamento o restituisce un errore. PKEY non valido restituisce 404. | [Limitazioni REST API](acs-v8-differences.md#rest-api-limitations) |
| Una PKEY memorizzata non funziona più nelle chiamate API. | I valori PKEY cambiano dopo la migrazione. Non conservarli al di fuori di Campaign. Da ogni chiamata dagli href restituiti dalla chiamata precedente. | [Utilizzo chiave](acs-v8-differences.md#key-usage) |
| Fuso orario o `ccpaOptOut` mancante in una risposta del profilo. | Questi campi vengono restituiti solo da `profileAndServicesExt/profile`, non da `profileAndServices/profile`. Chiama l&#39;endpoint esteso. | [Fuso orario profilo e ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| Un filtro personalizzato restituisce un errore in una chiamata API REST. | In Campaign v8, assegna al filtro un nome nel campo **Nome filtro in API REST** e utilizza questo nome così come è nella richiesta, senza il prefisso &quot;by&quot;. | [Filtro](acs-v8-differences.md#rest-filtering) |
| Una chiamata che attiva un segnale esterno di flusso di lavoro non può creare il corpo della richiesta. | L’API GET del flusso di lavoro non restituisce più le variabili del flusso di lavoro. Crea i parametri del corpo della richiesta POST in base alla tua conoscenza del flusso di lavoro. | [Segnali esterni flusso di lavoro](acs-v8-differences.md#workflow-signals) |
| Accesso negato alle API transazionali. | L’accesso alle API transazionali dall’istanza di esecuzione richiede un nuovo profilo di prodotto. Esamina la mappatura del profilo di prodotto degli account tecnici. | [Mappatura profilo prodotto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Un pubblico migrato mostra solo il valore più recente, oppure un pubblico di tipo file non ha dimensioni. | Questo è previsto. Un filtro predefinito accetta solo il valore più recente dopo la migrazione del pubblico e i tipi di pubblico di tipo file diventano tipi di pubblico di tipo Elenco senza dimensioni. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| La cronologia dei flussi di lavoro eseguiti in Campaign Standard è vuota. | I registri cronologici dei flussi di lavoro eseguiti in Campaign Standard non vengono migrati. I flussi di lavoro eseguiti in Campaign v8 hanno una propria cronologia e registri. | [Creare un flusso di lavoro](marketers.md#acs-gs-marketers-wf) |
| Alcuni utenti possono visualizzare o eseguire più operazioni di prima. | Gli utenti con il ruolo **Modello dati** ma non con il ruolo **Amministrazione** ottengono l&#39;accesso **Amministrazione** e i gruppi di sicurezza con unità organizzative parallele possono avere un accesso più ampio. Esamina i gruppi di operatori, i diritti denominati e le autorizzazioni della cartella. | [Gestione degli accessi utente](user-management-acs.md) |
| Un profilo di test contrassegnato come **Trap** non riceve l&#39;invio finale. | In Campaign v8, aggiungi un **gruppo di trap** nelle impostazioni Pubblico della consegna. | [Gruppo di trap](../../v8/audience/trap-group.md) |
| Un’e-mail ricorrente non dispone di un’opzione di periodo di aggregazione. | Questa opzione non è disponibile in Campaign v8. | [Attività del canale](../../v8/workflows/activities/channels.md) |
| Il reporting dinamico non mostra dati per una consegna. | Il reporting dinamico riguarda le consegne di e-mail, le campagne con le consegne di e-mail e i messaggi transazionali. | [Reportistica](marketers.md#acs-gs-marketers-reporting) |
