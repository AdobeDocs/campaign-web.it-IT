---
audience: end-user
title: Rapporti globali per il canale di direct mailing
description: Ulteriori informazioni sui rapporti globali per il canale di direct mailing
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 23%

---

# Rapporti globali per il canale di direct mailing {#global-report-direct}

I report globali Direct mail forniscono agli utenti una panoramica completa delle metriche di traffico e coinvolgimento a livello di canale.

Accedi a **[!UICONTROL Rapporti]** menu all&#39;interno di **[!UICONTROL Generazione rapporti]** sezione. Puoi filtrare i dati in base alla data del rapporto, alla cartella o alle regole. [Ulteriori informazioni](global-reports.md)

## Riepilogo della consegna {#delivery-summary-direct}

### Panoramica della consegna {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Panoramica della consegna"
>abstract="Il **Panoramica della consegna** presenta le metriche delle prestazioni chiave (KPI, Key Performance Metrics), con informazioni approfondite sull’interazione dei visitatori con ogni consegna di direct mailing. Le metriche sono descritte di seguito."

Il **[!UICONTROL Panoramica della consegna]** presenta le metriche delle prestazioni chiave (KPI, Key Performance Metrics), con informazioni approfondite sull’interazione dei visitatori con ogni consegna di direct mailing. Le metriche sono descritte di seguito.

![](assets/global_report_direct_mail_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Ulteriori informazioni sulle metriche della panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.

* **[!UICONTROL Consegnato]**: numero di messaggi inviati correttamente rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Errori]**: totale degli errori accumulati durante la consegna e l’elaborazione automatica dei messaggi restituiti rispetto al numero totale di messaggi inviati.

* **[!UICONTROL Annulla iscrizione]**: numero di destinatari che hanno fatto clic sull’opzione per annullare l’abbonamento.
+++

### Pubblico target {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Pubblico target"
>abstract="I dati del destinatario e le informazioni sul messaggio vengono visualizzati nel **Pubblico di destinazione** grafico che riflette l’analisi della preparazione della consegna."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Pubblico target"
>abstract="Il **Pubblico di destinazione** La tabella fornisce una suddivisione dettagliata dei destinatari e dei messaggi corrispondenti, in base ai risultati del processo di preparazione della consegna."

Tabella e grafico per **[!UICONTROL Pubblico di destinazione]** mostra i dati relativi ai destinatari, con le metriche dettagliate fornite di seguito.

![](assets/global_report_direct_mail_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++Ulteriori informazioni sulle metriche del pubblico di destinazione.

* **[!UICONTROL Pubblico di destinazione]**: numero totale di destinatari target.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Esclusione]**: numero totale di indirizzi ignorati durante l’analisi durante l’applicazione delle regole: indirizzo mancante, messo in quarantena, in fase di inserisce nell&#39;elenco Bloccati del, ecc.

+++

### Statistiche consegna {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Statistiche consegna"
>abstract="Il **Statistiche consegna** Il grafico fornisce informazioni sull’efficacia delle consegne Direct mailing, incluse le consegne riuscite ed eventuali errori riscontrati."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Statistiche consegna"
>abstract="Il **Statistiche consegna** La tabella descrive il completamento della consegna Direct mailing e gli errori che si sono verificati."

Il **[!UICONTROL Statistiche consegna]** grafico e tabella forniscono una suddivisione del successo di ogni consegna di direct mailing, con metriche dettagliate descritte di seguito.

+++Ulteriori informazioni sulle metriche delle statistiche di consegna.

* **[!UICONTROL Messaggio da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.

* **[!UICONTROL Completato]**: numero di messaggi elaborati correttamente in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Errori/mancati recapiti]**: numero totale di errori accumulati durante le consegne ed elaborazione automatica del rimbalzo in relazione al numero di messaggi da consegnare.

* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena a seguito di una consegna non riuscita (utente sconosciuto, dominio non valido) rispetto al numero di messaggi da consegnare.

+++

### Cause di esclusione {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Esclusioni"
>abstract="Il **Cause di esclusione** nella tabella viene visualizzata una suddivisione dettagliata, per regola, dei messaggi rifiutati durante il processo di preparazione della consegna."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Cause di esclusione della consegna"
>abstract="Il **Cause di esclusione** il grafico illustra la distribuzione dei messaggi rifiutati durante la preparazione per la consegna, suddivisi per regola."

![](assets/global_report_direct_mail_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

Il grafico e la tabella Esclusioni illustrano i motivi che hanno impedito ai profili utente, esclusi dai profili target, di ricevere il messaggio.

+++Ulteriori informazioni sulle metriche Cause di esclusione.

* **[!UICONTROL Indirizzo in quarantena]**: tipo di errore generato quando l’indirizzo viene messo in quarantena.

* **[!UICONTROL Indirizzo non specificato]**: tipo di errore generato durante l’invio di una consegna per indicare che l’indirizzo non esiste.

* **[!UICONTROL Indirizzo di qualità non valida]**: tipo di errore generato quando la valutazione della qualità dell’indirizzo postale è troppo bassa.

* **[!UICONTROL Inserire nell&#39;elenco Bloccati Indirizzo]**: tipo di errore generato quando il destinatario è stato inserito nell&#39;elenco Bloccati al momento dell’esecuzione della consegna.

* **[!UICONTROL Doppio]**: tipo di errore generato quando il destinatario è stato escluso perché i suoi valori delle chiavi non erano univoci.

* **[!UICONTROL Gruppo di controllo]**: l’indirizzo del destinatario fa parte del gruppo di controllo.

* **[!UICONTROL Target di dimensioni limitate]**: è stata raggiunta la dimensione massima di consegna per il destinatario.

+++

