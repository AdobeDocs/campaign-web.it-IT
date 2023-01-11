---
audience: end-user
title: Impostazioni avanzate
description: Documentazione Web di Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 22%

---

# Impostazioni avanzate {#advanced-settings}

![](../assets/do-not-localize/badge.png)

Queste impostazioni sono **parametri tecnici di consegna** definiti nel modello e-mail. Se desideri modificarli per una consegna specifica, procedi con cautela.

## Impostazioni di consegna e-mail {#email-delivery-settings}

>[!NOTE]
>
> Modifica solo le impostazioni, nessuna nuova creazione consentita. Soggetto ai diritti di accesso.

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="La tipologia ti consente di controllare, filtrare e monitorare l’invio di consegne."

Le tipologie sono insiemi di **regole di tipologia** che vengono eseguite durante la fase di analisi dei messaggi. Consentono di assicurarsi che le e-mail contengano sempre alcuni elementi, come un collegamento per l’annullamento dell’abbonamento o una riga dell’oggetto oppure regole di filtro per escludere i gruppi dal target previsto, ad esempio utenti non abbonati, concorrenti o clienti non fidelizzati.

Durante l’associazione di una tipologia a un messaggio o a un relativo modello, le regole di tipologia incluse in essa vengono eseguite per verificare la validità del messaggio.

### Parametri di pressione {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso consegna"
>abstract="I pesi di distribuzione consentono di identificare le consegne prioritarie nel quadro della gestione della pressione. I messaggi con il peso maggiore hanno priorità."

In questa sezione, i parametri di pressione consentono di definire un **soglia**. È il numero massimo di messaggi che possono essere inviati a un profilo in un dato periodo di tempo. Una volta raggiunta tale soglia, non potranno più essere effettuate ulteriori consegne fino alla fine del periodo considerato. Questo processo ti consente di escludere automaticamente un profilo da una consegna se un messaggio supera la soglia impostata, evitando in tal modo una sollecitazione eccessiva.

I valori di soglia possono essere costanti o variabili. Ciò significa che per un dato periodo le soglie possono variare da un profilo all’altro, o anche per lo stesso profilo.

In **Tipo di peso** sono disponibili tre opzioni: (formula mancante a seconda dell&#39;opzione..)

* **Costante**
* **Dipende dal destinatario**
* **Definito in ciascuna regola**

La **Peso della consegna** campo : Ogni consegna ha un peso che rappresenta il suo livello di priorità. Per impostazione predefinita, il peso di una consegna è impostato su 5. Le regole di pressione ti consentono di definire il peso delle consegne a cui verranno applicate.I pesi possono essere impostati o calcolati tramite una formula adatta ai destinatari. Ad esempio, puoi definire il peso di una consegna in base agli interessi dei destinatari.

La **Modalità di consegna** campo. ?

* **Stima target e personalizzazione messaggio**
* **Stima e approvazione del target provvisorio**
* **Valutazione del target**

### Impostazioni capacità {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importanza del destinatario"
>abstract="L’importanza del destinatario è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità."

In questa sezione puoi selezionare una regola di capacità definita nella console Adobe Campaign v8. Questa regola è associata al canale e-mail.

La **importanza del destinatario** field è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità.

## Pubblico {#audience}

In questa sezione puoi scegliere una **mappatura target** definiti nella console Adobe Campaign v8. La creazione della mappatura di destinazione è necessaria nel caso in cui utilizzi una tabella dei destinatari diversa da quella fornita da Adobe Campaign.

## Consegna {#delivery}

**Indirizzamento** selezione: L’account esterno di indirizzamento e-mail integrato è fornito per impostazione predefinita. Contiene i parametri tecnici che consentono all’applicazione di effettuare l’invio di e-mail.

**Test della consegna SMTP**: utilizza questa opzione per testare l’invio tramite SMTP. La consegna viene elaborata fino alla connessione al server SMTP, ma non viene inviata: per ogni destinatario della consegna, Campaign si connette al server del provider SMTP, esegue il comando SMTP RCPT TO e chiude la connessione prima del comando SMTP DATA.

**Ccn e-mail**: utilizza questa opzione per memorizzare le e-mail su un sistema esterno tramite CCN semplicemente aggiungendo un indirizzo e-mail CCN al target del messaggio.

### Nuovi tentativi {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Numero massimo di nuovi tentativi"
>abstract="Se un messaggio non riesce a causa di un errore temporaneo, verranno eseguiti nuovi tentativi per tutta la durata della consegna."

I messaggi temporaneamente non consegnati a causa di un errore morbido o ignorato sono soggetti a un nuovo tentativo automatico. Per impostazione predefinita, sono pianificati cinque nuovi tentativi per il primo giorno della consegna con un intervallo minimo di un’ora suddiviso nelle 24 ore del giorno. Un nuovo tentativo al giorno viene programmato dopo e fino alla scadenza della consegna, definita nella scheda Validità .

## Attività Approval {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modalità di approvazione"
>abstract="Ogni fase di una consegna può essere soggetta ad approvazione per garantire il pieno monitoraggio e controllo dei vari processi."

**Manuale**: Al termine della fase di analisi, l’utente deve confermare la consegna per iniziare l’invio.

**Semiautomatico**: L’invio inizia automaticamente se la fase di analisi non genera messaggi di avviso.

**Automatico**: L’invio inizia automaticamente al termine della fase di analisi, indipendentemente dal risultato.


## Validità {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Durata consegna"
>abstract="Il campo Durata consegna ti consente di inserire il limite per i tentativi di consegna globali. Questo significa che Adobe Campaign invia i messaggi a partire dalla data di inizio e quindi, per i messaggi che restituiscono un errore, vengono eseguiti tentativi regolari e configurabili fino al raggiungimento del limite di validità."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite di validità delle risorse"
>abstract="Il campo Limite di validità viene utilizzato per le risorse caricate, principalmente per la pagina speculare e per le immagini. Le risorse presenti in questa pagina sono valide per un periodo di tempo limitato."


La **Durata della consegna** consente di immettere il limite per i tentativi di consegna globali. Questo significa che Adobe Campaign invia i messaggi a partire dalla data di inizio e quindi, per i messaggi che restituiscono un errore, vengono eseguiti tentativi regolari e configurabili fino al raggiungimento del limite di validità.

Puoi anche scegliere di specificare le date. A questo scopo, seleziona **Impostazione esplicita delle date di validità**. In questo caso, le date del limite di consegna e validità ti consentono anche di specificare l’ora. L’ora corrente viene utilizzata per impostazione predefinita, ma puoi modificarla direttamente nel campo di input.

**Limite di validità delle risorse** viene utilizzato per le risorse caricate, principalmente per la pagina speculare e per le immagini. Le risorse presenti in questa pagina sono valide per un periodo di tempo limitato (per risparmiare spazio su disco).

### Gestione di pagine mirror {#mirror}

**Gestione pagina speculare** contiene quattro opzioni :

* **Genera la pagina speculare se nel contenuto dell’e-mail viene visualizzato un collegamento speculare**: la pagina speculare viene generata se il collegamento viene inserito nel contenuto della posta.
* **Force the generation of the mirror page**: anche se nei messaggi non viene inserito alcun collegamento alla pagina speculare, la pagina verrà creata ugualmente.
* **Do not generate the mirror page**: non viene creata alcuna pagina speculare, anche se il collegamento è presente nei messaggi.
* **Genera una pagina speculare accessibile utilizzando solo l’identificatore del messaggio**: questa opzione ti consente di accedere al contenuto della pagina speculare, con informazioni sulla personalizzazione, nella finestra del registro di consegna.


### Tracciamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Periodo di validità"
>abstract="Questa opzione definisce la durata per la quale verrà attivato il tracciamento sugli URL."

**Limite di validità del tracciamento**: Questa opzione definisce la durata per la quale verrà attivato il tracciamento sugli URL.

**URL di sostituzione per gli URL scaduti**: utilizza questa opzione per immettere un URL per una pagina web di fallback: viene visualizzato una volta scaduto il tracciamento.


## Impostazioni di test {#test-setttings}

**Mantieni doppio** ti consente di autorizzare più consegne a destinatari che soddisfano più criteri di targeting.

**Mantieni indirizzi inserita nell&#39;elenco Bloccati** consente di mantenere dal target qualsiasi profilo non più oggetto di targeting dalla consegna, ad esempio dopo un annullamento dell’abbonamento (opt-out).

**Mantieni indirizzi in quarantena** ti consente di mantenere dal target qualsiasi profilo con un indirizzo che non risponde.

**Mantieni il codice di consegna per la bozza** ti consente di assegnare alla bozza lo stesso codice di consegna definito per la consegna a cui si riferisce.

Per impostazione predefinita, l’oggetto della bozza è preceduto da &quot;Proof #&quot;, dove # è il numero della bozza. Puoi modificare questo prefisso nella **Prefisso etichetta** campo .