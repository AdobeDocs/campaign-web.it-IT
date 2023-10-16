---
audience: end-user
title: Rapporti sulle consegne e-mail
description: Scopri come accedere ai rapporti sulle consegne e-mail e come utilizzarli
badge: label="Beta"
exl-id: 2a0bd3e9-5d75-47c8-bd6a-b3e0b1ce0a01
source-git-commit: fa68c32b61583e41819cfe4e31bc17305126396c
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 99%

---

# Rapporto sulla consegna e-mail {#email-report}

Il **Rapporto sulle consegne e-mail** offre informazioni complete e dati specifici per il canale e-mail. Fornisce una panoramica completa con informazioni dettagliate su prestazioni, efficacia e risultati delle singole consegne.

## Riepilogo delle consegne {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Invio reportistica"
>abstract="La scheda **Invio** all’interno del rapporto fornisce informazioni approfondite sulle interazioni dei visitatori con le consegne e su eventuali errori potenziali riscontrati."

### Popolazione target iniziale {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Popolazione target iniziale"
>abstract="Il grafico della **Popolazione target iniziale** mostra i dati relativi ai destinatari e ai messaggi, in base ai risultati della preparazione della consegna."

Il grafico **[!UICONTROL Popolazione target iniziale]** mostra i dati relativi ai destinatari. Le metriche vengono calcolate durante la preparazione della consegna e mostrano: il pubblico iniziale, il numero di messaggi da inviare e il numero di destinatari esclusi.

![](assets/reporting_email_1.png){width="50%" align="left" zoomable="yes"}

Passa il puntatore del mouse su una parte del grafico per visualizzare il numero esatto.

![](assets/reporting_email_1.1.png){width="50%" align="left" zoomable="yes"}


+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

* **[!UICONTROL Da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di destinatari esclusi dalla popolazione target.
+++

### Statistiche consegna {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Statistiche consegna"
>abstract="Il grafico **Statistiche consegna** descrive il successo della consegna e gli errori che si sono verificati."


Il grafico **[!UICONTROL Statistiche consegna]** descrive il successo della consegna. Le metriche sono descritte di seguito.

![](assets/reporting_email_2.png){width="50%" align="left" zoomable="yes"}

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Messaggio inviato]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

### Cause di esclusione  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Cause di esclusione della consegna"
>abstract="Il grafico e la tabella **Cause di esclusione** mostrano il raggruppamento per regola dei messaggi rifiutati durante la preparazione della consegna."


Il grafico e la tabella **[!UICONTROL Cause di esclusione]** mostrano il raggruppamento per regola dei messaggi rifiutati durante la preparazione della consegna. Le regole di esclusione sono descritte nella [Documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Utente sconosciuto]**: tipo di errore generato durante la consegna per indicare che l’indirizzo e-mail non è valido.

* **[!UICONTROL Dominio non valido]**: tipo di errore generato durante l’invio di una consegna per indicare che il dominio dell’indirizzo e-mail è errato o non esiste.

* **[!UICONTROL Cassetta postale piena]**: tipo di errore generato dopo cinque tentativi di consegna per indicare che la casella in entrata dei destinatari contiene troppi messaggi.

* **[!UICONTROL Account disabilitato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste più.

* **[!UICONTROL Rifiutato]**: tipo di errore generato quando un indirizzo viene rifiutato da IAP (Internet Access Provider), ad esempio in seguito all’applicazione di una regola di sicurezza (software anti-spam).

* **[!UICONTROL Non raggiungibile]**: tipo di errore che si verifica nella stringa di distribuzione del messaggio: incidente sul relay SMTP, dominio temporaneamente non raggiungibile, ecc.

* **[!UICONTROL Non connesso]**: tipo di errore per indicare che il telefono cellulare del destinatario è spento o disconnesso dalla rete al momento dell’invio.

+++

## Velocità di consegna {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Velocità di consegna"
>abstract="Il rapporto **Velocità di consegna** presenta informazioni dettagliate sulla velocità effettiva di consegna dell’intera piattaforma in un arco temporale specifico."

Questo rapporto presenta informazioni dettagliate sulla velocità effettiva di consegna dell’intera piattaforma in un arco temporale specifico. La metrica primaria utilizzata per misurare la velocità di consegna dei messaggi è il numero di messaggi inviati all’ora.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Statistiche di trasmissione {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Statistiche di trasmissione"
>abstract="Il rapporto **Statistiche di trasmissione** contiene i dati disponibili per i possibili errori riscontrati in ciascun dominio."

La tabella **[!UICONTROL Statistiche di trasmissione]** contiene i dati disponibili per i possibili errori riscontrati in ciascun dominio. Le metriche sono descritte di seguito.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL E-mail elaborate]**: numero totale di messaggi elaborati dal server di consegna.

* **[!UICONTROL Consegnato]**: percentuale del numero di messaggi elaborati correttamente rispetto al numero totale di messaggi elaborati.

* **[!UICONTROL Mancati recapiti permanenti]**: percentuale del numero di mancati recapiti permanenti, ossia errori permanenti, ad esempio per indirizzo e-mail errato, rispetto al numero totale di messaggi elaborati.

* **[!UICONTROL Mancati recapiti non permanenti]**: percentuale del numero di mancati recapiti non permanenti, ossia errori temporanei, ad esempio una casella in entrata piena, rispetto al numero totale di messaggi elaborati

* **[!UICONTROL Aperture]**: percentuale del numero di destinatari che hanno aperto un messaggio almeno una volta rispetto al numero di messaggi elaborati correttamente.

* **[!UICONTROL Clic]**: percentuale del numero di persone che hanno fatto clic su una consegna almeno una volta rispetto al numero di messaggi elaborati correttamente.

* **[!UICONTROL Annullamenti iscrizione]**: percentuale del numero di clic su un collegamento di annullamento dell’iscrizione rispetto al numero di messaggi elaborati correttamente.
+++

## Non consegnabili {#non-deliverables-email}

### Raggruppamento degli errori per tipo {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Raggruppamento degli errori per tipo"
>abstract="La tabella e il grafico **Raggruppamento degli errori per tipo** contengono i dati disponibili per ogni tipo di errore riscontrato: utente sconosciuto, cassetta postale piena, dominio non valido e altro ancora."

La tabella e il grafico **[!UICONTROL Raggruppamento degli errori per tipo]** contengono i dati disponibili per ciascun tipo di errore riscontrato. Le metriche sono descritte di seguito.

Gli errori inclusi in questo rapporto attivano il processo di quarantena. Per ulteriori informazioni sulla gestione della quarantena, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=it){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Utente sconosciuto]**: tipo di errore generato durante la consegna per indicare che l’indirizzo e-mail non è valido.

* **[!UICONTROL Dominio non valido]**: tipo di errore generato durante l’invio di una consegna per indicare che il dominio dell’indirizzo e-mail è errato o non esiste.

* **[!UICONTROL Cassetta postale piena]**: tipo di errore generato dopo cinque tentativi di consegna per indicare che la casella in entrata dei destinatari contiene troppi messaggi.

* **[!UICONTROL Account disabilitato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste più.

* **[!UICONTROL Rifiutato]**: tipo di errore generato quando un indirizzo viene rifiutato da IAP (Internet Access Provider), ad esempio in seguito all’applicazione di una regola di sicurezza (software anti-spam).

* **[!UICONTROL Non raggiungibile]**: tipo di errore che si verifica nella stringa di distribuzione del messaggio: incidente sul relay SMTP, dominio temporaneamente non raggiungibile, ecc.

* **[!UICONTROL Non connesso]**: tipo di errore per indicare che il telefono cellulare del destinatario è spento o disconnesso dalla rete al momento dell’invio.

+++


### Raggruppamento degli errori per dominio {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Raggruppamento degli errori per dominio"
>abstract="La tabella e il grafico **Raggruppamento degli errori per dominio** contengono i dati disponibili per ogni tipo di errore riscontrato in base a ciascun dominio."


La tabella e il grafico **[!UICONTROL Raggruppamento degli errori per dominio]** contengono i dati disponibili per i possibili errori riscontrati con ciascun dominio.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Fai clic sull’icona accanto al nome di ciascun dominio per visualizzare i dettagli.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Le metriche disponibili sono le stesse del [Raggruppamento degli errori per tipo](#email-delivery-breakdown-type) descritto in precedenza.

## Indicatori di tracciamento {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Tracciamento reportistica"
>abstract="La scheda **Tracciamento** all’interno del rapporto rende disponibili dati importanti, tra cui il comportamento del destinatario per collegamento, il raggruppamento di aperture e clic, nonché informazioni dettagliate sugli URL cliccati più frequentemente durante una consegna."


### Statistiche consegna  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Statistiche consegna"
>abstract="Il report **Statistiche di consegna** fornisce indicatori chiave di performance (KPI) e informazioni dettagliate sui dati disponibili per le e-mail inviate: riuscite, aperte, click e altro."


Il report **[!UICONTROL Statistiche di consegna]** fornisce indicatori chiave di performance (KPI) e informazioni dettagliate sui dati disponibili per le e-mail inviate. Le metriche sono descritte di seguito.

![](assets/reporting_email_5.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Aperture distinte]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Clic sul collegamento di rinuncia]**: numero di clic sul collegamento di annullamento dell’iscrizione.

* **[!UICONTROL Clic sul collegamento mirror]**: numero di clic sul collegamento alla pagina mirror.

* **[!UICONTROL Stima degli inoltri]**: stima del numero di e-mail inoltrate dai destinatari target.
+++

### Percentuale di apertura e click-through {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Percentuale di apertura e click-through"
>abstract="La tabella **Percentuale di apertura e click-through** mostra i dati relativi al coinvolgimento dei destinatari nella consegna."



La tabella **[!UICONTROL Percentuale di apertura e click-through]** mostra i dati relativi ai destinatari. Le metriche sono descritte di seguito.

![](assets/reporting_email_6.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Inviati]**: numero totale di messaggi inviati.

* **[!UICONTROL Reclami]**: numero di messaggi per questo dominio che sono stati segnalati come indesiderati dal destinatario.

* **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Clic]**: numero di destinatari target distinti che hanno fatto clic almeno una volta nella stessa consegna.

* **[!UICONTROL Reattività raw]**: percentuale del numero di destinatari che hanno fatto clic su una consegna almeno una volta rispetto al numero di destinatari che hanno aperto una consegna almeno una volta.
+++

## URL e flussi di clic {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL e flussi di clic"
>abstract="Il rapporto **URL e flussi di clic** fornisce indicatori chiave di performance (KPI) che offrono informazioni dettagliate sugli URL più cliccati durante una consegna."


Il rapporto **[!UICONTROL URL e flussi di clic]** fornisce indicatori chiave di performance (KPI) che offrono informazioni dettagliate sugli URL più cliccati durante una consegna.

![](assets/reporting_email_7.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

* **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Media piattaforma]**: questa media, visualizzata sotto ogni valore (reattività, clic distinti e clic cumulativi), è calcolata per le consegne inviate nei sei mesi precedenti. Vengono prese in considerazione solo le consegne con la stessa tipologia e sullo stesso canale. Le bozze sono escluse.

+++

### 10 collegamenti più visitati {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="10 collegamenti più visitati"
>abstract="Il grafico e la tabella **10 collegamenti più visitati** contengono i dati disponibili sul comportamento dei destinatari in base al collegamento."


Il grafico e la tabella **[!UICONTROL 10 collegamenti più visitati]** contengono i dati disponibili sul comportamento dei destinatari in base al collegamento.

![](assets/reporting_email_8.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Percentuale]**: percentuale di utenti che hanno interagito con la consegna.

+++

### Raggruppamento dei clic nel tempo {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="Raggruppamento dei clic nel tempo"
>abstract="Il grafico **Raggruppamento dei clic nel tempo** contiene i dati disponibili per il comportamento dei destinatari in base al collegamento."


Il grafico **[!UICONTROL Raggruppamento dei clic nel tempo]** contiene i dati disponibili per il comportamento dei destinatari in base al collegamento.

![](assets/reporting_email_9.png){align="center"}

## Attività degli utenti {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Attività degli utenti"
>abstract="Il grafico **Attività degli utenti** mostra il raggruppamento di aperture e clic sotto forma di grafico. Puoi scegliere il periodo di tempo in cui eseguire il targeting dei dati: ultimo giorno, ultima ora o ultimi 30 minuti."

Il rapporto **[!UICONTROL Attività degli utenti]** mostra il raggruppamento di aperture e clic sotto forma di grafico. Puoi scegliere il periodo di tempo in cui eseguire il targeting dei dati: ultimo giorno, ultima ora o ultimi 30 minuti.

![](assets/reporting_email_10.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

+++

## Statistiche di tracciamento {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Statistiche di tracciamento"
>abstract="Il grafico **Statistiche di tracciamento** fornisce statistiche su aperture e clic. Puoi selezionare l’arco temporale specifico per il targeting dei dati."

Il grafico **[!UICONTROL Statistiche di tracciamento]** fornisce statistiche su aperture e clic. Puoi selezionare l’arco temporale specifico per il targeting dei dati.

![](assets/reporting_email_11.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

+++

## Raggruppamenti delle aperture {#breakdown-opens}

### Raggruppamento delle aperture per dispositivo {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Raggruppamento per dispositivo"
>abstract="Il rapporto **Raggruppamento per dispositivo** mostra il raggruppamento dei messaggi aperti per tipo di dispositivo per il periodo in questione. Per ogni categoria vengono utilizzati due grafici. Il primo visualizza le statistiche relative all’apertura su un computer e dispositivi mobili. Il secondo visualizza il numero esatto e la percentuale per ciascun tipo di dispositivo."

Il rapporto **Raggruppamento per dispositivo** mostra, per il periodo in questione, il raggruppamento delle aperture per dispositivo: personal computer, dispositivi Android, dispositivi Apple o altri.

Per ogni categoria vengono utilizzati due grafici. Il primo visualizza le statistiche relative all’apertura su un computer e dispositivi mobili. Il secondo visualizza il numero esatto e la percentuale per ciascun tipo di dispositivo.

![](assets/reporting_email_13.png){align="center"}


### Raggruppamento delle aperture per sistema operativo {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Raggruppamento per sistema operativo"
>abstract="Il rapporto **Raggruppamento per sistema operativo** mostra il raggruppamento delle aperture per sistema operativo per il periodo in questione. Il primo grafico visualizza le statistiche relative all’apertura su computer e dispositivi mobili. Il secondo visualizza il numero esatto e la percentuale per ciascun sistema operativo."

Il rapporto **Raggruppamento per sistema operativo** mostra, per il periodo in questione, il raggruppamento delle aperture per sistema operativo: sistemi Windows, sistemi Android, sistemi iOS o altri.

Per ogni categoria vengono utilizzati due grafici. Il primo visualizza le statistiche relative alle aperture su sistemi operativi di computer e dispositivi mobili. Il secondo visualizza il numero e la percentuale esatti per ciascun sistema operativo.

![](assets/reporting_email_13.1.png){align="center"}

### Raggruppamento delle aperture per browser {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Raggruppamento per browser"
>abstract="Il **Raggruppamento per browser** mostra il raggruppamento delle aperture per browser per il periodo in questione. Il primo grafico visualizza le statistiche relative all’apertura su computer e dispositivi mobili. Il secondo mostra il numero esatto e la percentuale per ciascun browser."

Il rapporto **Raggruppamento per browser** mostra il raggruppamento delle aperture per browser: Chrome, Safari, Internet Explorer e altri.

Per ogni categoria vengono utilizzati due grafici. Il primo visualizza le statistiche relative alle aperture su sistemi operativi di computer e dispositivi mobili. Il secondo mostra il numero esatto e la percentuale per ciascun browser.

![](assets/reporting_email_13.2.png){align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Rapporto sugli Hotclicks"
>abstract="Il rapporto sugli **Hotclicks** mostra il contenuto dell’e-mail (HTML e/o testo) e la percentuale di clic per ogni collegamento. I blocchi di personalizzazione, i collegamenti per annullare l’iscrizione, per le pagine mirror e per le offerte vengono presi in considerazione nei clic totali cumulati, ma non vengono mostrati nel rapporto."

Questo rapporto mostra il contenuto del messaggio (HTML e/o testo) e la percentuale di clic per ogni collegamento. I blocchi di personalizzazione, i collegamenti per annullare l’iscrizione, per le pagine mirror e per le offerte vengono presi in considerazione nei clic totali cumulati, ma non vengono mostrati nel rapporto.

![](assets/reporting11.png)
