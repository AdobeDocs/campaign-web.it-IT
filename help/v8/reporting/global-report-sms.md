---
audience: end-user
title: Rapporti globali per il canale SMS
description: Comprendere i rapporti globali per il canale SMS
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 32%

---

# Rapporti globali per il canale SMS {#campaign-reports-sms}

I rapporti globali forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Passa al menu **[!UICONTROL Report]** nella sezione **[!UICONTROL Reporting]**. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-sms}

### Panoramica della consegna {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Panoramica della consegna SMS"
>abstract="I KPI della **panoramica della consegna degli SMS** forniscono un riepilogo dettagliato della consegna degli SMS, fornendo informazioni approfondite e dettagliate e dati specifici. Fornisce informazioni complete sulle prestazioni, l’efficacia e i risultati della consegna."

Il rapporto **[!UICONTROL Panoramica della consegna]** offre indicatori prestazioni chiave (KPI, Key Performance Indicators) completi, con informazioni approfondite sui pattern di interazione dei visitatori con ogni consegna SMS. Di seguito sono descritte le metriche seguenti.

![Schermata del rapporto Panoramica consegna che mostra gli indicatori prestazioni chiave per la consegna SMS.](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Recapitato]**: percentuale di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Tasso di click-through]**: percentuale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Errori]**: percentuale di errori accumulati durante la consegna e l&#39;elaborazione automatica della restituzione, in relazione al numero totale di messaggi inviati.

+++

### Pubblico target {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Popolazione target degli SMS"
>abstract="Il grafico e la tabella della **Popolazione target** presentano i dati relativi al pubblico degli SMS, incluse informazioni sui messaggi da consegnare e sulle esclusioni."

La tabella e il grafico **[!UICONTROL Pubblico di destinazione]** presentano i dati relativi ai destinatari per ogni consegna SMS inviata. Le metriche sono descritte di seguito.

![Schermata del report Pubblico di destinazione che mostra i dati sui destinatari e le esclusioni per le consegne SMS.](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari di destinazione.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l&#39;analisi durante l&#39;applicazione di regole, ad esempio indirizzo mancante, in quarantena o in un inserisco nell&#39;elenco Bloccati di.

+++

### Statistiche consegna {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Statistiche di consegna degli SMS"
>abstract="Il rapporto **Statistiche di consegna** fornisce informazioni complete sull’SMS inviato, offrendo un raggruppamento di varie metriche quali tassi di successo, occorrenze di errori e pubblico messo in quarantena. Questa presentazione dettagliata consente di esaminare in modo approfondito le prestazioni complessive e i risultati del processo di consegna degli SMS."

La tabella **[!UICONTROL Statistiche di consegna]** descrive il completamento di ogni consegna SMS. Le metriche sono descritte di seguito.

![Schermata del rapporto Statistiche di consegna che mostra i tassi di successo, gli errori e le quarantene per le consegne SMS.](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggi totali]**: numero totale di messaggi da recapitare dopo la preparazione della consegna.

* **[!UICONTROL Operazione completata]**: numero di messaggi elaborati correttamente, in relazione al numero di messaggi da recapitare.

* **[!UICONTROL Errori / mancati recapiti]**: numero totale di errori accumulati durante le consegne e l&#39;elaborazione automatica dei rimbalzi, in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena in seguito a una consegna non riuscita (ad esempio, utente sconosciuto, dominio non valido), in relazione al numero di messaggi da recapitare.

  I tipi di errore SMS sono elencati nella [documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#sms-quarantines){target="_blank"}.

+++

### Cause di esclusione {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Cause di esclusione SMS"
>abstract="Il grafico e la tabella **Cause di esclusione** illustrano i diversi motivi che hanno impedito ai profili utente di ricevere i messaggi SMS."

Il grafico e la tabella **[!UICONTROL Cause di esclusione]** visualizzano i motivi che hanno impedito ai profili utente esclusi dai profili di destinazione di ricevere le consegne SMS.

I tipi di errore sono elencati nella [documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#email-error-types){target="_blank"}.

![Schermata del rapporto Cause di esclusione che mostra i motivi delle esclusioni nella consegna SMS.](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Velocità di consegna {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Velocità di consegna SMS"
>abstract="Il rapporto **Velocità di consegna** fornisce informazioni approfondite ed esaurienti sull’efficienza del sistema di consegna dei messaggi SMS, presentando una panoramica dettagliata dei tassi di successo e di errore in un arco temporale specifico."

![Schermata del report Throughput di consegna che mostra le percentuali di successo e di errore per le consegne SMS nel tempo.](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

Il rapporto **[!UICONTROL Throughput di consegna]** offre informazioni complete sull&#39;efficacia del sistema di consegna dei messaggi SMS, offrendo un riepilogo dettagliato dei tassi di successo e di errore in un periodo specificato.