---
audience: end-user
title: Creare un pubblico una tantum per una consegna
description: Scopri come creare un pubblico una tantum per una consegna.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 32%

---

# Creare un pubblico una tantum {#one-time}

Questa sezione spiega come creare un pubblico durante la creazione di una nuova consegna. In questo scenario, il targeting dei profili inclusi nel pubblico di consegna viene eseguito interrogando il database utilizzando il modellatore di query. Il pubblico risultante viene utilizzato una sola volta per questa consegna e non viene salvato nell’elenco dei tipi di pubblico.

Quando definisci il target principale di una consegna, puoi anche:
* [Selezionare un pubblico esistente](add-audience.md) dall’elenco **[!UICONTROL Tipi di pubblico]**.
* [Caricare un pubblico da un file esterno](file-audience.md) (solo per e-mail).

Per creare un nuovo pubblico una tantum per una consegna, segui questi passaggi:

1. Nella sezione **Pubblico** dell’assistente alla creazione di consegne, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   [Schermata che mostra la sezione Pubblico dell&#39;assistente per la creazione della consegna con il pulsante Seleziona pubblico evidenziato](assets/segment-builder0.png){zoomable="yes"}

1. Seleziona **Crea** per aprire il modellatore di query. Il modellatore di query ti consente di definire la popolazione target filtrando i dati contenuti nel database. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md).

   [Schermata che mostra l&#39;interfaccia di Query Modeler](assets/query-modeler.png){zoomable="yes"}

1. Quando la query è pronta, fai clic su **Conferma** per utilizzare il pubblico risultante come destinazione principale della consegna.

   Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceve il messaggio. Ciò ti consente di confrontare il comportamento della popolazione che ha ricevuto il messaggio con il comportamento dei contatti che non lo hanno fatto. [Ulteriori informazioni](control-group.md).