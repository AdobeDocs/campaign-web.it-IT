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
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 2%
---
# Differenze tra Campaign Standard e Campaign v8 {#acs-v8-differences}

La maggior parte dei concetti sono gli stessi in Campaign Standard e Campaign v8. Questa pagina raccoglie le differenze che ti interessano dopo la transizione e contiene i collegamenti alla pagina che spiega ciascuna. Completa le guide per [addetti al marketing](marketers.md) e per [amministratori e sviluppatori](admin-developers.md).

* Per le modifiche terminologiche, vedi [Differenze chiave tra Campaign Standard e Campaign v8](overview.md#experiences).
* Per i controlli da eseguire e i problemi segnalati dopo una transizione, vedere [Controlli e risoluzione dei problemi dopo la transizione](post-transition-checks.md).
* Per le funzionalità disponibili solo nella console client, vedere [Console client Campaign Web e Campaign](../../v8/get-started/capability-matrix.md).

## Canali e contenuti {#channels}

I passaggi per creare e inviare messaggi sono simili in entrambi i prodotti, come descritto nella [guida per gli addetti al marketing](marketers.md). Le differenze seguenti riguardano la disponibilità dei canali, le consegne di test, le pagine di destinazione e i flussi di lavoro di direct mailing.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| Il canale in-app non è disponibile in Campaign v8. | [Canale in-app](marketers.md#acs-gs-marketers-in-app) |
| Per eseguire la transizione dei flussi di lavoro e delle consegne push esistenti, contatta il tuo Adobe Campaign Transition Manager. | [Notifiche push](marketers.md#acs-gs-marketers-push) |
| In Campaign Standard, un profilo di test potrebbe essere contrassegnato come **Abbondanza** per ricevere l&#39;invio finale. In Campaign v8, abilita l’opzione per includere i profili di test nel pubblico principale della consegna. | [Consegne di prova](../../v8/preview-test/test-deliveries.md) |
| Le pagine di destinazione create nell’interfaccia utente di Campaign Web non supportano campi di input nascosti o JavaScript personalizzato. | [Pagine di destinazione](../../v8/landing-pages/get-started-lp.md) |
| In Campaign Standard, anche la transizione in uscita di un’attività di direct mailing trasportava il file generato. In Campaign v8, porta solo la popolazione target. Per inviare il file a un server, aggiungi un&#39;attività **Estrazione dati**, quindi un&#39;attività **Trasferimento file**. | [Direct mail](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Tipi di pubblico, flussi di lavoro e consegne {#data-and-workflows}

Queste differenze interessano i tipi di pubblico e i flussi di lavoro migrati da Campaign Standard, alcune opzioni di consegne ricorrenti e dell&#39;attività **Trasferimento file** e l&#39;ambito del reporting dinamico.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| I tipi di pubblico vengono trasformati durante la transizione. Ad esempio, i tipi di pubblico creati con l’attività Query diventano filtri predefiniti, mentre i tipi di pubblico di tipo file diventano tipi di pubblico di tipo Elenco senza dimensioni. | [Gestione tipi di pubblico](marketers.md#acs-gs-marketers-audiences) |
| I registri cronologici dei flussi di lavoro eseguiti in Campaign Standard non vengono migrati. | [Creare un flusso di lavoro](marketers.md#acs-gs-marketers-wf) |
| In Campaign Standard, puoi selezionare il periodo di aggregazione di un’e-mail ricorrente. Questa opzione non è disponibile in Campaign v8. | [Attività del canale](../../v8/workflows/activities/channels.md) |
| In Campaign Standard, l&#39;attività **Trasferimento file** potrebbe ordinare i file in modo alfanumerico. Questa opzione non è disponibile in Campaign v8. | [Trasferisci file](../../v8/workflows/activities/transfer-file.md) |
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

## Amministrazione, tracciamento e pagine mirror {#admin-tracking}

Queste differenze influiscono sulle consegne inviate da Campaign Standard prima della transizione e sulle informazioni amministrative che non vengono riportate in Campaign v8.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| Non sono disponibili pagine mirror delle consegne inviate da Campaign Standard prima della transizione. Le pagine mirror delle consegne inviate da Campaign v8 funzionano normalmente. | [Pagine mirror](../../v8/email/mirror-page.md) |
| I dati di tracciamento delle consegne transazionali in tempo reale inviate da Campaign Standard prima della transizione non vengono acquisiti in Campaign v8. I collegamenti di questi messaggi continuano a essere reindirizzati. | [Monitorare i messaggi transazionali](../../v8/transactional-messaging/monitor-transactional.md) |
| Le impostazioni URL tracciate delle bozze di consegna non vengono mantenute. Dopo la transizione, i collegamenti di tracciamento, di pagina speculare e di abbonamento seguono lo standard Campaign v8 e i collegamenti sono tracciati per impostazione predefinita. | [Aggiungere collegamenti e tenere traccia dei messaggi](../../v8/email/message-tracking.md) |
| Unità geografiche non disponibili. Il controllo degli accessi in base alle unità geografiche viene perso. | [Controllo dell&#39;accesso](../../v8/get-started/connect-to-campaign.md#access-control) |
| Le informazioni delle entità **Creato da** e **Modificato da** non sono disponibili dopo la transizione. | [Audit trail](admin-developers.md#acs-gs-admin-audit-trail) |
| Gli URL dei sottodomini di branding vengono adeguati allo standard Campaign v8. Le configurazioni di branding non standard non vengono migrate e vengono servite tramite il brand predefinito. | [Marchio](../../v8/administration/branding/branding-gs.md) |

## API e integrazioni {#apis-and-integrations}

Queste differenze influiscono sulle integrazioni che chiamano Campaign tramite l’API REST e sulle integrazioni con altre soluzioni e strumenti di Adobe.

| Cosa cambia | Ulteriori informazioni |
|---|---|
| I valori PKEY cambiano dopo la migrazione. Se memorizzi le PKEY al di fuori di Campaign, segui invece gli href restituiti dall’API. | [API REST](admin-developers.md#acs-gs-admin-apis) |
| Alcuni campi del profilo migrati, come fuso orario e `ccpaOptOut`, vengono restituiti solo dall&#39;API `profileAndServicesExt/profile`. | [API REST](admin-developers.md#acs-gs-admin-apis) |
| Le integrazioni Dreamweaver e Connettore dati Adobe Experience Platform di Campaign Standard non sono disponibili in Campaign v8. | [Utilizzare Campaign e altre soluzioni Adobe](../../v8/integrations/integration.md) |
| Adobe esegue la migrazione delle configurazioni di Adobe Analytics e Audience Manager. Devi configurare nuovamente le integrazioni Triggers e Adobe Target. | [Gestione integrazioni Adobe Campaign](admin-developers.md#acs-gs-integrations) |
