---
audience: end-user
title: Rapporti globali per il canale di direct mailing
description: Ulteriori informazioni sui rapporti globali per il canale di direct mailing
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 44%

---

# Rapporti globali per il canale di direct mailing {#global-report-direct}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Accedi a **[!UICONTROL Rapporti]** menu all&#39;interno di **[!UICONTROL Generazione rapporti]** sezione. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-direct}

### Panoramica della consegna {#delivery-overview-direct}

Il **[!UICONTROL Panoramica della consegna]** presenta le metriche delle prestazioni chiave (KPI, Key Performance Metrics), con informazioni approfondite sull’interazione dei visitatori con ogni consegna di e-mail. Le metriche sono descritte di seguito.

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Annulla iscrizione]**: numero di destinatari che hanno fatto clic sull’opzione per annullare l’abbonamento.
+++

### Pubblico target {#delivery-summary-direct-initial-target}

Tabella e grafico per **[!UICONTROL Pubblico di destinazione]** mostra i dati relativi ai destinatari, con le metriche dettagliate fornite di seguito.

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

### Statistiche consegna {#delivery-summary-direct-exec-stats}

Il **[!UICONTROL Statistiche consegna]** La tabella fornisce una suddivisione del successo di ogni consegna di direct mailing, con le metriche dettagliate descritte di seguito.

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori/mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

### Cause di esclusione {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

Il grafico e la tabella Esclusioni illustrano i motivi che hanno impedito ai profili utente, esclusi dai profili target, di ricevere il messaggio.

## Velocità di consegna {#delivery-throughput}

Questo rapporto fornisce dettagli completi sulla velocità effettiva di consegna entro un intervallo di tempo specificato. La metrica chiave utilizzata per misurare la velocità di consegna dei messaggi è il numero di messaggi inviati all’ora.

## Non consegnabili {#non-deliverables-direct}

### Raggruppamento degli errori per tipo {#delivery-summary-direct-breakdown-per-type}

Il **[!UICONTROL Raggruppamento degli errori per tipo]** la tabella e il grafico presentano i dati relativi a potenziali errori riscontrati in vari domini, con le metriche specifiche fornite di seguito.

Gli errori inclusi in questo rapporto attivano il processo di quarantena. Per ulteriori informazioni sulla gestione della quarantena, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=it){target="_blank"}.

+++Ulteriori informazioni sulla suddivisione degli errori per metrica per tipo.

* **[!UICONTROL Utente sconosciuto]**: tipo di errore generato durante la consegna per indicare che l’indirizzo non è valido.

* **[!UICONTROL Dominio non valido]**: tipo di errore generato durante l’invio di una consegna per indicare che il dominio dell’indirizzo è errato o non esiste.

* **[!UICONTROL Cassetta postale piena]**: tipo di errore generato dopo cinque tentativi di consegna per indicare che la casella in entrata dei destinatari contiene troppi messaggi.

* **[!UICONTROL Account disabilitato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste più.

* **[!UICONTROL Rifiutato]**: tipo di errore generato quando un indirizzo viene rifiutato da IAP (Internet Access Provider), ad esempio in seguito all’applicazione di una regola di sicurezza (software anti-spam).

* **[!UICONTROL Non raggiungibile]**: tipo di errore che si verifica nella stringa di distribuzione del messaggio: incidente sul relay SMTP, dominio temporaneamente non raggiungibile, ecc.

* **[!UICONTROL Non connesso]**: tipo di errore per indicare che il telefono cellulare del destinatario è spento o disconnesso dalla rete al momento dell’invio.

+++

### Raggruppamento degli errori per dominio {#delivery-summary-email-breakdown-per-domain}

Il **[!UICONTROL Raggruppamento degli errori per dominio]** la tabella e il grafico mostrano i dati relativi a potenziali errori all’interno di ciascun dominio. Le metriche sono comuni alla tabella e al grafico **[!UICONTROL Raggruppamento degli errori per tipo]** descritti in precedenza.

