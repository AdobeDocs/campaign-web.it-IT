---
audience: end-user
title: Monitorare i registri di consegna
description: Documentazione Web di Campaign v8
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 13765b02288ec4682c5d55603c68f8ea1a5758f8
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 21%

---

# Monitorare i registri di consegna {#delivery-logs}

>[!NOTE]
>
>Questa documentazione è in fase di costruzione e viene aggiornata frequentemente. La versione finale di questo contenuto sarà pronta a gennaio 2023.

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Log di consegna"
>abstract="TBC"

Dopo aver preparato e inviato un’e-mail, i registri di consegna ti consentono di verificare che non vi siano errori. Questi registri sono accessibili direttamente dal dashboard dei messaggi. Mostrano i dettagli dell’invio, quale target è stato escluso e perché, nonché le informazioni di tracciamento come aperture e clic.

Per visualizzare i registri, accedi al dashboard di consegna e fai clic su **Registri** pulsante .

Sono disponibili diverse schede:

## Registri

La **Registri** contiene tutti i messaggi relativi alla consegna e alle bozze. Le icone specifiche consentono di identificare errori o avvisi.

Vengono elencati tutti i passaggi, gli avvisi e gli errori di convalida. Le icone colorate mostrano il tipo di messaggio:

* L’icona grigia indica un messaggio informativo.
* L’icona gialla indica un errore di elaborazione non critico.
* L’icona rossa indica un errore critico che impedisce l’invio della consegna.

![](assets/logs.png)

## Consegne

La **Consegne** tab offre una cronologia di ogni occorrenza della consegna. L’elenco dei messaggi inviati e i relativi stati sono archiviati qui. Consente di visualizzare lo stato di consegna per ciascun destinatario.

![](assets/logs2.png)

## Esclusioni

La **Log di esclusione** La scheda elenca tutti i messaggi che sono stati esclusi dal target inviato e specifica il motivo dell’errore di invio.

![](assets/logs3.png)

## Cause di esclusione

La **Cause di esclusione** visualizza il volume (in numero di messaggi) dei messaggi esclusi dall’invio del target.

![](assets/logs4.png)

## URL tracciati

La **URL tracciati** la scheda raggruppa gli URL contenuti nel messaggio inviato, tra cui il loro tipo di URL e l’URL di origine.

![](assets/logs5.png)

## Tracciamento

La **Tracking** elenca la cronologia di tracciamento per la consegna. In questa scheda vengono visualizzati i dati di tracciamento per i messaggi inviati, ovvero tutti gli URL soggetti al tracciamento da parte di Adobe Campaign.

>[!NOTE]
>
>Se il tracciamento non è abilitato per una consegna, questa scheda non viene visualizzata.

![](assets/logs6.png)
