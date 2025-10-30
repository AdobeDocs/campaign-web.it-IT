---
title: Gestione del fuso orario
description: Scopri come l’interfaccia utente web di Adobe Campaign visualizza i valori di data e ora in base ai fusi orari di browser, operatori, flussi di lavoro e server.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 3%

---

# Gestione del fuso orario {#timezone-management}

Nell&#39;interfaccia utente di Adobe Campaign Web vengono visualizzati tutti i valori di data e ora in base al **fuso orario locale del browser Web dell&#39;utente**. Questo comportamento può causare differenze nel confronto dei timestamp tra l’interfaccia utente web e la console client.

In questa sezione vengono illustrate le differenze previste tra i fusi orari **Interfaccia utente Web**, **Console client** e **Esecuzione flusso di lavoro**.

>[!NOTE]
>
>Nessun dato archiviato sul server viene modificato. Solo la visualizzazione nell’interfaccia cambia.

## Concetti chiave

* **Fuso orario del server**: il fuso orario del server corrisponde a quello configurato nel sistema operativo del server. Tutti i timestamp vengono memorizzati internamente in UTC sul server.

* **Comportamento console client**: la console client visualizza i timestamp utilizzando il fuso orario dell&#39;operatore **operator**, definito nelle impostazioni dell&#39;operatore. Per impostazione predefinita, corrisponde al fuso orario del server **&#x200B;**.

* **Comportamento interfaccia Web**: l&#39;interfaccia utente Web visualizza i timestamp utilizzando il fuso orario locale del browser **&#x200B;**. Quando un utente modifica il browser o il fuso orario del sistema, i valori di data/ora visualizzati vengono aggiornati automaticamente.

* **Comportamento del flusso di lavoro**: i flussi di lavoro interpretano le marche temporali locali in base al fuso orario configurato del **flusso di lavoro**. Se non viene specificato, per impostazione predefinita viene utilizzato il fuso orario del server **1&rbrace;.**

## Esempio

| Interfaccia | Fuso orario utilizzato | Esempio di visualizzazione |
|------------|----------------|-----------------|
| Console client | Operatore (predefinito = server) | `2025-10-20 14:00:00` |
| Interfaccia utente web | Fuso orario locale del browser | `2025-10-20 21:00:00` (per browser in UTC +7) |

In questo esempio, entrambe le interfacce fanno riferimento allo stesso timestamp UTC sottostante, ma ciascuna di esse lo esegue utilizzando un fuso orario diverso.

## Impatto

Le differenze nei tempi di visualizzazione possono essere visualizzate in:

* Campi profilo o dati contenenti `datetime` valori
* Registri di consegna o date di contatto
* Esecuzione del flusso di lavoro e timestamp di importazione

I dati sottostanti rimangono identici. La differenza è solo nel **rendering**.

>[!NOTE]
>
>Se utenti di più aree geografiche collaborano alla stessa istanza, possono verificarsi discrepanze apparenti tra l’interfaccia utente web e le marche temporali della console.

## Consigli

Per allineare i valori di visualizzazione tra le interfacce, è possibile:

* Modifica il **fuso orario del browser** in modo che corrisponda al **fuso orario dell&#39;operatore o del server**.
* Durante l’esportazione dei dati (le esportazioni utilizzano UTC), assicurati che la conversione sia coerente negli strumenti di reporting.
* Durante la progettazione dei flussi di lavoro, imposta in modo esplicito il **fuso orario del flusso di lavoro** nelle proprietà dell&#39;attività per ottenere un comportamento prevedibile di pianificazione e importazione.
* Comunicare agli utenti aziendali che le differenze di marca temporale tra le visualizzazioni Interfaccia utente Web e Console client sono **normali e previste**.
