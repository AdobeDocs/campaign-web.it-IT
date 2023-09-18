---
audience: end-user
title: Rapporti sulla campagna
description: Scopri come accedere ai rapporti sulle consegne e come utilizzarli
badge: label="Beta"
source-git-commit: 173bed2c5651e09965a92a848b07d3368c10bb42
workflow-type: tm+mt
source-wordcount: '1853'
ht-degree: 94%

---

# Rapporti sulla campagna {#campaign-reports}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Reportistica sull’invio"
>abstract="La scheda Invio all’interno del rapporto fornisce informazioni approfondite sulle interazioni dei visitatori con le consegne e su eventuali errori potenziali riscontrati."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Tracciamento reportistica"
>abstract="La scheda Invio all’interno del rapporto offre dati preziosi, tra cui il comportamento del destinatario per collegamento, il raggruppamento di aperture e clic, nonché informazioni dettagliate sugli URL su cui si è fatto clic più frequentemente durante una consegna."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Panoramica della consegna"
>abstract="La Panoramica della consegna fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori si interagiscono con la consegna delle e-mail."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Statistiche iniziali sul pubblico target"
>abstract="La tabella delle statistiche del pubblico di destinazione iniziale mostra i dati relativi ai destinatari"

Il rapporto sulle campagne è suddiviso in diversi widget che descrivono il successo e gli errori di una campagna.

La pagina del rapporto della campagna verrà visualizzata con le seguenti schede:

* [Canale e-mail](#email-channel)
* [Canale SMS](#sms-channel)
* [Canale push](#push-channel)

Per accedere al rapporto della campagna, fai clic su Rapporti nella dashboard della campagna.

![](assets/campaign_report_email_13.png)

## Canale e-mail {#email-channel}

### Riepilogo delle consegne {#delivery-summary-email}

* La **[!UICONTROL Panoramica della consegna]** offre indicatori chiave di performance (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna e-mail.

  ![](assets/campaign_report_email_1.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Mancati recapiti]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari:

  ![](assets/campaign_report_email_2.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell’elenco Bloccati, ecc.

+++

* La tabella **[!UICONTROL Statistiche esecuzione]** descrive il successo della consegna.

  ![](assets/campaign_report_email_3.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

* La tabella **[!UICONTROL Statistiche sulle reazioni]** contiene i dati disponibili per l’attività del destinatario per la consegna.

  ![](assets/campaign_report_email_4.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Annullamenti iscrizione]**: numero di destinatari che hanno fatto clic sull’annullamento delle iscrizioni per il periodo in questione.

   * **[!UICONTROL Pagina mirror]**: numero di destinatari che hanno fatto clic sul collegamento alla pagina mirror.

   * **[!UICONTROL Inoltri]**: numero di destinatari che hanno fatto clic e che hanno inoltrato l’e-mail.
+++

* La tabella **[!UICONTROL Flussi di clic generati]** mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna.

  ![](assets/campaign_report_email_5.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++

### Non consegnabili {#non-deliverables-email}

* Le tabelle e i grafici **[!UICONTROL Raggruppamento degli errori per tipo]** e **[!UICONTROL Raggruppamento degli errori per dominio]** contengono i dati disponibili per i possibili errori riscontrati per ciascun dominio.

  Gli errori inclusi in questo rapporto attivano il processo di quarantena. Per ulteriori informazioni sulla gestione della quarantena, consulta [Documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=it){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Utente sconosciuto]**: tipo di errore generato durante la consegna per indicare che l’indirizzo e-mail non è valido.

   * **[!UICONTROL Dominio non valido]**: tipo di errore generato durante l’invio di una consegna per indicare che il dominio dell’indirizzo e-mail è errato o non esiste.

   * **[!UICONTROL Cassetta postale piena]**: tipo di errore generato dopo cinque tentativi di consegna per indicare che la casella in entrata dei destinatari contiene troppi messaggi.

   * **[!UICONTROL Account disabilitato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste più.

   * **[!UICONTROL Rifiutato]**: tipo di errore generato quando un indirizzo viene rifiutato da IAP (Internet Access Provider), ad esempio in seguito all’applicazione di una regola di sicurezza (software anti-spam).

   * **[!UICONTROL Non raggiungibile]**: tipo di errore che si verifica nella stringa di distribuzione del messaggio: incidente sul relay SMTP, dominio temporaneamente non raggiungibile, ecc.

   * **[!UICONTROL Non connesso]**: tipo di errore per indicare che il telefono cellulare del destinatario è spento o disconnesso dalla rete al momento dell’invio.

+++

### Indicatori di tracciamento {#tracking-indicators-email}

* **[!UICONTROL Statistiche consegna]** fornisce indicatori di prestazioni chiave (KPI) e informazioni dettagliate sui dati disponibili per le e-mail inviate.

  ![](assets/campaign_report_email_7.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Clic sul collegamento di rinuncia]**: numero di clic sul collegamento di annullamento dell’iscrizione.

   * **[!UICONTROL Clic sul collegamento mirror]**: numero di clic sul collegamento alla pagina mirror.

   * **[!UICONTROL Stima degli inoltri]**: stima del numero di e-mail inoltrate dai destinatari target.
+++

* La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari.

  ![](assets/campaign_report_email_8.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Inviati]**: numero totale di messaggi inviati.

   * **[!UICONTROL Reclami]**: numero di messaggi per questo dominio che sono stati segnalati come indesiderati dal destinatario.

   * **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Clic]**: numero di destinatari target distinti che hanno fatto clic almeno una volta nella stessa consegna.

   * **[!UICONTROL Reattività raw]**: percentuale del numero di destinatari che hanno fatto clic su una consegna almeno una volta rispetto al numero di destinatari che hanno aperto una consegna almeno una volta.
+++

### URL e flussi di clic {#url-email}

* **[!UICONTROL URL e flussi di clic]** fornisce indicatori chiave di performance (KPI) e informazioni dettagliate sugli URL più cliccati durante una consegna.

  ![](assets/campaign_report_email_9.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Media piattaforma]**: questa media, visualizzata sotto ogni valore (reattività, clic distinti e clic cumulativi), è calcolata per le consegne inviate nei sei mesi precedenti. Vengono prese in considerazione solo le consegne con la stessa tipologia e sullo stesso canale. Le bozze sono escluse.
+++

* Il grafico e la tabella **[!UICONTROL 10 collegamenti più visitati]** contengono i dati disponibili per il comportamento dei destinatari in base al collegamento.

  ![](assets/campaign_report_email_10.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Percentuale]**: percentuale di utenti che hanno interagito con la consegna.

+++

* Il grafico **[!UICONTROL Raggruppamento dei clic nel tempo]** contiene i dati disponibili per il comportamento dei destinatari in base al collegamento.

  ![](assets/campaign_report_email_11.png)

### Attività degli utenti {#user-activities-email}

* **[!UICONTROL Attività degli utenti]** mostra il raggruppamento di aperture e clic sotto forma di grafico.

  ![](assets/campaign_report_email_12.png)

  +++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

+++

## Canale SMS {#sms-channel}

### Riepilogo delle consegne {#delivery-summary-sms}

* La **[!UICONTROL Panoramica della consegna]** offre indicatori chiave di performance (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna SMS.

  ![](assets/campaign_report_sms_1.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari:

  ![](assets/campaign_report_sms_2.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell&#39;elenco Bloccati, ecc.

+++

* La tabella **[!UICONTROL Statistiche esecuzione]** descrive il successo della consegna:

  ![](assets/campaign_report_sms_3.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

* La tabella **[!UICONTROL Flussi di clic generati]** mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna:

  ![](assets/campaign_report_sms_4.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++

## Canale push {#push-channel}

### Riepilogo delle consegne {#delivery-summary-push}

* La **[!UICONTROL Panoramica della consegna]** offre indicatori chiave di performance (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna delle notifiche push.

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell&#39;elenco Bloccati, ecc.

+++

* La tabella **[!UICONTROL Statistiche esecuzione]** descrive il successo della consegna:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

* La tabella **[!UICONTROL Flussi di clic generati]** mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++
