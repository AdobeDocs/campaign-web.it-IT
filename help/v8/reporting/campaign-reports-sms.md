---
audience: end-user
title: Rapporti sulle campagne per il canale SMS
description: Ulteriori informazioni sui rapporti sulle campagne per il canale SMS
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 100%

---

# Rapporti sulle campagne per il canale SMS {#campaign-reports-sms-channel}

Ogni rapporto di una campagna è suddiviso in diversi widget che ne descrivono il successo e gli errori. Per il canale SMS, i rapporti e le metriche sono descritti di seguito. Scopri come accedere ai rapporti sulle campagne in [questa pagina](campaign-reports.md).

## Riepilogo della consegna {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Panoramica della consegna"
>abstract="Il rapporto **Panoramica della consegna** offre indicatori chiave di prestazioni (KPI) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna SMS."


Il rapporto **[!UICONTROL Panoramica della consegna]** offre indicatori chiave di prestazioni (KPI) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna SMS. Le metriche sono descritte di seguito.

![](assets/campaign_report_sms_1.png){zoomable="yes"}

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
>abstract="La tabella **Statistiche iniziali sul pubblico target** mostra i dati relativi ai destinatari"

La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari. Le metriche sono descritte di seguito.


![](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell&#39;elenco Bloccati, ecc.

+++


### Statistiche di esecuzione {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Statistiche di esecuzione"
>abstract="La tabella **Statistiche di esecuzione** descrive il successo della consegna: messaggi da consegnare, consegne riuscite, errori e nuove quarantene."


La tabella **[!UICONTROL Statistiche di esecuzione]** descrive il successo della consegna. Le metriche sono descritte di seguito.


![](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

  I tipi di errore SMS sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#sms-quarantines){target="_blank"}.

+++

### Flussi di clic generati {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Flussi di clic generati"
>abstract="La tabella **Flussi di clic generati** mostra i dati disponibili relativi al modo in cui i destinatari hanno interagito con la consegna."

La tabella **[!UICONTROL Flussi di clic generati]** mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne SMS.

* **[!UICONTROL Clic distinti]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++
