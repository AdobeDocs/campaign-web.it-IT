---
audience: end-user
title: Impostazioni avanzate
description: Documentazione Web di Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 4fbb5e2eb0211712d17f1437986038c40ed15602
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 24%

---

# Impostazioni avanzate {#advanced-settings}

>[!NOTE]
>
>Questa documentazione è in fase di costruzione e viene aggiornata frequentemente. La versione finale di questo contenuto sarà pronta a gennaio 2023.

Queste impostazioni sono parametri di consegna tecnici definiti nel modello e-mail. Se desideri modificarli per una consegna specifica, procedi con cautela.

## Impostazioni di consegna e-mail {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Tutti i parametri di consegna tecnici dal modello.
Cambia solo i parametri, nessuna creazione qui.
In base alle autorizzazioni, i professionisti non devono modificare questo, cautela. Controlla e cambia solo la regola di tipologia -> resto definito nel modello

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="La tipologia ti consente di controllare, filtrare e monitorare l’invio di consegne."

Le tipologie sono insiemi di regole di tipologia che vengono eseguite durante la fase di analisi dei messaggi. Consentono di assicurarsi che le e-mail contengano sempre alcuni elementi, come un collegamento per l’annullamento dell’abbonamento o una riga dell’oggetto oppure regole di filtro per escludere i gruppi dal target previsto, ad esempio utenti non abbonati, concorrenti o clienti non fidelizzati.

Durante l’associazione di una tipologia a un messaggio o a un relativo modello, le regole di tipologia incluse in essa vengono eseguite per verificare la validità del messaggio.

### Parametri di pressione {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso consegna"
>abstract="I pesi di distribuzione consentono di identificare le consegne prioritarie nel quadro della gestione della pressione. I messaggi con il peso maggiore hanno priorità."

In questa sezione, i parametri di pressione consentono di definire una soglia. È il numero massimo di messaggi che possono essere inviati a un profilo in un dato periodo di tempo. Una volta raggiunta tale soglia, non potranno più essere effettuate ulteriori consegne fino alla fine del periodo considerato. Questo processo ti consente di escludere automaticamente un profilo da una consegna se un messaggio supera la soglia impostata, evitando in tal modo una sollecitazione eccessiva.

I valori di soglia possono essere costanti o variabili. Ciò significa che per un dato periodo le soglie possono variare da un profilo all’altro, o anche per lo stesso profilo.

In **Tipo di peso** sono disponibili tre opzioni:

La **Peso della consegna** field consente di:

La **Modalità di consegna** campo.

### Impostazioni capacità {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importanza del destinatario"
>abstract="L’importanza del destinatario è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità."

In questa sezione puoi selezionare una regola di capacità definita nella console Adobe Campaign v8. Questa regola è associata al canale e-mail.

La **importanza del destinatario** field è una formula utilizzata per determinare quali destinatari vengono mantenuti quando vengono superate le regole di tipologia della capacità.

## Pubblico {#audience}

In questa sezione, puoi scegliere una mappatura di destinazione definita nella console Adobe Campaign v8. La creazione della mappatura di destinazione è necessaria nel caso in cui utilizzi una tabella dei destinatari diversa da quella fornita da Adobe Campaign.

## Consegna {#delivery}

Prova la consegna SMTP: utilizza questa opzione per testare l’invio tramite SMTP. La consegna viene elaborata fino alla connessione al server SMTP, ma non viene inviata: per ogni destinatario della consegna, Campaign si connette al server del provider SMTP, esegue il comando SMTP RCPT TO e chiude la connessione prima del comando SMTP DATA.

Ccn e-mail: utilizza questa opzione per memorizzare le e-mail su un sistema esterno tramite CCN semplicemente aggiungendo un indirizzo e-mail CCN al target del messaggio.

### Nuovi tentativi {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Numero massimo di nuovi tentativi"
>abstract="Se un messaggio non riesce a causa di un errore temporaneo, verranno eseguiti nuovi tentativi per tutta la durata della consegna."

I messaggi temporaneamente non consegnati a causa di un errore morbido o ignorato sono soggetti a un nuovo tentativo automatico. Per impostazione predefinita, sono pianificati cinque nuovi tentativi per il primo giorno della consegna con un intervallo minimo di un’ora suddiviso nelle 24 ore del giorno. Un nuovo tentativo al giorno viene programmato dopo e fino alla scadenza della consegna, definita nella scheda Validità .

## Attività Approval {#approval}

**Manuale**

**Semiautomatico**

**Automatica**

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modalità di approvazione"
>abstract="Ogni fase di una consegna può essere soggetta ad approvazione per garantire il pieno monitoraggio e controllo dei vari processi."

## Validità {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Durata consegna"
>abstract="Il campo Durata consegna ti consente di inserire il limite per i tentativi di consegna globali. Questo significa che Adobe Campaign invia i messaggi a partire dalla data di inizio e quindi, per i messaggi che restituiscono un errore, vengono eseguiti tentativi regolari e configurabili fino al raggiungimento del limite di validità."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite di validità delle risorse"
>abstract="Il campo Limite di validità viene utilizzato per le risorse caricate, principalmente per la pagina speculare e per le immagini. Le risorse presenti in questa pagina sono valide per un periodo di tempo limitato."


Il campo Durata consegna ti consente di inserire il limite per i tentativi di consegna globali. Questo significa che Adobe Campaign invia i messaggi a partire dalla data di inizio e quindi, per i messaggi che restituiscono un errore, vengono eseguiti tentativi regolari e configurabili fino al raggiungimento del limite di validità.

Puoi anche scegliere di specificare le date. A questo scopo, selezionare Imposta esplicitamente le date di validità. In questo caso, le date del limite di consegna e validità ti consentono anche di specificare l’ora. L’ora corrente viene utilizzata per impostazione predefinita, ma puoi modificarla direttamente nel campo di input.

Limite di validità delle risorse: Il campo Limite di validità viene utilizzato per le risorse caricate, principalmente per la pagina speculare e per le immagini. Le risorse presenti in questa pagina sono valide per un periodo di tempo limitato (per risparmiare spazio su disco).

### Gestione di pagine mirror {#mirror}

**Gestione di pagine mirror**

### Tracciamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Periodo di validità"
>abstract="Questa opzione definisce la durata per la quale verrà attivato il tracciamento sugli URL."

**Limite di validità del tracciamento**: Questa opzione definisce la durata per la quale verrà attivato il tracciamento sugli URL.

**URL di sostituzione per gli URL scaduti**: TBC


## Impostazioni di test{#test-setttings}

**Mantieni doppio**

**Mantieni indirizzi inseriti nell’elenco Bloccati**

**Mantieni indirizzi in quarantena**

**Usa il codice di consegna per la bozza**

**Prefisso etichetta**