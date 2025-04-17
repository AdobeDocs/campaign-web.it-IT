---
audience: end-user
title: Rapporti direct mail
description: Scopri come accedere e utilizzare i report Direct mail
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 26%

---

# Rapporto sulle consegne Direct mail {#direct-mail-report}

Il **report di consegna direct mail** fornisce informazioni complete e dati specifici per la consegna direct mail. Include informazioni dettagliate su prestazioni, efficacia e risultati delle singole consegne, offrendo una panoramica completa.

## Riepilogo della consegna {#delivery-summary-direct-mail}

### Panoramica della consegna {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Panoramica della consegna"
>abstract="La **Panoramica della consegna** presenta le metriche delle prestazioni chiave (KPI) che offrono informazioni approfondite sull’interazione dei visitatori con ogni consegna di direct maili. Le metriche sono descritte di seguito."

La **[!UICONTROL Panoramica della consegna]** fornisce informazioni dettagliate sulle interazioni dei visitatori con ogni consegna di direct mailing, mostrando le metriche delle prestazioni chiave (KPI, Key Performance Metrics) essenziali. Le metriche sono descritte di seguito.

![Grafico delle metriche di panoramica della consegna che mostra gli indicatori di prestazioni chiave per la consegna direct mailing.](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++Ulteriori informazioni sulle metriche di panoramica della consegna.

* **[!UICONTROL Messaggi da consegnare]**: numero totale di messaggi elaborati durante la preparazione della consegna.
* **[!UICONTROL Destinati]**: numero di profili utente qualificati come profili di destinazione per i messaggi di direct mailing.
* **[!UICONTROL Da escludere]**: numero di profili utente esclusi dai profili target che non riceveranno messaggi di direct mailing.
+++

### Popolazione target iniziale {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Popolazione target iniziale"
>abstract="Il grafico della **Popolazione target iniziale** mostra i dati relativi ai destinatari e ai messaggi, in base ai risultati della preparazione della consegna."

Il grafico **[!UICONTROL Popolazione target iniziale]** visualizza i dati relativi ai destinatari. Le metriche vengono calcolate durante la preparazione della consegna e includono il pubblico iniziale, il numero di messaggi da inviare e il numero di destinatari esclusi.

![Grafico iniziale della popolazione target con dimensioni del pubblico, messaggi da inviare ed esclusioni.](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Passa il puntatore del mouse su una parte del grafico per visualizzare il numero esatto.

![Visualizzazione dettagliata del grafico della popolazione di destinazione iniziale con funzionalità al passaggio del mouse.](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche dei rapporti di consegna Direct mail.

* **[!UICONTROL Pubblico iniziale]**: numero totale di destinatari target.
* **[!UICONTROL Da consegnare]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.
* **[!UICONTROL Esclusione]**: numero totale di destinatari esclusi dalla popolazione target.
+++

### Statistiche consegna {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Statistiche consegna"
>abstract="Il grafico **Statistiche di consegna** descrive il successo della consegna direct mail e gli errori che si sono verificati."

Il grafico **[!UICONTROL Statistiche di consegna]** fornisce una panoramica delle prestazioni di consegna, offrendo metriche dettagliate per misurare il successo e l&#39;efficacia.

![Grafico delle statistiche di consegna che mostra tassi di successo, errori e quarantene.](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++Ulteriori informazioni sulle metriche dei rapporti delle campagne direct mail.

* **[!UICONTROL Messaggio inviato]**: numero totale di messaggi da consegnare dopo la preparazione della consegna.
* **[!UICONTROL Operazione completata]**: numero di messaggi elaborati correttamente confrontato con il numero di messaggi da recapitare.
* **[!UICONTROL Errori]**: numero totale di errori accumulati durante le consegne e l&#39;elaborazione automatica di rimbalzo rispetto al numero di messaggi da consegnare.
* **[!UICONTROL Nuove quarantene]**: numero totale di indirizzi messi in quarantena dopo la consegna non riuscita (ad esempio, utente sconosciuto, dominio non valido) rispetto al numero di messaggi da recapitare.
+++

### Cause di esclusione {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Cause di esclusione della consegna"
>abstract="Il grafico **Cause di esclusione** illustra la distribuzione dei messaggi rifiutati durante la preparazione per la consegna, suddivisi per regola."

Il grafico **[!UICONTROL Cause di esclusione]** fornisce una suddivisione dei motivi del rifiuto del messaggio durante la preparazione della consegna. Questa disaggregazione è organizzata in base a diverse regole, offrendo una visione dettagliata dei fattori che contribuiscono all’esclusione dei messaggi. Le regole di esclusione sono descritte in dettaglio nella [documentazione di Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=it#email-error-types){_blank}.

![Grafico delle cause di esclusione che mostra la distribuzione dei messaggi rifiutati per regola.](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Ulteriori informazioni sulle metriche Cause di esclusione.

* **[!UICONTROL Indirizzo in quarantena]**: tipo di errore generato quando un indirizzo viene messo in quarantena.
* **[!UICONTROL Indirizzo non specificato]**: tipo di errore generato quando un indirizzo non esiste.
* **[!UICONTROL Indirizzo di qualità non valido]**: tipo di errore generato quando la valutazione della qualità dell&#39;indirizzo postale è troppo bassa.
* inserire nell&#39;elenco Bloccati inserire nell&#39;elenco Bloccati **[!UICONTROL Indirizzo]**: tipo di errore generato quando il destinatario è stato durante la consegna.
* **[!UICONTROL Doppio]**: tipo di errore generato quando il destinatario è stato escluso a causa di valori di chiave non univoci.
* **[!UICONTROL Gruppo di controllo]**: l&#39;indirizzo del destinatario fa parte del gruppo di controllo.
* **[!UICONTROL Destinazione con dimensione limitata]**: è stata raggiunta la dimensione massima di consegna per il destinatario.
+++

### Esclusioni {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Esclusioni"
>abstract="La tabella **[!UICONTROL Esclusioni]** mostra una suddivisione dettagliata, per regola, dei messaggi rifiutati durante il processo di preparazione della consegna."

La tabella **[!UICONTROL Esclusioni]** fornisce un raggruppamento dettagliato, suddiviso per regole specifiche, dei messaggi rifiutati durante la preparazione della consegna. Questa suddivisione offre una chiara comprensione dei motivi alla base dell’esclusione dei messaggi.

![Tabella delle esclusioni che mostra la suddivisione dettagliata dei messaggi rifiutati per regola.](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Le metriche disponibili sono le stesse delle [cause di esclusione](#direct-mail-delivery-exclusions) descritte in precedenza.