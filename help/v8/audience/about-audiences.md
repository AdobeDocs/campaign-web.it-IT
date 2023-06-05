---
audience: end-user
title: Introduzione ai tipi di pubblico
description: Scopri come utilizzare i tipi di pubblico nell’interfaccia utente di Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 3ebe92659916cf2fa4cacb8d28b79d7b6d5359f3
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 31%

---


# Introduzione ai tipi di pubblico {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


Il pubblico è il target principale della consegna: i destinatari che ricevono i messaggi. Il tipo di pubblico dipende dalla mappatura target definita nel modello di consegna. Scopri cos’è un modello di consegna [in questa sezione](../msg/delivery-template.md).

Per definire la popolazione del pubblico, puoi:

* Seleziona un pubblico esistente, creato come elenco nella console client. [Ulteriori informazioni](add-audience.md)
* Seleziona un pubblico di Adobe Experience Platform. [Ulteriori informazioni](aep-audience.md)
* Crea un nuovo pubblico con il generatore di regole definendo e combinando criteri di filtro. [Ulteriori informazioni](segment-builder.md)
* Utilizza un pubblico da un file esterno: questa opzione è disponibile solo per le consegne e-mail autonome e non può essere utilizzata nelle consegne delle campagne. [Ulteriori informazioni](file-audience.md)

Quando si inviano messaggi nel contesto di un flusso di lavoro di una campagna, il pubblico viene definito in un **Read audience** attività del flusso di lavoro. In questo contesto, non è possibile caricare un pubblico da un file per una consegna e-mail e il pubblico è definito solo in questa attività dedicata. Scopri come definire il pubblico della consegna in un flusso di lavoro della campagna [in questa sezione](../workflows/orchestrate-activities.md).

Inoltre, puoi definire dei gruppi di controllo per evitare di inviare messaggi a una parte del pubblico, in modo da misurare l’impatto delle campagne. [Ulteriori informazioni](control-group.md)

![](assets/about-audience.png)

