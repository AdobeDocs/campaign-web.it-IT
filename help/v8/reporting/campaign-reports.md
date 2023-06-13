---
audience: end-user
title: Rapporti sulle campagne
description: Scopri come accedere e utilizzare i rapporti delle campagne
badge: label="Alpha" type="Positive"
source-git-commit: 1833f4eafced860592c8419938bc09fe0fe27351
workflow-type: tm+mt
source-wordcount: '1753'
ht-degree: 2%

---

# Rapporti sulle campagne {#campaign-reports}

Il rapporto della campagna è diviso in diversi widget che descrivono nel dettaglio il successo e gli errori della campagna.

La pagina del rapporto della campagna verrà visualizzata con le seguenti schede:

* [Canale e-mail](#email-channel)
* [Canale SMS](#sms-channel)
* [Canale push](#push-channel)

Per accedere al rapporto della campagna, fai clic su Rapporti nel dashboard della campagna.

![](assets/campaign_report_email_13.png)

## Canale e-mail {#email-channel}

### Riepilogo consegne {#delivery-summary-email}

* **[!UICONTROL Panoramica della consegna]** fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna delle e-mail.

  ![](assets/campaign_report_email_1.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente, in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Mancati recapiti]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica della restituzione in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari di destinazione che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* **[!UICONTROL Statistiche del pubblico di destinazione iniziale]** nella tabella vengono visualizzati i dati relativi ai destinatari:

  ![](assets/campaign_report_email_2.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

* **[!UICONTROL Statistiche di esecuzione]** la tabella descrive il successo della consegna.

  ![](assets/campaign_report_email_3.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) in relazione al numero di messaggi da consegnare.

+++

* **[!UICONTROL Statistiche sulle reazioni]** la tabella contiene i dati disponibili per l’attività del destinatario per la consegna.

  ![](assets/campaign_report_email_4.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari di destinazione che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Aperture]**: numero di destinatari di destinazione distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Annullamenti iscrizione]**: numero di destinatari che hanno fatto clic sull’annullamento degli abbonamenti per il periodo in questione.

   * **[!UICONTROL Pagina mirror]**: numero di destinatari che hanno fatto clic sul collegamento della pagina speculare.

   * **[!UICONTROL Forwards]**: numero di destinatari che hanno fatto clic e che hanno inoltrato l’e-mail.
+++

* **[!UICONTROL Flussi di clic generati]** La tabella mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna.

  ![](assets/campaign_report_email_5.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari interessati che hanno fatto clic in una consegna e il numero stimato di destinatari interessati che hanno aperto una consegna.

+++

### Non consegnabili {#non-deliverables-email}

* **[!UICONTROL Raggruppamento degli errori per tipo]** e **[!UICONTROL Raggruppamento degli errori per dominio]** tabelle e grafici contengono i dati disponibili per i possibili errori riscontrati con ciascun dominio.

  Gli errori visualizzati in questo report attivano il processo di quarantena. Per ulteriori informazioni sulla gestione della quarantena, consulta [Gestione della quarantena](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=it).

  ![](assets/campaign_report_email_6.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Utente sconosciuto]**: tipo di errore generato durante la consegna per indicare che l’indirizzo e-mail non è valido.

   * **[!UICONTROL Dominio non valido]**: tipo di errore generato durante l’invio di una consegna per indicare che il dominio dell’indirizzo e-mail è errato o non esiste.

   * **[!UICONTROL Cassetta postale piena]**: tipo di errore generato dopo cinque tentativi di consegna per indicare che la casella in entrata dei destinatari contiene troppi messaggi.

   * **[!UICONTROL Account disabilitato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste più.

   * **[!UICONTROL Rifiutato]**: tipo di errore generato quando un indirizzo viene rifiutato da IAP (Internet Access Provider), ad esempio in seguito all’applicazione di una regola di sicurezza (software anti-spam).

   * **[!UICONTROL Non raggiungibile]**: tipo di errore che si verifica nella stringa di distribuzione del messaggio: incidente sull’inoltro SMTP, dominio temporaneamente non raggiungibile, ecc.

   * **[!UICONTROL Non connesso]**: tipo di errore per indicare che il telefono cellulare del destinatario è spento o disconnesso dalla rete al momento dell’invio.

+++

### Indicatori di tracciamento {#tracking-indicators-email}

* **[!UICONTROL Statistiche consegna]** fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sui dati disponibili per le e-mail inviate.

  ![](assets/campaign_report_email_7.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Aperture distinte]**: numero totale di destinatari di destinazione che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Aperture]**: numero di destinatari di destinazione distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Fai clic sul collegamento di rinuncia]**: numero di clic sul collegamento di annullamento dell’abbonamento.

   * **[!UICONTROL Clic sul collegamento mirror]**: numero di clic sul collegamento alla pagina speculare.

   * **[!UICONTROL Stima degli inoltri]**: stima del numero di e-mail inoltrate dai destinatari interessati.
+++

* **[!UICONTROL Statistiche del pubblico di destinazione iniziale]** nella tabella vengono visualizzati i dati relativi ai destinatari.

  ![](assets/campaign_report_email_8.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Inviato]**: numero totale di messaggi inviati.

   * **[!UICONTROL Reclami]**: numero di messaggi per questo dominio che sono stati segnalati come non desiderati dal destinatario.

   * **[!UICONTROL Aperture]**: numero di destinatari di destinazione distinti per questo dominio che hanno aperto un messaggio almeno una volta.

   * **[!UICONTROL Clic]**: numero di destinatari di destinazione distinti che hanno fatto clic almeno una volta nella stessa consegna.

   * **[!UICONTROL Reattività raw]**: percentuale del numero di destinatari che hanno fatto clic su una consegna almeno una volta rispetto al numero di destinatari che hanno aperto una consegna almeno una volta.
+++

### URL e flussi di clic {#url-email}

* **[!UICONTROL URL e flussi di clic]** fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sugli URL su cui si è fatto clic maggiormente durante una consegna.

  ![](assets/campaign_report_email_9.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari interessati che hanno fatto clic in una consegna e il numero stimato di destinatari interessati che hanno aperto una consegna.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Media piattaforma]** : questo tasso medio, visualizzato sotto ogni tasso (reattività, clic distinti e clic cumulativi), è calcolato per le consegne inviate nei sei mesi precedenti. Vengono prese in considerazione solo le consegne con la stessa tipologia e sullo stesso canale. Le bozze sono escluse.
+++

* **[!UICONTROL I 10 collegamenti più visitati]** il grafico e la tabella contengono i dati disponibili per il comportamento dei destinatari in base al collegamento.

  ![](assets/campaign_report_email_10.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Percento]**: percentuale di utenti che hanno interagito con la consegna.

+++

* **[!UICONTROL Raggruppamento dei clic nel tempo]** il grafico contiene i dati disponibili per il comportamento dei destinatari in base al collegamento.

  ![](assets/campaign_report_email_11.png)

### Attività degli utenti {#user-activities-email}

* **[!UICONTROL Attività degli utenti]** mostra il raggruppamento di aperture e clic sotto forma di grafico.

  ![](assets/campaign_report_email_12.png)

  +++Ulteriori informazioni sulle metriche del rapporto della campagna e-mail.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Aperture]**: numero di destinatari di destinazione distinti per questo dominio che hanno aperto un messaggio almeno una volta.

+++

## Canale SMS {#sms-channel}

### Riepilogo consegne {#delivery-summary-sms}

* **[!UICONTROL Panoramica della consegna]** fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna di SMS.

  ![](assets/campaign_report_sms_1.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente, in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica della restituzione in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* **[!UICONTROL Statistiche del pubblico di destinazione iniziale]** nella tabella vengono visualizzati i dati relativi ai destinatari:

  ![](assets/campaign_report_sms_2.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

* **[!UICONTROL Statistiche di esecuzione]** la tabella descrive il successo della consegna:

  ![](assets/campaign_report_sms_3.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) in relazione al numero di messaggi da consegnare.

+++

* **[!UICONTROL Flussi di clic generati]** la tabella mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna:

  ![](assets/campaign_report_sms_4.png)

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari interessati che hanno fatto clic in una consegna e il numero stimato di destinatari interessati che hanno aperto una consegna.

+++

## Canale push {#push-channel}

### Riepilogo consegne {#delivery-summary-push}

* **[!UICONTROL Panoramica della consegna]** fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna delle notifiche push.

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante l’analisi della consegna.

   * **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente, in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica della restituzione in relazione al numero totale di messaggi inviati.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

* **[!UICONTROL Statistiche del pubblico di destinazione iniziale]** nella tabella vengono visualizzati i dati relativi ai destinatari:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

* **[!UICONTROL Statistiche di esecuzione]** la tabella descrive il successo della consegna:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo l’analisi della consegna.

   * **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

   * **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) in relazione al numero di messaggi da consegnare.

+++

* **[!UICONTROL Flussi di clic generati]** la tabella mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna:

  +++Ulteriori informazioni sulle metriche dei rapporti delle campagne push.

   * **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

   * **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

   * **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari interessati che hanno fatto clic in una consegna e il numero stimato di destinatari interessati che hanno aperto una consegna.

+++
