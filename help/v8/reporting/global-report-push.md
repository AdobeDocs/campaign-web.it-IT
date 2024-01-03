---
audience: end-user
title: Rapporti globali per il canale push
description: Comprendere i rapporti globali per il canale push
badge: label="Disponibilità limitata"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 44%

---

# Rapporti globali per il canale push {#campaign-reports-push}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Accedi a **[!UICONTROL Rapporti]** menu all&#39;interno di **[!UICONTROL Generazione rapporti]** sezione. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-push}

### Riepilogo della consegna {#delivery-overview-push}

Il **[!UICONTROL Panoramica della consegna]** Il rapporto fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul coinvolgimento dei visitatori con ogni consegna di notifiche push. Le metriche sono descritte di seguito.

![](assets/global_report_push_delivery_overview.png)

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Clic totali]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

+++

### Pubblico target {#delivery-summary-push-initial-target}

Il **[!UICONTROL Pubblico di destinazione]** La tabella e il grafico presentano i dati relativi ai destinatari per ogni consegna di notifiche push inviata. Le metriche sono descritte di seguito.

![](assets/global_report_push_targeted_audience.png)

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

### Statistiche consegna {#delivery-summary-push-exec-stats}

Il **[!UICONTROL Statistiche consegna]** La tabella descrive il completamento di ogni consegna di notifiche push. Le metriche sono descritte di seguito.

![](assets/global_report_push_delivery_statistics.png)

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggi totali]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori/mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (ad esempio a causa di una registrazione non valida, un rifiuto del messaggio, un errore di payload) rispetto al numero di messaggi da consegnare.

  I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

+++

### Cause di esclusione {#causes-exclusion}

Il **[!UICONTROL Cause di esclusione]** il grafico e la tabella mostrano i motivi che hanno impedito ai profili utente, che erano stati esclusi dai profili target, di ricevere il messaggio.

I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

## Velocità di consegna {#delivery-throughput-sms}

![](assets/global_report_push_delivery_statistics.png)

Questo rapporto fornisce dettagli completi sulla velocità effettiva di consegna entro un intervallo di tempo specificato.

