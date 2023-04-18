---
audience: end-user
title: Creare flussi di lavoro con Adobe Campaign Web
description: Scopri come creare flussi di lavoro con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 9a4ca68d475cfbbcccb7a5b0d84f841589824288
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 6%

---


# Principi fondamentali per la creazione di flussi di lavoro {#gs-workflow-creation}

Un flusso di lavoro è una definizione del processo: il diagramma del flusso di lavoro, che rappresenta ciò che dovrebbe accadere. Un flusso di lavoro è anche un’istanza di questo processo: un’istanza di flusso di lavoro, che è una rappresentazione di ciò che sta effettivamente accadendo.

Il modello di flusso di lavoro descrive le varie attività da eseguire e il modo in cui vengono collegate tra loro. I modelli di attività sono denominati attività e sono rappresentati da icone. Sono collegate tra loro da transizioni.

schermata TBD

## Cosa c&#39;è all&#39;interno di un flusso di lavoro?

Ogni flusso di lavoro contiene:

* **Attività**: Un’attività descrive un modello di attività. Le varie attività disponibili sono rappresentate nel diagramma da icone. Ogni tipo ha proprietà comuni e proprietà specifiche.

   In un diagramma di flusso di lavoro, una determinata attività può produrre più attività, in particolare in presenza di un ciclo o di azioni ricorrenti.

* **Transizioni**: Le transizioni ti consentono di collegare le attività e definirne la sequenza. Una transizione collega un’attività sorgente a un’attività di destinazione.

* **Tabelle di lavoro**: La tabella di lavoro contiene tutte le informazioni riportate dalla transizione. Ogni flusso di lavoro utilizza diverse tabelle di lavoro. I dati trasmessi in queste tabelle possono essere accelerati e utilizzati per l’intero ciclo di vita del flusso di lavoro, purché non vengano eliminati. In effetti, le tabelle non necessarie vengono eliminate ogni volta che il flusso di lavoro viene passivato e possibilmente durante l’esecuzione dei flussi di lavoro più grandi per evitare di sovraccaricare il server.

## Flussi di lavoro autonomi e per campagne

I flussi di lavoro possono essere creati sia come flussi di lavoro autonomi, sia all’interno di una campagna.

Da definire: specifica le specificità tra flussi di lavoro autonomi e per campagne.

## Passaggi principali per creare un flusso di lavoro

I passaggi principali per creare flussi di lavoro sono i seguenti:

Da definire: grafico che mostra l&#39;intero processo con spiegazione e riferimento alle pagine della documentazione