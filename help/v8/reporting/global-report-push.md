---
audience: end-user
title: Rapporti globali per il canale push
description: Comprendere i rapporti globali per il canale push
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 42%

---

# Rapporti globali per il canale push {#campaign-reports-push}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Passa al menu **[!UICONTROL Report]** nella sezione **[!UICONTROL Reporting]**. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-push}

### Panoramica della consegna {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Panoramica sulla consegna push"
>abstract="I KPI della **panoramica sulla consegna** push forniscono un esame approfondito delle consegne push, con informazioni approfondite e dati specifici. Fornisce dettagli completi sulle prestazioni, l’efficacia e i risultati delle consegne."

Il rapporto **[!UICONTROL Panoramica consegna]** fornisce indicatori prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul coinvolgimento dei visitatori con ogni consegna di notifiche push. Le metriche sono descritte di seguito.

![Metriche di panoramica della consegna, con i KPI relativi alle prestazioni delle notifiche push.](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Clic totali]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l&#39;elaborazione automatica della restituzione in relazione al numero totale di messaggi inviati.

+++

### Pubblico target {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Popolazione target della consegna push"
>abstract="Il grafico e la tabella della **Popolazione target** mostrano i dati relativi al pubblico della messaggistica push, presentando informazioni sui messaggi da consegnare e sulle esclusioni."

La tabella e il grafico **[!UICONTROL Pubblico di destinazione]** presentano i dati relativi ai destinatari per ogni consegna di notifiche push inviata. Le metriche sono descritte di seguito.

![Metriche del pubblico di destinazione, con i dati relativi ai destinatari e alle esclusioni per le notifiche push.](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari di destinazione.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l&#39;analisi durante l&#39;applicazione delle regole: indirizzo mancante, messo in quarantena, in caso di inserisco nell&#39;elenco Bloccati di e motivi simili.

+++

### Statistiche consegna {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistiche di consegna push"
>abstract="Il rapporto **Statistiche complessive** fornisce informazioni sulle notifiche push inviate, tra cui tassi di successo, errori e quarantene."

La tabella **[!UICONTROL Statistiche di consegna]** descrive il completamento di ogni consegna di notifica push. Le metriche sono descritte di seguito.

![Metriche delle statistiche di consegna, con tassi di successo, errori e quarantene per le notifiche push.](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggi totali]**: numero totale di messaggi da recapitare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori / mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica dei rimbalzi in relazione al numero di messaggi da recapitare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (registrazione non valida, rifiuto del messaggio, errore di payload e motivi simili) in relazione al numero di messaggi da recapitare.

  I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

+++

### Cause di esclusione {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Cause di esclusione push"
>abstract="Il grafico e la tabella **Cause di esclusione** illustrano i diversi motivi che hanno impedito ai profili utente di ricevere le notifiche push."

Il grafico e la tabella **[!UICONTROL Cause di esclusione]** visualizzano i motivi che hanno impedito ai profili utente esclusi dai profili target di ricevere il messaggio.

I tipi di errore per le notifiche push sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#push-error-types){target="_blank"}.

## Velocità di consegna {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Rapporto velocità di consegna"
>abstract="Il rapporto **Velocità di consegna** presenta informazioni dettagliate sulla velocità di consegna delle notifiche push dell’intera piattaforma in un arco temporale specifico."

![Metriche di velocità effettiva di consegna che mostrano i tassi di successo e di errore per le notifiche push in un periodo specificato.](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

Il rapporto **[!UICONTROL Throughput di consegna]** offre informazioni complete sull&#39;efficacia del sistema di consegna delle notifiche push, offrendo un riepilogo dettagliato dei tassi di successo e di errore in un periodo specificato.