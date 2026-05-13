---
audience: end-user
title: Creare un pubblico una tantum per una consegna
description: Scopri come creare un pubblico una tantum per una consegna.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
TQID: https://experienceleague.adobe.com/96G-USwsSAOJUSeXTpgpCTgeCNfwgIBHorvcxvObcuw
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 33%

---

# Creare un pubblico una tantum {#one-time}

Questa sezione spiega come creare un pubblico durante la creazione di una nuova consegna. In questo scenario, il targeting dei profili inclusi nel pubblico di consegna viene eseguito interrogando il database utilizzando il modellatore di query. Il pubblico risultante viene utilizzato una sola volta per questa consegna e non viene salvato nell’elenco dei tipi di pubblico.

Quando definisci il target principale di una consegna, puoi anche:
* [Selezionare un pubblico esistente](add-audience.md) dall’elenco **[!UICONTROL Tipi di pubblico]**.
* [Caricare un pubblico da un file esterno](file-audience.md) (solo per e-mail).

Per creare un nuovo pubblico una tantum per una consegna, segui questi passaggi:

1. Nella sezione **Pubblico** dell’assistente alla creazione di consegne, fai clic sul pulsante **[!UICONTROL Seleziona pubblico]**.

   [Schermata che mostra la sezione Pubblico dell’assistente per la creazione della consegna con il pulsante Seleziona pubblico evidenziato](assets/segment-builder0.png){zoomable="yes"}

1. Seleziona **Crea** per aprire il modellatore di query. Il modellatore di query ti consente di definire la popolazione target filtrando i dati contenuti nel database. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md).

   [Schermata che mostra l’interfaccia di Query Modeler](assets/query-modeler.png){zoomable="yes"}

1. Quando la query è pronta, fai clic su **Conferma** per utilizzare il pubblico risultante come destinazione principale della consegna.

   Puoi anche impostare un gruppo di controllo per misurare l’impatto delle campagne. Il gruppo di controllo non riceve il messaggio. Ciò ti consente di confrontare il comportamento della popolazione che ha ricevuto il messaggio con il comportamento dei contatti che non lo hanno fatto. [Ulteriori informazioni](control-group.md).