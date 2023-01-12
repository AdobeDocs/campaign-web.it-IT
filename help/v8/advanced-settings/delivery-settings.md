---
audience: end-user
title: Impostazioni di consegna e-mail
description: Documentazione Web di Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: ed814fbb9d3f9daeb725f44a7a1929217d1d48d2
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 14%

---

# Impostazioni di consegna e-mail {#email-del-settings}

![](../assets/do-not-localize/badge.png)

Queste impostazioni sono **parametri tecnici di consegna** definiti nel modello e-mail.

## Impostazioni di consegna e-mail {#email-delivery-settings}

>[!CAUTION]
>
> Queste impostazioni sono descritte solo a scopo informativo. Alcune dipendono dalla configurazione e dalle autorizzazioni. Non devono essere modificati in questa versione del prodotto.

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="La tipologia ti consente di controllare, filtrare e monitorare l’invio di consegne."

Le tipologie sono insiemi di **regole di tipologia** che vengono eseguite durante la fase di analisi dei messaggi. Consentono di assicurarsi che le e-mail contengano sempre alcuni elementi, come un collegamento per l’annullamento dell’abbonamento o una riga dell’oggetto oppure regole di filtro per escludere i gruppi dal target previsto, ad esempio utenti non abbonati, concorrenti o clienti non fidelizzati.

Quando si associa una tipologia a un messaggio o a un modello di messaggio, le regole di tipologia incluse nella tipologia vengono eseguite per verificare la validità del messaggio durante la preparazione dei messaggi.

![](assets/delivery-settings-1.png)


### Parametri di pressione {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso consegna"
>abstract="I pesi di distribuzione consentono di identificare le consegne prioritarie nel quadro della gestione della pressione. I messaggi con il peso maggiore hanno priorità."

In questa sezione, i parametri di pressione consentono di definire un **soglia**. È il numero massimo di messaggi che possono essere inviati a un profilo in un dato periodo di tempo. Una volta raggiunta tale soglia, non potranno più essere effettuate ulteriori consegne fino alla fine del periodo considerato. Questo processo ti consente di escludere automaticamente un profilo da una consegna se un messaggio supera la soglia impostata, evitando in tal modo una sollecitazione eccessiva.

I valori di soglia possono essere costanti o variabili. Ciò significa che per un dato periodo le soglie possono variare da un profilo all’altro, o anche per lo stesso profilo.

In **Tipo di peso** sono disponibili tre opzioni:

* **Costante**
* **Dipende dal destinatario**
* **Definito in ciascuna regola**

Utilizza la **Peso della consegna** per definire la priorità di consegna. Ogni consegna ha un peso che rappresenta il suo livello di priorità. Per impostazione predefinita, il peso di una consegna è impostato su 5. Le regole di pressione ti consentono di definire il peso delle consegne a cui verranno applicate.I pesi possono essere impostati o calcolati tramite una formula adatta ai destinatari. Ad esempio, puoi definire il peso di una consegna in base agli interessi dei destinatari.


Utilizza la **Modalità di consegna** per selezionare la modalità di valutazione target. Sono disponibili tre modalità:

* **Stima target e personalizzazione messaggio**
* **Stima e approvazione del target provvisorio**
* **Valutazione del target**

La gestione dell’affaticamento viene fornita con **Ottimizzazione di Campaign** add-on. Ulteriori informazioni sulle regole di pressione e su come configurare la gestione dell’affaticamento in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=it){target="_blank"}.

### Impostazioni capacità {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importanza del destinatario"
>abstract="L’importanza del destinatario è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità."

In questa sezione puoi selezionare una regola di capacità definita nella console Adobe Campaign v8. Questa regola è associata al canale e-mail.

La **importanza del destinatario** field è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità.

Ulteriori informazioni sulle regole di coerenza e capacità e su come configurarle in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Pubblico {#audience}

In questa sezione puoi selezionare una **mappatura target** tra quelli disponibili. Le mappature di destinazione sono definite nella console Adobe Campaign v8.

Ulteriori informazioni sulle mappature target in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Consegna {#delivery}

I parametri di consegna sono impostazioni tecniche applicabili alla consegna.

* **Indirizzamento**: l’account esterno di indirizzamento e-mail integrato è fornito per impostazione predefinita. Contiene i parametri tecnici che consentono all’applicazione di effettuare l’invio di e-mail.

* **Test della consegna SMTP**: questa opzione viene utilizzata per testare l’invio tramite SMTP. La consegna viene elaborata fino alla connessione al server SMTP, ma non viene inviata: per ogni destinatario della consegna, Campaign si connette al server del provider SMTP, esegue il comando SMTP RCPT TO e chiude la connessione prima del comando SMTP DATA.

* **Ccn e-mail**: questa opzione viene utilizzata per memorizzare le e-mail su un sistema esterno tramite CCN semplicemente aggiungendo un indirizzo e-mail CCN al target del messaggio. Ulteriori informazioni su CCN e-mail in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Nuovi tentativi {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Numero massimo di nuovi tentativi"
>abstract="Se un messaggio non riesce a causa di un errore temporaneo, verranno eseguiti nuovi tentativi per tutta la durata della consegna."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Ulteriori informazioni sulla gestione dei tentativi in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Attività Approval {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modalità di approvazione"
>abstract="Ogni fase di una consegna può essere soggetta ad approvazione per garantire il pieno monitoraggio e controllo dei vari processi."

Se durante la preparazione della consegna vengono generati avvisi, puoi configurare la consegna per definire se eseguire o meno la consegna. Per impostazione predefinita, l’utente deve confermare l’invio di messaggi al termine della fase di analisi: questo è **manuale** convalida.

Puoi selezionare un’altra modalità di approvazione nel campo appropriato. Le modalità disponibili sono:

* **Manuale**: Al termine della fase di analisi, l’utente deve confermare la consegna per iniziare l’invio.

* **Semiautomatico**: L’invio inizia automaticamente se la fase di analisi non genera messaggi di avviso.

* **Automatico**: L’invio inizia automaticamente al termine della fase di analisi, indipendentemente dal risultato.


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

![](assets/delivery-settings-2.png)


Ulteriori informazioni sul periodo di validità della consegna in [Documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Gestione di pagine mirror {#mirror}

La pagina speculare è una pagina HTML accessibile online tramite un browser web. Il contenuto è identico all’e-mail. Per impostazione predefinita, la pagina speculare viene generata se il collegamento viene inserito nel contenuto della posta.

Oltre alla modalità predefinita, sono disponibili anche le seguenti opzioni:

* **[!UICONTROL Forza la generazione della pagina speculare]**: anche se nella consegna non viene inserito alcun collegamento alla pagina speculare, verrà creata la pagina speculare.
* **[!UICONTROL Non generare la pagina speculare]**: non viene generata alcuna pagina speculare, anche se il collegamento è presente nella consegna.
* **[!UICONTROL Genera una pagina speculare accessibile utilizzando solo l’identificatore del messaggio]**: questa opzione ti consente di accedere al contenuto della pagina speculare, con informazioni sulla personalizzazione, nella finestra del registro di consegna. A questo scopo, dopo la fine della consegna, fai clic sul pulsante **[!UICONTROL Consegna]** e selezionare la riga del destinatario di cui si desidera visualizzare la pagina speculare. Fai clic sul pulsante **[!UICONTROL Visualizza la pagina speculare del messaggio...]** link.


### Tracciamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Periodo di validità"
>abstract="Questa opzione definisce la durata per la quale verrà attivato il tracciamento sugli URL."

I parametri di tracciamento sono definiti nella sezione correlata. Le opzioni possibili sono:

**Limite di validità del tracciamento**: utilizza questa opzione per modificare la durata per la quale verrà attivato il tracciamento sugli URL.

**URL di sostituzione per gli URL scaduti**: utilizza questa opzione per immettere un URL per una pagina web di fallback: viene visualizzato una volta scaduto il tracciamento.

## Impostazioni di test {#test-setttings}

Puoi impostare i parametri di esclusione in questa sezione. Le opzioni disponibili sono:

* **Mantieni doppio** ti consente di autorizzare più consegne a destinatari che soddisfano più criteri di targeting.

* **Mantieni indirizzi inserita nell&#39;elenco Bloccati** consente di mantenere dal target qualsiasi profilo non più oggetto di targeting dalla consegna, ad esempio dopo un annullamento dell’abbonamento (opt-out).

* **Mantieni indirizzi in quarantena** ti consente di mantenere dal target qualsiasi profilo con un indirizzo che non risponde.

Puoi anche personalizzare il nome delle bozze.

Utilizza la **Mantieni il codice di consegna per la bozza** associare alla bozza lo stesso codice di consegna definito per la consegna a cui si riferisce.

Per impostazione predefinita, l’oggetto della prova è preceduto da &quot;PROOF #&quot;, dove # è il numero della prova. Puoi modificare questo prefisso nella **Prefisso etichetta** campo .