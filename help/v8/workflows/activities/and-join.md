---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro AND-join
description: Scopri come utilizzare l’attività del flusso di lavoro AND-join
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 4%

---


# Attività AND-join {#join}

Il **And-join** attività consente di sincronizzare più rami di esecuzione di un flusso di lavoro.

L’attività AND-join attiva solo la relativa transizione in uscita dopo che tutte le transizioni in entrata vengono attivate, in altre parole, dopo che tutte le attività precedenti sono state completate.

Per configurare il **Unione AND** attività:

1. Aggiungi più attività come **Combina** attività per formare almeno due rami di esecuzione diversi.
1. Aggiungi un **Unione AND** ad uno qualsiasi dei rami.
1. In **Opzioni di unione** , controlla tutte le attività precedenti a cui desideri partecipare.
1. Seleziona la **Set primario** da mantenere nella transizione in uscita.
