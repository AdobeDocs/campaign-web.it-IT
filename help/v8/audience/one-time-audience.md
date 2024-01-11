---
audience: end-user
title: Creare un pubblico una tantum per una consegna
description: Scopri come creare un pubblico una tantum per una consegna.
badge: label="Beta"
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 85%

---

# Creare un pubblico una tantum per una consegna {#sone-time}

Questa sezione descrive come creare un pubblico durante la creazione di una nuova consegna. In questo caso, il target dei destinatari da includere nel pubblico di consegna è rappresentato dalla query nel database con il modellatore di query.

Il pubblico risultante viene utilizzato una sola volta per questa consegna. Non viene salvato nell’elenco dei tipi di pubblico.

Quando definisci il target principale di una consegna, puoi anche:

* [Selezionare un pubblico esistente](add-audience.md) dall’elenco **[!UICONTROL Tipi di pubblico]**.
* [Caricare un pubblico da un file esterno](file-audience.md) (solo per e-mail).

Per creare un nuovo pubblico direttamente da una consegna, segui questi passaggi:

1. Nella sezione **Pubblico** dell’assistente alla creazione di consegne, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   ![](assets/segment-builder0.png)

1. Seleziona **Crea nuovo**. Viene visualizzato il modellatore di query. Questo consente di definire la popolazione target della consegna filtrando i dati contenuti nel database. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md)

   ![](assets/segment-builder.png)

1. Quando la query è pronta, fai clic su **Conferma** per utilizzare il pubblico come target principale della consegna.

   Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceve il messaggio. Ciò consente di confrontare il comportamento di chi ha ricevuto il messaggio con quello dei contatti che non lo hanno ricevuto. [Ulteriori informazioni](control-group.md)
