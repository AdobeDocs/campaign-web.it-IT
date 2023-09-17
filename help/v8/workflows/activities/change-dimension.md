---
audience: end-user
title: Utilizzare l’attività del flusso di lavoro Modifica dimensione
description: Scopri come utilizzare l’attività del flusso di lavoro Modifica dimensione
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Cambiare dimensione {#change-dimension}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generate Complement"
>abstract="TBD"
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Cambia attività dimensione"
>abstract="Questa attività ti consente di modificare la dimensione di targeting durante la creazione di un pubblico. Sposta l’asse in base al modello di dati e alla dimensione di input. Ad esempio, puoi passare dalla dimensione &quot;contratti&quot; alla dimensione &quot;clienti&quot;."


Il **Cambia dimensione** l&#39;attività è un **Targeting** attività. Questa attività ti consente di modificare la dimensione di targeting durante la creazione di un pubblico. Questa attività sposta l’asse a seconda del modello di dati e della dimensione di input. Ad esempio, puoi passare dalla dimensione &quot;contratti&quot; alla dimensione &quot;clienti&quot;.

Puoi inoltre utilizzare questa attività per definire le colonne aggiuntive della nuova destinazione e i criteri di deduplicazione dei dati.

## Configurazione

Per configurare il **Cambia dimensione** attività:

1. Aggiungi un **Cambia dimensione** al flusso di lavoro.

   ![](../assets/workflow-change-dimension.png)

1. Definisci il **Nuova dimensione di destinazione**.

Durante la modifica della dimensione vengono conservati tutti i record.