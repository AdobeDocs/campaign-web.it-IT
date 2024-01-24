---
audience: end-user
title: Rapporti sulle campagne per il canale e-mail
description: Ulteriori informazioni sui rapporti sulle campagne per il canale e-mail
badge: label="Disponibilità limitata"
exl-id: c44c91f8-1f88-4087-8417-34be64a2ab19
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '1573'
ht-degree: 99%

---

# Rapporti sulle campagne per il canale e-mail {#campaign-reports-email-channel}

Ogni rapporto di una campagna è suddiviso in diversi widget che ne descrivono il successo e gli errori. Per il canale e-mail, i rapporti e le metriche sono descritti di seguito. Scopri come accedere ai rapporti sulle campagne in [questa pagina](campaign-reports.md).

## Riepilogo della consegna {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Panoramica della consegna"
>abstract="Il rapporto **Panoramica della consegna** offre indicatori chiave di prestazioni (KPI) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna e-mail."

### Panoramica della consegna {#delivery-summary-email-ovv}

La sezione **[!UICONTROL Panoramica della consegna]** offre indicatori chiave di prestazioni (KPI) che forniscono informazioni dettagliate sul modo in cui i visitatori interagiscono con la consegna e-mail. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_1.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Mancati recapiti]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Aperture totali]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Clic totali]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

+++

### Statistiche iniziali sul pubblico target {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Statistiche iniziali sul pubblico target"
>abstract="La tabella Statistiche del pubblico di destinazione iniziale visualizza i dati relativi ai destinatari."

La tabella **[!UICONTROL Statistiche iniziali sul pubblico target]** mostra i dati relativi ai destinatari. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_2.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Rifiutato da regole]**: numero totale di indirizzi ignorati durante l’analisi quando si applicano le regole: indirizzo mancante, messo in quarantena, inserito nell&#39;elenco Bloccati, ecc.

+++

### Statistiche di esecuzione {#delivery-summary-email-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="Statistiche di esecuzione"
>abstract="La tabella **Statistiche di esecuzione** descrive il successo della consegna: messaggi da consegnare, consegne riuscite, errori e nuove quarantene."

La tabella **[!UICONTROL Statistiche di esecuzione]** descrive il successo della consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_3.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l’elaborazione automatica dei messaggi restituiti rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

  I tipi di errore delle e-mail sono elencati nella [Documentazione di Adobe Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#email-error-types){target="_blank"}.

+++

### Statistiche di reazione {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="Statistiche di reazione"
>abstract="La tabella **Statistiche di reazione** mostra i dati disponibili per l’attività del destinatario della consegna: numero di aperture, iscrizioni, annullamenti di iscrizioni, clic sul collegamento alla pagina mirror."

La tabella **[!UICONTROL Statistiche di reazione]** contiene i dati disponibili per l’attività del destinatario della consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_4.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Aperture univoche]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Aperture totali]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Annullamenti iscrizione]**: numero di destinatari che hanno fatto clic sull’annullamento delle iscrizioni per il periodo in questione.

* **[!UICONTROL Pagina mirror]**: numero di destinatari che hanno fatto clic sul collegamento alla pagina mirror.

* **[!UICONTROL Inoltri]**: numero di destinatari che hanno fatto clic e che hanno inoltrato l’e-mail.
+++

### Flussi di clic generati {#delivery-summary-email-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_click_streams"
>title="Flussi di clic generati"
>abstract="La tabella **Flussi di clic generati** mostra i dati disponibili relativi al modo in cui i destinatari hanno interagito con la consegna."

La tabella **[!UICONTROL Flussi di clic generati]** mostra i dati relativi al modo in cui i destinatari hanno interagito con la consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_5.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Clic univoci]**: numero totale di destinatari univoci che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Clic totali]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

+++

## Non consegnabili {#non-deliverables-email}

### Raggruppamento degli errori per tipo {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="Raggruppamento degli errori per tipo"
>abstract="La tabella e il grafico **Raggruppamento degli errori per tipo** contengono i dati disponibili per ogni tipo di errore riscontrato: utente sconosciuto, cassetta postale piena, dominio non valido e altro ancora."

La tabella e il grafico **[!UICONTROL Raggruppamento degli errori per tipo]** contengono i dati disponibili per i possibili errori riscontrati per ciascun tipo di dominio. Le metriche sono descritte di seguito.

Gli errori inclusi in questo rapporto attivano il processo di quarantena. Per ulteriori informazioni sulla gestione della quarantena, consulta la [documentazione di Campaign v8 (console client)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=it){target="_blank"}.

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

### Raggruppamento degli errori per dominio {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_domain"
>title="Raggruppamento degli errori per dominio"
>abstract="La tabella e il grafico **Raggruppamento degli errori per dominio** contengono i dati disponibili per ogni tipo di errore riscontrato in base a ciascun dominio."

La tabella e il grafico **[!UICONTROL Raggruppamento degli errori per dominio]** contengono i dati disponibili dei possibili errori riscontrati in ciascun dominio. Le metriche sono comuni alla tabella e al grafico **[!UICONTROL Raggruppamento degli errori per tipo]** descritti in precedenza.

## Indicatori di tracciamento {#tracking-indicators-email}

### Statistiche consegna {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="Statistiche consegna"
>abstract="Il grafico **Statistiche consegna** descrive il successo della consegna e gli errori che si sono verificati."

Le metriche **[!UICONTROL Statistiche consegna]** forniscono indicatori chiave di prestazioni (KPI) e informazioni dettagliate sui dati disponibili per le e-mail inviate. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_7.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Messaggio/i da consegnare]**: numero di messaggi elaborati correttamente rispetto al numero di messaggi da consegnare.

* **[!UICONTROL Aperture univoche]**: numero totale di destinatari target che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Aperture totali]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Clic sul collegamento di rinuncia]**: numero di clic sul collegamento di annullamento dell’iscrizione.

* **[!UICONTROL Clic sul collegamento mirror]**: numero di clic sul collegamento alla pagina mirror.

* **[!UICONTROL Stima degli inoltri]**: stima del numero di e-mail inoltrate dai destinatari target.
+++

### Percentuale di apertura e click-through {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="Percentuale di apertura e click-through"
>abstract="La tabella **Percentuale di apertura e click-through** mostra i dati relativi al coinvolgimento dei destinatari nella consegna."

La tabella **[!UICONTROL Percentuale di apertura e click-through]** visualizza i dati relativi ai destinatari. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_8.png)

+++ Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Inviati]**: numero totale di messaggi inviati.

* **[!UICONTROL Reclami]**: numero e percentuale di messaggi per questo dominio che sono stati segnalati come indesiderati dal destinatario.

* **[!UICONTROL Aperture univoche]**: numero e percentuale di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

* **[!UICONTROL Clic univoci]**: numero e percentuale di destinatari target distinti che hanno fatto clic almeno una volta nella stessa consegna.

* **[!UICONTROL Reattività raw]**: percentuale del numero di destinatari che hanno fatto clic su una consegna almeno una volta rispetto al numero di destinatari che hanno aperto una consegna almeno una volta.

+++

## URL e flussi di clic {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="URL e flussi di clic"
>abstract="Il rapporto **URL e flussi di clic** fornisce indicatori chiave di prestazioni (KPI) che offrono informazioni dettagliate sugli URL più cliccati durante una consegna."

Il rapporto **[!UICONTROL URL e flussi di clic]** fornisce indicatori chiave di prestazioni (KPI) che offrono informazioni dettagliate sugli URL più cliccati durante una consegna. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_9.png)

+++ Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Reattività]**: rapporto tra il numero di destinatari target che hanno fatto clic in una consegna e il numero stimato di destinatari target che hanno aperto una consegna.

* **[!UICONTROL Clic univoci]**: numero totale di destinatari distinti che hanno fatto clic almeno una volta in una consegna.

* **[!UICONTROL Clic totali]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Media piattaforma]**: questa media, visualizzata sotto ogni valore (reattività, clic distinti e clic cumulativi), è calcolata per le consegne inviate nei sei mesi precedenti. Vengono prese in considerazione solo le consegne con la stessa tipologia e sullo stesso canale. Le bozze sono escluse.

+++

### 10 collegamenti più visitati {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="10 collegamenti più visitati"
>abstract="Il grafico e la tabella **10 collegamenti più visitati** contengono i dati disponibili sul comportamento dei destinatari in base al collegamento."

Il grafico e la tabella **[!UICONTROL 10 collegamenti più visitati]** contengono i dati disponibili sul comportamento dei destinatari in base al collegamento. Le metriche sono descritte di seguito.

![](assets/campaign_report_email_10.png)

+++Ulteriori informazioni sulle metriche del rapporto sulla campagna e-mail.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Percentuale]**: percentuale di utenti che hanno interagito con la consegna.

+++

### Raggruppamento dei clic nel tempo {#campaign-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="Raggruppamento dei clic nel tempo"
>abstract="Il grafico **Raggruppamento dei clic nel tempo** contiene i dati disponibili per il comportamento dei destinatari in base al collegamento."

Il grafico **[!UICONTROL Raggruppamento dei clic nel tempo]** contiene i dati disponibili per il comportamento dei destinatari in base al collegamento.

![](assets/campaign_report_email_11.png)

## Attività degli utenti {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="Attività degli utenti"
>abstract="Il grafico **Attività degli utenti** mostra il raggruppamento di aperture e clic sotto forma di grafico."

Il rapporto **[!UICONTROL Attività degli utenti]** mostra il raggruppamento di aperture e clic sotto forma di grafico. Le metriche di questo rapporto sono descritte di seguito.

![](assets/campaign_report_email_user_activities.png){align="center"}

+++Ulteriori informazioni sulle metriche del rapporto sulle consegne e-mail.

* **[!UICONTROL Clic]**: numero totale di clic sui collegamenti nelle consegne.

* **[!UICONTROL Aperture]**: numero di destinatari target distinti per questo dominio che hanno aperto un messaggio almeno una volta.

+++
