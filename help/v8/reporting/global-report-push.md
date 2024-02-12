---
audience: end-user
title: Rapporti globali per il canale push
description: Comprendere i rapporti globali per il canale push
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 33%

---

# Rapporti globali per il canale push {#campaign-reports-push}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Accedi a **[!UICONTROL Rapporti]** menu all&#39;interno di **[!UICONTROL Generazione rapporti]** sezione. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-push}

### Panoramica della consegna {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Panoramica sulla consegna push"
>abstract="Il Push **panoramica della consegna** I KPI forniscono un esame approfondito delle consegne push, con informazioni dettagliate e dati specifici. Fornisce dettagli completi sulle prestazioni, l’efficacia e i risultati delle consegne."

Il **[!UICONTROL Panoramica della consegna]** Il rapporto fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul coinvolgimento dei visitatori con ogni consegna di notifiche push. Le metriche sono descritte di seguito.

![](assets/global_report_push_delivery_overview.png){zoomable=&quot;yes&quot;}

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Clic totali]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

+++

### Pubblico target {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Popolazione target della consegna push"
>abstract="Il **Popolazione target** grafici e tabelle mostrano i dati relativi al pubblico dei messaggi push, presentando informazioni sui messaggi da consegnare ed esclusioni."

Il **[!UICONTROL Pubblico di destinazione]** La tabella e il grafico presentano i dati relativi ai destinatari per ogni consegna di notifiche push inviata. Le metriche sono descritte di seguito.

![](assets/global_report_push_targeted_audience.png){zoomable=&quot;yes&quot;}

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

### Statistiche consegna {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistiche consegna push"
>abstract="Il **Statistiche generali** Il rapporto fornisce informazioni sulle notifiche push inviate, tra cui tassi di successo, errori e quarantene."

Il **[!UICONTROL Statistiche consegna]** La tabella descrive il completamento di ogni consegna di notifiche push. Le metriche sono descritte di seguito.

![](assets/global_report_push_delivery_statistics.png){zoomable=&quot;yes&quot;}

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggi totali]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori/mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (ad esempio a causa di una registrazione non valida, un rifiuto del messaggio, un errore di payload) rispetto al numero di messaggi da consegnare.

  I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

+++

### Cause di esclusione {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Cause push di esclusione"
>abstract="Il **Cause di esclusione** i grafici e le tabelle illustrano i diversi motivi che hanno impedito ai profili utente di ricevere le notifiche push."

Il **[!UICONTROL Cause di esclusione]** il grafico e la tabella mostrano i motivi che hanno impedito ai profili utente, che erano stati esclusi dai profili target, di ricevere il messaggio.

I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

## Velocità di consegna {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Rapporto velocità di consegna"
>abstract="Il **Velocità effettiva di consegna** Il rapporto presenta informazioni dettagliate sulla velocità effettiva di consegna delle notifiche push dell’intera piattaforma in un arco temporale specificato."

![](assets/global_report_push_delivery_throughput.png){zoomable=&quot;yes&quot;}

Il **[!UICONTROL Velocità effettiva di consegna]** Il rapporto offre informazioni complete sull’efficacia del sistema di consegna delle notifiche push, offrendo un riepilogo dettagliato dei tassi di successo e di errore in un determinato periodo di tempo.
