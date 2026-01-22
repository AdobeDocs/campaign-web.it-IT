---
title: Indicatori chiave di prestazioni
description: Scopri come comprendere gli indicatori chiave di prestazioni
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 48%

---

# Indicatori chiave di prestazioni {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicatori chiave di prestazioni"
>abstract="La sezione **Indicatori chiave di prestazioni** consente di verificare l’efficacia della piattaforma tramite i KPI più diffusi."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI spam"

Passa alla pagina Home per verificare gli indicatori chiave di prestazioni per la tua piattaforma. Questi indicatori mostrano il numero e la percentuale di messaggi consegnati, aperti, su cui è stato fatto clic, di annullamenti di abbonamenti e di tassi di errore.

Per impostazione predefinita, le metriche sono calcolate per le consegne inviate nei sette giorni precedenti. Puoi modificare il periodo dall’elenco a discesa nella sezione superiore destra della scheda. Sono esclusi i messaggi inviati ai profili di test.

Puoi selezionare il canale da visualizzare. Per impostazione predefinita, questi indicatori riflettono le metriche per il canale e-mail.

![Schermata che mostra la scheda KPI con le metriche per il canale e-mail.](assets/kpi.png){zoomable="yes"}

## Messaggio consegnato {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Consegnati"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti i messaggi elaborati correttamente e la percentuale di messaggi consegnati correttamente rispetto al numero totale di messaggi inviati."

Il numero di messaggi consegnati riflette la percentuale di recapitabilità. Non può mai essere 100% per i seguenti motivi: alcuni indirizzi o numeri di telefono possono essere errati, i bloccanti della posta indesiderata presso i provider di posta elettronica possono rifiutare i messaggi o possono verificarsi problemi di recapito.

L&#39;indicatore **Delivered** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di messaggi consegnati con successo rispetto al numero totale di messaggi inviati.

* Somma di tutti i messaggi elaborati correttamente.

In Adobe Campaign, la regola per contrassegnare un messaggio come “Consegnato” è:

Numero di messaggi per i quali il campo &quot;Indirizzo seed&quot; è uguale a &quot;No&quot; e con uno stato uguale a &quot;Preso in considerazione dal provider di servizi&quot; (per SMS), &quot;Inviato&quot; (per e-mail) o &quot;Ricevuto su dispositivi mobili&quot; (per notifiche push).

## Aperture totali {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Messaggi aperti"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti i messaggi aperti e la percentuale dei messaggi aperti rispetto al numero totale di messaggi consegnati correttamente."

Il totale delle aperture viene calcolato tenendo traccia del numero totale di volte in cui un messaggio viene aperto, indipendentemente dal numero di singoli destinatari che generano tali aperture. Questo indicatore è disponibile solo per le e-mail.

L&#39;indicatore **Opens** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di messaggi aperti rispetto al numero totale di messaggi consegnati con successo.

* Somma di tutti i messaggi aperti per canale.

Adobe Campaign rileva le aperture dei messaggi quando il destinatario scarica le immagini nell’e-mail. Le e-mail HTML e Multipart/Alternative includono un’immagine a 0 pixel, che consente di rilevare i messaggi aperti. Poiché i messaggi in formato testo non includono immagini, è impossibile rilevare se sono stati aperti. I valori calcolati in base all’apertura dei messaggi sono sempre stime dovute al margine di errore collegato alla visualizzazione delle immagini.

## Tasso di click-through {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clic"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti gli URL su cui è stato fatto clic nei messaggi e la percentuale di clic rispetto al numero totale di messaggi consegnati correttamente."

Aggiungi URL nel contenuto del messaggio per reindirizzare i destinatari a una pagina particolare. Il tasso di click-through misura il numero e la percentuale di destinatari che hanno fatto clic su un collegamento nel messaggio.

L&#39;indicatore **Clic** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di clic rispetto al numero totale di messaggi consegnati con successo.

* Numero di persone distinte che hanno fatto clic almeno una volta in una consegna. I collegamenti di annullamento dell’abbonamento e i collegamenti alla pagina mirror dell’e-mail sono esclusi.

Queste metriche si basano sulla tabella di tracciamento consolidata (`nms:trackingStats`). Questa tabella aggregata viene utilizzata per motivi di prestazioni durante la visualizzazione dei report, anziché per la tabella dei registri di tracciamento dei destinatari (`nms:trackingLogRcp`). Non viene calcolato in tempo reale. La tabella viene generata pochi minuti dopo il recupero dei registri di tracciamento.

## Percentuali di abbonamento {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Abbonamenti"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti gli abbonamenti a un servizio e la relativa percentuale rispetto al numero totale di messaggi consegnati correttamente."

I destinatari possono acconsentire alle comunicazioni e-mail e SMS.

L&#39;indicatore **Sottoscrizioni** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di abbonamenti rispetto al numero totale di messaggi consegnati con successo.

>[!NOTE]
>
> I KPI per l’iscrizione e l’annullamento dell’iscrizione variano in base al tipo di servizio. Ad esempio, le iscrizioni e gli annullamenti di iscrizioni alle e-mail comprendono tutti i servizi relativi alle e-mail, sia che derivino da azioni manuali che da moduli web. È importante distinguere questo approccio dalla metrica di annullamento dell’iscrizione a livello di consegna, che tiene traccia dei clic sui collegamenti all’annullamento dell’iscrizione anziché degli utenti effettivamente che l’hanno annullata.

## Percentuali di annullamento dell’abbonamento {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Abbonamenti annullati"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti gli annullamenti di iscrizione a un servizio e la relativa percentuale rispetto al numero totale di messaggi consegnati correttamente."

I destinatari devono essere in grado di rinunciare a e-mail e SMS tramite un collegamento dedicato di annullamento dell’abbonamento nel contenuto dell’e-mail o rispondendo STOP a un SMS.

L&#39;indicatore **Annullamenti abbonamenti** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di annullamenti di abbonamento rispetto al numero totale di messaggi consegnati correttamente.

* Somma di tutti i clic su un collegamento di annullamento dell’abbonamento, ovvero con una categoria URL uguale a &quot;Rinuncia&quot;.

>[!NOTE]
>
> I KPI per l’iscrizione e l’annullamento dell’iscrizione variano in base al tipo di servizio. Ad esempio, le iscrizioni e gli annullamenti di iscrizioni alle e-mail comprendono tutti i servizi relativi alle e-mail, sia che derivino da azioni manuali che da moduli web. È importante distinguere questo approccio dalla metrica di annullamento dell’iscrizione a livello di consegna, che tiene traccia dei clic sui collegamenti all’annullamento dell’iscrizione anziché degli utenti effettivamente che l’hanno annullata.

## Percentuali di errore {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errori"
>abstract="Numero totale di errori accumulati durante le consegne ed elaborazione automatica dei mancati recapiti. Il tasso associato è il rapporto con il numero di messaggi da consegnare."

Alcuni messaggi inviati dalla piattaforma Adobe Campaign potrebbero non raggiungere la destinazione. Può verificarsi quando l’indirizzo utente o il telefono ha errori di battitura, se il destinatario ha cambiato il proprio indirizzo e-mail o se la casella di posta è piena. Se non è possibile inviare un messaggio a un profilo, il server remoto invia automaticamente un messaggio di errore ad Adobe Campaign. Questo errore consente di determinare se l’indirizzo e-mail, il numero di telefono o il dispositivo devono essere messi in quarantena.

Controlla e aggiorna regolarmente il database e assicurati che tutti i profili siano attivi e reali. Gli errori di consegna possono essere temporanei o permanenti, soft o hard bounce, a seconda del motivo per cui il messaggio non è stato consegnato.

L&#39;indicatore **Errori** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di errori rispetto al numero totale di messaggi da consegnare.

* Numero totale di errori accumulati durante le consegne ed elaborazione automatica dei messaggi restituiti.

## Messaggio inviato {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Inviato"
>abstract="Questa metrica mostra, per il canale di direct mail, la somma di tutti i messaggi inviati e la percentuale di messaggi inviati al provider, rispetto al numero totale di messaggi preparati durante la fase di preparazione della consegna."

Durante la fase di preparazione, viene generato il file di estrazione della direct mailing, ma le informazioni relative ai destinatari (registri di consegna) non vengono aggiornate. Lo stato di una consegna passa da In sospeso a Inviato quando l’utente di Campaign conferma l’invio della consegna. Quindi la consegna viene impostata su Completata.

Non può mai essere il 100% dei messaggi inviati rispetto al totale dei messaggi preparati, in quanto alcuni indirizzi possono essere mancanti o incompleti.

L&#39;indicatore **Inviato** mostra i KPI seguenti per il canale direct mailing:

* Percentuale del numero di messaggi inviati rispetto al numero totale di messaggi preparati.

* Somma di tutti i messaggi inviati.