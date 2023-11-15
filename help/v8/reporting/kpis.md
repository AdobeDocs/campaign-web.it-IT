---
title: Indicatori chiave di performance
description: Scopri come comprendere gli indicatori chiave di performance
badge: label="Beta"
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: 3c6d086c1941b5f2e29b2eb18f58ab1fc541464a
workflow-type: ht
source-wordcount: '936'
ht-degree: 100%

---

# Indicatori chiave di performance {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicatori chiave di performance"
>abstract="La sezione **Indicatori chiave di performance** consente di verificare l’efficacia della piattaforma tramite KPI comuni."

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI spam"

Passa alla pagina Home per verificare gli indicatori chiave di performance per la piattaforma. Questi indicatori mostrano il numero e la percentuale di messaggi consegnati, aperti, su cui è stato fatto clic, di annullamento degli abbonamenti e le percentuali di errori.

Per impostazione predefinita, le metriche sono calcolate per le consegne inviate nei 7 giorni precedenti. Puoi modificare il periodo dall’elenco a discesa nella sezione in alto a destra della scheda. Sono esclusi i messaggi inviati ai profili di test.

Puoi selezionare il canale da visualizzare. Per impostazione predefinita, questi indicatori riflettono le metriche per il canale e-mail.

![](assets/kpi.png)

## Messaggio consegnato {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Consegnati"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti i messaggi elaborati e la percentuale di messaggi consegnati correttamente rispetto al numero totale di messaggi inviati."

Il numero di messaggi consegnati riflette la percentuale di recapitabilità. Non può mai essere pari al 100% per i seguenti motivi: alcuni indirizzi o numeri di telefono possono essere errati, i filtri anti-spam dei provider di posta elettronica potrebbero rifiutare i messaggi oppure possono verificarsi problemi di recapitabilità.

L’indicatore **Consegnato** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di messaggi consegnati correttamente rispetto al numero totale di messaggi inviati.

* Somma di tutti i messaggi elaborati correttamente.

In Adobe Campaign, la regola per contrassegnare un messaggio come “Consegnato” è:

Numero di messaggi per i quali il campo “Indirizzo seed” è uguale a “No” e con uno stato uguale a “Considerato dal fornitore di servizi” (per gli SMS) o “Inviato” (per le e-mail) o “Ricevuto su dispositivo mobile” (per le notifiche push).


## Aperture totali {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aperture"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti i messaggi aperti e la relativa percentuale rispetto al numero totale di messaggi consegnati correttamente."

Il totale delle aperture è calcolato mediante tracciamento del numero totale di volte che un messaggio viene aperto, indipendentemente dal numero di singoli destinatari da cui tali aperture vengono generate. Questo indicatore è disponibile solo per le e-mail.

L’indicatore **Aperture** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di messaggi aperti rispetto al numero totale di messaggi consegnati correttamente.

* Somma di tutti i messaggi aperti per canale.

Adobe Campaign rileva le aperture dei messaggi quando il destinatario scarica le immagini nell’e-mail. Le e-mail HTML e Multipart/Alternative includono un’immagine a 0 pixel, che consente di rilevare quali messaggi sono stati aperti. Poiché i messaggi in formato di testo non includono immagini, è impossibile rilevare se sono stati aperti o meno. I valori calcolati in base alle aperture dei messaggi sono sempre delle stime, a causa del margine di errore legato alla visualizzazione delle immagini.



## Tasso di click-through {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clic"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti gli URL su cui è stato fatto clic nei messaggi e la percentuale di clic rispetto al numero totale di messaggi consegnati correttamente."

Gli URL possono essere aggiunti al contenuto del messaggio per reindirizzare i destinatari a una pagina specifica. La percentuale di click-through misura il numero e il tasso di destinatari che hanno fatto clic su un collegamento nel messaggio.

L’indicatore **Clic** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di clic rispetto al numero totale di messaggi consegnati con successo.

* Numero di persone distinte che hanno fatto clic almeno una volta in una consegna. Sono esclusi i collegamenti di annullamento dell’abbonamento e i collegamenti alla pagina mirror dell’e-mail.

Queste metriche si basano sulla tabella di tracciamento consolidata (`nms:trackingStats`). Questa tabella aggregata viene utilizzata per motivi di prestazioni quando si visualizzano i report al posto della tabella dei registri di tracciamento dei destinatari (`nms:trackingLogRcp`) e non viene calcolata in tempo reale. La tabella viene generata pochi minuti dopo il recupero dei registri di tracciamento.


## Percentuali di annullamento dell’abbonamento {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Annullamenti dell’iscrizione"
>abstract="Questa metrica mostra, per il canale selezionato, la somma di tutti gli annullamenti di iscrizione a un servizio e la relativa percentuale rispetto al numero totale di messaggi consegnati correttamente."

>[!NOTE]
>
> I KPI per l’iscrizione e l’annullamento dell’iscrizione variano in base al tipo di servizio. Ad esempio, le iscrizioni e gli annullamenti di iscrizioni alle e-mail comprendono tutti i servizi relativi alle e-mail, sia che derivino da azioni manuali che da moduli web. È importante distinguere questo approccio dalla metrica di annullamento dell’iscrizione a livello di consegna, che tiene traccia dei clic sui collegamenti all’annullamento dell’iscrizione anziché degli utenti effettivamente che l’hanno annullata.

I destinatari devono essere in grado di ricorrere alla funzione di rinuncia alla ricezione di e-mail e SMS tramite un collegamento dedicato di annullamento dell’abbonamento nel contenuto dell’e-mail o rispondendo INTERROMPI a un SMS.

L’indicatore **Annullamenti dell’abbonamento** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di annullamenti di abbonamento rispetto al numero totale di messaggi consegnati correttamente.

* La somma di tutti i clic su un collegamento di annullamento dell’abbonamento, ovvero con una categoria URL equivalente a “Rinuncia”.


## Percentuali di errore {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errori"
>abstract="Numero totale di errori accumulati durante le consegne ed elaborazione automatica dei mancati recapiti. Il tasso associato è il rapporto con il numero di messaggi da consegnare."

Alcuni messaggi inviati dalla piattaforma Adobe Campaign potrebbero non raggiungere la destinazione. Ciò può verificarsi quando l’indirizzo o il numero di telefono dell’utente contiene errori di ortografici, oppure se il destinatario ha cambiato il proprio indirizzo e-mail o se la cassetta postale è piena. Se non è possibile inviare un messaggio a un profilo, il server remoto invia automaticamente un messaggio di errore ad Adobe Campaign. Questo errore consente di determinare se l’indirizzo e-mail, il numero di telefono o il dispositivo devono essere messi in quarantena.

Di conseguenza, devi sempre verificare e aggiornare il database e assicurarti che tutti i profili siano attivi e reali. Gli errori di consegna possono essere temporanei o permanenti, con mancati recapiti permanenti o non permanenti, a seconda del motivo per cui il messaggio non è stato consegnato.

L’indicatore **Errori** mostra i KPI seguenti per ogni canale:

* Percentuale del numero di errori rispetto al numero totale di messaggi da consegnare.

* Numero totale di errori accumulati durante le consegne ed elaborazione automatica dei messaggi restituiti.
