---
title: Migrazione degli utenti tecnici alla console Adobe Developer
description: Scopri come migrare la gestione degli accessi utente da Campaign Standard a Campaign v8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '1403'
ht-degree: 2%

---

# Gestione degli accessi utente da Campaign Standard a Campaign v8 {#user-management-acs}

Sia Adobe Campaign Standard che Adobe Campaign v8 consentono agli utenti di definire e gestire le autorizzazioni per diversi utenti/operatori. Queste autorizzazioni sono costituite da diritti specifici che consentono agli utenti di accedere a varie funzioni del prodotto. Tuttavia, i due prodotti utilizzano approcci e implementazioni distinti per la gestione dell’accesso degli utenti.

Per ottenere la gestione degli accessi utente in Adobe Campaign Standard e Campaign v8 vengono utilizzati i seguenti concetti:

| Campaign Standard | Campaign v8 |
|---------|----------|
| Utente | Operatore |
| Ruolo | Denominato a destra |
| Gruppo di sicurezza | Gruppo di operatori |
| Unità organizzativa | Autorizzazione cartella |

## Approccio alla migrazione dal gruppo Sicurezza al gruppo Operatori

>[!IMPORTANT]
>
>Le funzionalità di questi ruoli/diritti denominati possono variare nell’implementazione, causando potenzialmente problemi di autorizzazione (ad esempio, elevazione dei privilegi o interruzioni di funzionalità). Consigliamo agli utenti di rivedere queste mappature dopo la transizione per garantire un corretto controllo degli accessi. [Ulteriori informazioni sulle autorizzazioni](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

La tabella seguente illustra l’approccio di migrazione per i gruppi di ruoli utente durante la transizione da Adobe Campaign Standard a Campaign v8. In Campaign Standard, viene utilizzato un **gruppo di sicurezza**, denominato **gruppo di operatori** in Campaign v8, per assegnare un set di ruoli a un utente. Anche se alcuni gruppi di sicurezza/gruppi di operatori sono predefiniti, gli utenti possono creare nuovi gruppi o modificarne di esistenti, se necessario.

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologia**  | Gruppo di sicurezza | Gruppo di operatori |

Sia in Adobe Campaign Standard che in Campaign v8, **I gruppi di sicurezza** e **I gruppi di operatori** sono mappati ai profili di prodotto in Admin Console. Se desideri assegnare un **gruppo di sicurezza** o un **gruppo di operatori** a un utente, puoi collegare il **profilo di prodotto** corrispondente in Admin Console. Questa associazione viene sincronizzata al momento dell’accesso dell’utente. [Ulteriori informazioni sul profilo di prodotto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Gruppo di sicurezza Campaign Standard** | **Gruppo di operatori di Campaign v8** |
|----------|---------|
| Amministratori | Amministratori |
| Supervisori della consegna | Amministratori |
| Supervisori del workflow | Supervisori del workflow  |

## Approccio di migrazione da ruoli utente a diritti denominati

>[!IMPORTANT]
>
>Durante la migrazione da Adobe Campaign Standard a Campaign v8, gli utenti con il ruolo **Modello dati** ma non **Amministrazione** otterranno automaticamente l&#39;accesso **Amministrazione**, in quanto la creazione dello schema in Campaign v8 richiede diritti di amministrazione. Per evitare questo problema, rimuovi il ruolo **Modello dati** prima della migrazione.

In Adobe Campaign Standard, il termine **Ruolo utente** è indicato come **Diritto denominato** in Campaign v8. La tabella seguente illustra la terminologia utilizzata per **Diritti denominati** in Campaign v8 corrispondenti a **Ruoli utente** in Campaign Standard.

| **Ruolo utente Campaign Standard** | **Campaign v8 denominato a destra** | **Descrizione**  |
|----------|---------|---------|
| Amministrazione | Amministrazione | L’utente con i permessi di amministratore ha accesso completo all’istanza. |
| Modello dati  | Amministrazione | Diritto di eseguire pubblicazioni e creare risorse personalizzate. Funzionalità correlate alla creazione di schemi disponibili per l’amministratore in Campaign v8.  |
| Recapito messaggi  | Amministrazione  | Diritto di approvare le consegne analizzate in precedenza.  |
| Esporta | Esporta | Diritto di esportare i dati.  |
| Accesso ai file  | Accesso ai file  | Diritto di approvare le consegne analizzate in precedenza.  |
| Importazione generica  | Importa  | Diritto per l’importazione di dati generici |
| Preparare le consegne | Preparare le consegne | Diritto di creare, modificare, preparare ed eliminare consegne.  |
| Esecuzione script SQL | Esecuzione script SQL | Diritto di eseguire qualsiasi comando SQL direttamente sul database. |
| Avviare le consegne  | Avviare le consegne  | Diritto di approvare le consegne analizzate in precedenza.  |
| Esecuzione comando di sistema | Esecuzione del programma | Diritto di eseguire comandi di sistema sul server. |
| Flusso di lavoro | Flusso di lavoro | Diritto di gestire l’esecuzione dei flussi di lavoro di avvio, arresto, pausa, ecc. |

## Approccio alla migrazione dall’unità organizzativa

>[!IMPORTANT]
>
>Le unità organizzative in Adobe Campaign Standard senza **All (all)** come padre diretto o indiretto non verranno migrate a Campaign v8.
></br>
>Agli utenti di più gruppi di sicurezza viene assegnata l’unità organizzativa del gruppo di sicurezza di livello più alto. Se più gruppi dispongono di unità parallele di primo livello, il sistema seleziona l’unità organizzativa per l’utente in Campaign Standard e l’utente avrà accesso solo all’unità organizzativa selezionata dal sistema e ai relativi elementi secondari. In Campaign v8 dopo la migrazione, l&#39;utente avrebbe accesso a **tutte le unità organizzative assegnate e ai relativi elementi secondari**, aumentando potenzialmente i privilegi. Per evitare questo problema, evita di assegnare gli utenti a gruppi di sicurezza con unità organizzative parallele. Ulteriori informazioni sull&#39;assegnazione di [unità organizzativa parallela](#parallel-assignments).


In Adobe Campaign Standard, l&#39;**unità organizzativa** è mappata al modello gerarchico **Cartella** esistente in Campaign v8 per mantenere un controllo degli accessi simile. [Ulteriori informazioni sulla gestione delle cartelle](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologia**  | Unità organizzativa | Cartella |


### Informazioni sull’assegnazione di unità organizzative parallele {#parallel-assignments}

L’assegnazione di un’unità organizzativa parallela si verifica quando un utente ha accesso a più unità (assegnate tramite gruppi di sicurezza) che esistono in rami separati della gerarchia senza avere accesso a un’unità organizzativa principale comune. Questo crea un rischio per la sicurezza durante la migrazione.

Ad esempio, considera la seguente gerarchia di unità organizzative:

![Diagramma di esempio assegnazione unità organizzativa parallela](assets/do-not-localize/parallel-org-units-sample.png){width="50%" zoomable="yes"}

Un’assegnazione senza unità organizzative parallele sarà simile alla seguente:

![Senza diagramma di esempio dell&#39;unità organizzativa parallela](assets/do-not-localize/without-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

In questo caso, l’utente ha accesso alle unità organizzative A, A1 e A2-1, tutte collegate sotto l’unità organizzativa principale A. L’utente può accedere a tutto ciò che si trova in A.

La seguente assegnazione contiene unità organizzative parallele:

![Con diagramma di esempio dell&#39;unità organizzativa parallela](assets/do-not-localize/with-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

L’utente ha accesso a A1-1, A2 e A2-1, che esistono in rami separati senza alcun elemento principale assegnato in comune.


**Implicazioni sulla sicurezza**

* In Campaign Standard, il sistema seleziona un’unità organizzativa di livello superiore (A1-1 o A2) per l’utente, limitando l’accesso solo a tale unità e ai relativi elementi secondari.
* Dopo la migrazione a Campaign V8, l’utente ottiene l’accesso alle risorse in tutte le unità organizzative assegnate e nei relativi elementi secondari.

**Risoluzione**

L’assegnazione di un’unità organizzativa parallela può essere risolta facendo in modo che tutte le unità organizzative assegnate a un utente rientrino in un’unica unità principale comune, anch’essa assegnata all’utente.

Di seguito sono indicati alcuni modi per raggiungere questo obiettivo:

1. Rimuovere l’accesso a più rami: revoca l’accesso a più rami paralleli e assicurati che tutto l’accesso avvenga sotto un singolo elemento principale.
1. Assegna un elemento padre comune: consente di concedere l’accesso a un’unità organizzativa padre comune appropriata che includa tutti i punti di accesso necessari.
1. Ristrutturare la gerarchia: modificare la struttura dell’unità organizzativa in modo da collocare tutto l’accesso necessario sotto un singolo ramo.

Nell’esempio precedente, in cui un utente ha accesso ad A1-1, A2 e A2-1, i passaggi per le risoluzioni specifiche sono:

1. Rimuovi l’accesso a più rami:

   1. Revocare l&#39;accesso a A1-1, lasciando solo l&#39;accesso a A2 (che include A2-1), oppure
   1. Revoca dell&#39;accesso a A2 e A2-1, lasciando solo l&#39;accesso a A1-1

1. Assegna un elemento padre comune:

   1. Concedere l’accesso all’unità organizzativa A, che è l’elemento padre comune sia di A1-1 che di A2, oppure
   1. Concedi l’accesso a Tutti, che copre l’intera gerarchia

1. Ristrutturare la gerarchia:

   1. Spostare A1-1 sotto A2, oppure
   1. Spostare A2 e A2-1 sotto A1-1


## Approccio alla migrazione dal programma

In Campaign v8, **I programmi** sono rappresentati come **Cartelle**. Campaign v8 consente di creare cartelle e di limitarne l’accesso.

Utilizzando **Gruppi** e **Diritti denominati**, è possibile concedere a **Operatori** l&#39;accesso a **Cartelle** specifiche all&#39;interno della gerarchia di navigazione, con la possibilità di assegnare autorizzazioni di lettura, scrittura ed eliminazione. [Ulteriori informazioni sulla gestione delle cartelle](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Poiché un **Programma** è trattato come una **Cartella** in Campaign v8, il suo accesso può essere gestito nello stesso modo di qualsiasi altra cartella. Dopo la migrazione, gli amministratori di Campaign Standard possono seguire questi passaggi:

1. In Esplora, fare clic con il pulsante destro del mouse su una cartella e selezionare **[!UICONTROL Proprietà...]**.

1. Passare alla scheda **[!UICONTROL Protezione]**.

1. Modifica le autorizzazioni del gruppo di operatori in base al modello di accesso desiderato. 

## Mappatura del profilo di prodotto per accedere alle API REST 

Per accedere alle API transazionali dall&#39;istanza di esecuzione in Campaign v8, è necessario un nuovo **profilo di prodotto**, oltre ai profili di prodotto **Amministratore** e **Centro messaggi**. Il nuovo **profilo di prodotto** verrà aggiunto agli account tecnici esistenti o precreati in Campaign Standard.

Dopo la migrazione, gli utenti di Campaign Standard devono rivedere le **mappature del profilo di prodotto** e assegnare il **profilo di prodotto** appropriato se non desiderano collegare i loro **account tecnici** al profilo di prodotto **Amministratore**. Per le integrazioni future, è consigliabile utilizzare l&#39;ID tenant **di Campaign v8 nell&#39;** URL REST **anziché l&#39;ID tenant** di Campaign Standard precedente.****

## Migrazione dell’accesso alle risorse integrate di Campaign per gli operatori Campaign Standard

Gli operatori migrati da Campaign Standard avranno accesso in lettura a specifiche risorse integrate in Campaign v8.

## Ruoli e gruppi di sicurezza non migrati {#non-migrated-groups-roles}

Di seguito è riportato un elenco dei ruoli di Campaign Standard per i quali non è stata eseguita la transizione:

* Account inoltro predefinito 

* Push del Centro messaggi 

Di seguito è riportato un elenco delle mappature dei gruppi di sicurezza di Campaign Standard per le quali non è stata eseguita la transizione.

* Agenti del Centro messaggi

* Agenti push del centro messaggi

* Application manager Adobe Experience Manager

* Account Relay

>[!NOTE]
>
>I ruoli personalizzati creati e assegnati agli utenti in Adobe Campaign Standard non verranno migrati ad Adobe Campaign v8.
