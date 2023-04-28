---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: d7e19b2d8730cacbbff1ad42f1956b32c84a309a
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 94%

---


# Principi chiave per la creazione di flussi di lavoro {#gs-workflow-creation}

contenuto TBD

Un flusso di lavoro è una definizione di un processo, cioè del diagramma del flusso di lavoro, che è una rappresentazione di ciò che dovrebbe accadere. Un flusso di lavoro è anche un’istanza di questo processo, ovvero di un’istanza del flusso di lavoro, che è una rappresentazione di ciò che sta effettivamente accadendo.

Il modello di flusso di lavoro descrive le varie attività da eseguire e il modo in cui vengono collegate tra loro. I modelli di attività sono denominati attività e sono rappresentati da icone. Sono collegati tra loro da transizioni.

schermata TBD

## Cosa c’è all&#39;interno di un flusso di lavoro?

Ogni flusso di lavoro contiene:

* **Attività**: un’attività descrive un modello di attività. Le varie attività disponibili sono rappresentate nel diagramma da icone. Ogni tipo ha proprietà comuni e proprietà specifiche.

   In un diagramma del flusso di lavoro, una determinata attività può produrre più attività, in particolare in presenza di un ciclo o di azioni ricorrenti.

* **Transizioni**: le transizioni consentono di collegare le attività e definirne la sequenza. Una transizione collega un’attività di origine a un’attività di destinazione.

* **Tabelle di lavoro**: la tabella di lavoro contiene tutte le informazioni riportate dalla transizione. Ogni flusso di lavoro utilizza diverse tabelle di lavoro. I dati trasmessi in queste tabelle possono essere accelerati e utilizzati per l’intero ciclo di vita del flusso di lavoro, purché non vengano eliminati. In effetti, le tabelle non necessarie vengono eliminate ogni volta che il flusso di lavoro viene passivato e possibilmente durante l’esecuzione dei flussi di lavoro più grandi per evitare di sovraccaricare il server.

## Flussi di lavoro autonomi e di campagna

I flussi di lavoro possono essere creati sia come flussi di lavoro autonomi, sia all’interno di una campagna.

TBD: specificità dei flussi di lavoro autonomi e di campagna.

## Passaggi principali per creare un flusso di lavoro

I passaggi principali per creare i flussi di lavoro sono i seguenti:

TBD: grafico che mostra l’intero processo con spiegazione e riferimento alle pagine della documentazione

crea e definisci proprietà > orchestra attività nell’area di lavoro > configura impostazioni se necessario > avvia l’esecuzione e monitora