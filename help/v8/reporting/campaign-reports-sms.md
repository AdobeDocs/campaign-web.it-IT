---
audience: end-user
title: Rapporti sulle campagne per il canale SMS
description: Comprendere i rapporti sulle campagne per il canale SMS
badge: label="Beta"
source-git-commit: 5d577c07c4d754e9265482f858c17740f304db42
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 55%

---


# Rapporti sulle campagne per il canale SMS {#campaign-reports-sms-channel}

Ogni rapporto della campagna è diviso in diversi widget che descrivono nel dettaglio il successo e gli errori della campagna. Per il canale SMS, i rapporti e le metriche sono descritti di seguito. Scopri come accedere ai rapporti delle campagne in [questa pagina](campaign-reports.md).

## Riepilogo delle consegne {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Panoramica della consegna"
>abstract="Il **Panoramica della consegna** Il rapporto fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori si interagiscono con la consegna di SMS."


Il **[!UICONTROL Panoramica della consegna]** Il rapporto fornisce indicatori di prestazioni chiave (KPI, Key Performance Indicators) che forniscono informazioni dettagliate sul modo in cui i visitatori si interagiscono con la consegna di SMS. Le metriche sono descritte di seguito.

![](assets/campaign_report_sms_1.png)

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Totale inviato]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++


### Statistiche iniziali sul pubblico target {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Statistiche iniziali sul pubblico target"
>abstract="Il **Statistiche del pubblico di destinazione iniziale** la tabella mostra i dati relativi ai destinatari"

Il **[!UICONTROL Statistiche del pubblico di destinazione iniziale]** nella tabella vengono visualizzati i dati relativi ai destinatari. Le metriche sono descritte di seguito.


![](assets/campaign_report_sms_2.png)

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell&#39;elenco Bloccati, ecc.

+++


### Statistiche di esecuzione {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Statistiche di esecuzione"
>abstract="Il **Statistiche di esecuzione** la tabella descrive il successo della consegna: messaggi da consegnare, successo, errori e nuove quarantene."


Il **[!UICONTROL Statistiche di esecuzione]** la tabella descrive il successo della consegna. Le metriche sono descritte di seguito.


![](assets/campaign_report_sms_3.png)

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

  I tipi di errore SMS sono elencati in [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Flussi di clic generati {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Flussi di clic generati"
>abstract="Il **Flussi di clic generati** La tabella mostra i dati disponibili relativi al modo in cui i destinatari hanno interagito con la consegna."

Il **[!UICONTROL Flussi di clic generati]** La tabella mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_sms_4.png)

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++
