---
audience: end-user
title: Utilizzare l’attività Fine flusso di lavoro
description: Scopri come utilizzare l’attività End workflow
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 20%

---

# Fine {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Attività Fine"
>abstract="L’attività **Fine** consente di contrassegnare graficamente la fine di un flusso di lavoro. Quando è disponibile più di una transizione in entrata, utilizzare la sezione **Set da unire** per selezionare le transizioni da connettere all&#39;attività."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Set da unire"
>abstract="Controlla le attività precedenti che desideri connettere come transizioni in entrata dell&#39;attività **Fine**. Le attività selezionate sono quindi connesse alla **Fine**. Questa sezione viene visualizzata solo quando è disponibile più di una transizione in entrata per essere connessa all’attività."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Segnale esterno"
>abstract="segnaposto per la sezione sul segnale esterno nei parametri dell’attività Fine. Disponibile solo per le campagne orchestrate. NON ELIMINARE"

L&#39;attività **End** è un&#39;attività **Controllo flusso**. Consente di contrassegnare graficamente la fine di un flusso di lavoro. Questa attività è facoltativa.

L’attività supporta più transizioni in entrata quando è disponibile più di una transizione in entrata.

Nella sezione **Set per partecipare**, controllare le attività precedenti che si desidera connettere come transizioni in entrata dell&#39;attività **End**. Le attività selezionate sono quindi collegate alla **Fine** nell&#39;area di lavoro del flusso di lavoro.

![Processo di configurazione deduplicazione flusso di lavoro](../assets/workflow-end.png)
