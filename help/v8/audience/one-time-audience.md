---
audience: end-user
title: Creare un pubblico una tantum per una consegna
description: Scopri come creare un pubblico una tantum per una consegna.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 85%

---

# Creare un pubblico una tantum {#one-time}

Questa sezione descrive come creare un pubblico durante la creazione di una nuova consegna. In questo caso, il targeting dei profili da includere nel pubblico di consegna viene eseguito interrogando il database con il modellatore di query.

Il pubblico risultante viene utilizzato una sola volta per questa consegna. Non viene salvato nell’elenco dei tipi di pubblico.

Quando definisci il target principale di una consegna, puoi anche:

* [Selezionare un pubblico esistente](add-audience.md) dall’elenco **[!UICONTROL Tipi di pubblico]**.
* [Caricare un pubblico da un file esterno](file-audience.md) (solo per e-mail).

Per creare un nuovo pubblico direttamente da una consegna, segui questi passaggi:

1. Nella sezione **Pubblico** dell’assistente alla creazione di consegne, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. Seleziona **Crea nuovo**. Viene visualizzato il modellatore di query. Questo consente di definire la popolazione target della consegna filtrando i dati contenuti nel database. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. Quando la query è pronta, fai clic su **Conferma** per utilizzare il pubblico come target principale della consegna.

   Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceve il messaggio. Ciò consente di confrontare il comportamento di chi ha ricevuto il messaggio con quello dei contatti che non lo hanno ricevuto. [Ulteriori informazioni](control-group.md)
