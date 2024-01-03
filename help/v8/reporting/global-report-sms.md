---
audience: end-user
title: Rapporti globali per il canale SMS
description: Comprendere i rapporti globali per il canale SMS
badge: label="Disponibilità limitata"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 26%

---

# Rapporti globali per il canale SMS {#campaign-reports-sms}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Accedi a **[!UICONTROL Rapporti]** menu all&#39;interno di **[!UICONTROL Generazione rapporti]** sezione. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-sms}

### Panoramica della consegna {#delivery-overview-sms}

Il **[!UICONTROL Panoramica della consegna]** Il rapporto offre indicatori di prestazioni chiave (KPI, Key Performance Indicators) completi con informazioni approfondite sui modelli di interazione dei visitatori con ogni consegna di SMS. Di seguito sono descritte le metriche seguenti.

![](assets/global_report_sms_delivery_overview.png)

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: percentuale di messaggi inviati correttamente, in relazione al numero totale di messaggi inviati.

* **[!UICONTROL Percentuale di click-through]**: percentuale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Errori]**: percentuale di errori accumulati durante la consegna e l’elaborazione automatica della restituzione in relazione al numero totale di messaggi inviati.

+++

### Pubblico target {#delivery-summary-sms-initial-target}

Il **[!UICONTROL Pubblico di destinazione]** tabella e grafico presentano i dati relativi ai destinatari per ogni consegna SMS inviata. Le metriche sono descritte di seguito.

![](assets/global_report_sms_targeted_audience.png)

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

### Statistiche consegna {#delivery-summary-sms-exec-stats}

Il **[!UICONTROL Statistiche consegna]** la tabella descrive il successo di ogni consegna SMS. Le metriche sono descritte di seguito.

![](assets/global_report_sms_delivery_statistics.png)

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggi totali]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori/mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

  I tipi di errore SMS sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#sms-quarantines){target="_blank"}.

+++

### Cause di esclusione {#causes-exclusion}

Il **[!UICONTROL Cause di esclusione]** Il grafico e la tabella mostrano i motivi che hanno impedito ai profili utente, che erano stati esclusi dai profili target, di ricevere le consegne SMS.

I tipi di errore sono elencati in [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Velocità di consegna {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

Questo rapporto fornisce dettagli completi sulla velocità effettiva di consegna entro un intervallo di tempo specificato.
