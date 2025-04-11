---
audience: end-user
title: Utilizzare le cartelle
description: Scopri come gestire una cartella in Adobe Campaign
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 25%

---

# Utilizzare le cartelle {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Proprietà cartella"
>abstract="Proprietà cartella"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Sicurezza cartella"
>abstract="Sicurezza cartella"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Restrizioni cartella"
>abstract="Restrizioni cartella"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Pianificazione cartella"
>abstract="Pianificazione cartella"

## Informazioni sulle cartelle {#about-folders}

In Adobe Campaign le cartelle sono oggetti che consentono di organizzare i componenti e i dati.

È possibile creare, rinominare, riordinare e spostare cartelle nella struttura di navigazione. Puoi anche eliminarli in base ai tuoi diritti.

![Interfaccia delle cartelle con l&#39;organizzazione delle cartelle](assets/folders.png){zoomable="yes"}

Puoi impostare un tipo di cartella. Ad esempio, una cartella di consegne. L’icona della cartella cambia in base al tipo.

## Creare una nuova cartella {#create-a-folder}

Per creare una nuova cartella nell’interfaccia utente di Adobe Campaign Web, segui questi passaggi:

1. In **[!UICONTROL Explorer]**, vai alla cartella in cui desideri creare la nuova cartella. Nel menu **[!UICONTROL ...]**, seleziona **[!UICONTROL Crea nuova cartella]**.

![Opzione Crea nuova cartella nel menu Esplora risorse](assets/folder_create.png){zoomable="yes"}

Quando si crea una nuova cartella, per impostazione predefinita il tipo di cartella corrisponde al tipo della cartella padre. In questo esempio viene creata una cartella nella cartella **[!UICONTROL Deliveries]**.

![Nuova cartella creata nella cartella Consegne](assets/folder_new.png){zoomable="yes"}

1. Modifica il tipo di cartella facendo clic sull’icona del tipo di cartella, se necessario, e seleziona il tipo desiderato dall’elenco mostrato di seguito:

![Interfaccia di selezione del tipo di cartella](assets/folder_type.png){zoomable="yes"}

Impostare il tipo di cartella facendo clic sul pulsante **[!UICONTROL Conferma]**.

Se si desidera creare una cartella senza un tipo specifico, selezionare il tipo **[!UICONTROL Cartella generica]**.

È, inoltre, possibile [creare e gestire cartelle nella console di Adobe Campaign](https://experienceleague.adobe.com/it/docs/campaign/campaign-v8/config/configuration/folders-and-views).

## Riordinare le cartelle {#reorder-folders}

Puoi riordinare le cartelle in base alle tue esigenze. A tale scopo, fare clic su **[!UICONTROL Riordina cartelle]**, come illustrato di seguito.

In questo esempio, la cartella **Deliveries** contiene quattro sottocartelle.

![Riordina l&#39;interfaccia delle cartelle con la gerarchia di cartelle](assets/folder-reorder.png){zoomable="yes"}

È possibile modificare l&#39;ordine delle cartelle **trascinando** o utilizzando **frecce verso l&#39;alto e verso il basso**.

![Funzionalità di trascinamento per il riordinamento delle cartelle](assets/folder-draganddrop.png){zoomable="yes"}

## Eliminare una cartella {#delete-a-folder}

>[!CAUTION]
>
>Durante l’eliminazione di una cartella, vengono eliminati anche tutti i dati memorizzati al suo interno.

Per eliminare una cartella, selezionarla nella struttura **[!UICONTROL Explorer]** e fare clic sul menu **[!UICONTROL ...]**. Scegli **[!UICONTROL Elimina cartella]**.

![Elimina cartella dal menu Esplora risorse](assets/folder_delete.png){zoomable="yes"}

## Distribuzione dei valori in una cartella {#distribution-values-folder}

La distribuzione dei valori consente di comprendere la percentuale di un valore in una colonna all&#39;interno di una tabella.

Per visualizzare la distribuzione dei valori in una cartella, procedere come spiegato di seguito.

Ad esempio, tra le consegne, potrebbe essere utile conoscere la distribuzione dei valori nella colonna **Canale**.

Per ottenere queste informazioni, vai alla cartella **[!UICONTROL Consegne]** e fai clic sull&#39;icona **[!UICONTROL Configura colonne]**.

Nella finestra **[!UICONTROL Configura colonne]**, fai clic sull&#39;icona **[!UICONTROL Informazioni]** relativa alla colonna da analizzare. Quindi, fare clic sul pulsante **[!UICONTROL Distribuzione dei valori]**.

![Interfaccia di distribuzione dei valori per le consegne](assets/values_deliveries.png){zoomable="yes"}

Nella colonna **[!UICONTROL Canale]** verrà visualizzata la percentuale di valori.

![Distribuzione percentuale dei valori nella colonna Canale](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
>Per le colonne con molti valori, vengono visualizzati solo i primi venti valori. Una notifica **[!UICONTROL Caricamento parziale]** ti avvisa.

Puoi anche visualizzare la distribuzione dei valori per un collegamento.

Nell’elenco degli attributi, fare clic sul pulsante **+** accanto al collegamento desiderato, come illustrato di seguito. Questo aggiunge il collegamento alle **[!UICONTROL colonne di output]**. È ora possibile accedere all&#39;icona **[!UICONTROL Informazioni]** per visualizzare la distribuzione dei relativi valori. Se non si desidera mantenere il collegamento nelle **[!UICONTROL colonne di output]**, fare clic sul pulsante **[!UICONTROL Annulla]**.

![Distribuzione di valori per un collegamento nelle colonne di output](assets/values_link.png){zoomable="yes"}

È inoltre possibile visualizzare la distribuzione dei valori in un modellatore di query. [Ulteriori informazioni](../query/build-query.md#distribution-of-values-in-a-query).

### Filtrare i valori {#filter-values}

Utilizzando i **[!UICONTROL Filtri avanzati]** nella finestra di distribuzione dei valori, è possibile filtrare i risultati in base a condizioni specificate.

Nell&#39;esempio dell&#39;elenco di consegna riportato sopra, che mostra la distribuzione per canale, è possibile filtrarla per visualizzare solo le consegne con stato **Completato**.

![Filtri avanzati applicati alla distribuzione dei valori](assets/values_filter.png){zoomable="yes"}