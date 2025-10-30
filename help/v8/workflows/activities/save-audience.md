---
audience: end-user
title: Utilizzare l’attività Salva pubblico nei flussi di lavoro
description: Scopri come utilizzare l’attività Fork nei flussi di lavoro
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 47%

---

# Salvare il pubblico {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Salva un pubblico"
>abstract="Utilizza questa attività per aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro. I tipi di pubblico creati vengono aggiunti all’elenco dei tipi di pubblico e sono disponibili tramite il menu **Tipi di pubblico**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Genera transizione in uscita"
>abstract="Utilizza questa opzione se desideri aggiungere una transizione dopo l’attività **Salva pubblico**."

L’attività **Salva pubblico** è un’attività di **targeting**. Questa attività consente di aggiornare un pubblico esistente o crearne uno nuovo dalla popolazione calcolata a monte in un flusso di lavoro. I tipi di pubblico creati vengono aggiunti all’elenco dei tipi di pubblico delle applicazioni e sono disponibili tramite il menu **Tipi di pubblico**.

Questa attività viene utilizzata principalmente per mantenere i gruppi di popolazione calcolati nello stesso flusso di lavoro convertendoli in tipi di pubblico riutilizzabili. Connettila ad altre attività di targeting, come a un’attività **Crea pubblico** o **Combina**.

## Configurare l’attività Salva pubblico {#save-audience-configuration}

Per configurare l’attività **Salva pubblico**, segui questi passaggi:

![Descrizione: configurazione del flusso di lavoro per l&#39;attività Save audience](../assets/workflow-save-audience.png)

1. Aggiungi un’attività **Salva pubblico** al flusso di lavoro.

1. Nel menu a discesa **Modalità**, selezionare l&#39;azione che si desidera eseguire:

   * **Crea o aggiorna un pubblico esistente**: definisci una **etichetta pubblico**. Se il pubblico esiste già, viene aggiornato; in caso contrario, viene creato un nuovo pubblico.

   * **Aggiorna un pubblico esistente**: scegli il **pubblico** da aggiornare dall&#39;elenco dei tipi di pubblico esistenti.

1. Seleziona la **modalità di aggiornamento** applicabile ai tipi di pubblico esistenti:

   * **Sostituisci il contenuto del pubblico con nuovi dati**: tutto il contenuto del pubblico viene sostituito e i vecchi dati andranno persi. Vengono conservati solo i dati della transizione in entrata dell&#39;attività **Save audience**. Questa opzione elimina il tipo di pubblico e la dimensione targeting del pubblico aggiornato.

   * **Pubblico completo con nuovi dati**: il contenuto del pubblico precedente viene mantenuto e i dati della transizione in entrata dell&#39;attività **Salva pubblico** vengono aggiunti a esso.

1. Seleziona l&#39;opzione **Genera una transizione in uscita** se desideri aggiungere una transizione dopo l&#39;attività **Salva pubblico**.

Il contenuto del pubblico salvato è quindi disponibile nella relativa visualizzazione dettagliata, accessibile dal menu **Tipi di pubblico**. Le colonne disponibili in questa visualizzazione corrispondono alle colonne della transizione in entrata dell&#39;attività **Save audience** del flusso di lavoro.

## Esempio {#save-audience-example}

L’esempio seguente illustra un semplice aggiornamento del pubblico dal targeting. Una pianificazione esegue il flusso di lavoro una volta al mese. Una query recupera tutti i profili abbonati alle diverse applicazioni disponibili. L&#39;attività **Save audience** aggiorna il pubblico rimuovendo i profili che hanno annullato l&#39;abbonamento al servizio dall&#39;ultima esecuzione del flusso di lavoro e aggiungendo i nuovi profili abbonati.