---
title: Aggiungere filtri personalizzati
description: Scopri come aggiungere filtri personalizzati come campi di accesso rapido nel riquadro dei filtri di una visualizzazione a elenco.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Aggiungere filtri personalizzati {#custom-filters}

La sezione **[!UICONTROL Configurazione elenco inventario]** > **[!UICONTROL Filtri personalizzati]** consente di scegliere gli attributi da visualizzare come campi di accesso rapido nel [riquadro filtri](../query/filter.md) della visualizzazione elenco di uno schema, sopra il generatore di regole **[!UICONTROL Filtri avanzati]**.

Per ulteriori informazioni sulla schermata di definizione dello schermo e su come accedervi, fare riferimento alla sezione [Accedere alla definizione dello schermo](schemas-browse-access.md#screen-def).

## Aggiungere filtri personalizzati {#add}

1. Accedi al menu **[!UICONTROL Schemi]** e individua gli schemi modificabili utilizzando i filtri.

1. Selezionare il nome dello schema nell&#39;elenco per aprirlo e fare clic sul pulsante **[!UICONTROL Screen edition]** nella visualizzazione dei dettagli dello schema per accedere alla definizione dello schermo.

1. Vai alla sezione **[!UICONTROL Configurazione elenco inventario]** e fai clic sull&#39;icona dei puntini di sospensione sopra la tabella **[!UICONTROL Filtri personalizzati]**, quindi scegli **[!UICONTROL Seleziona attributi]**.

   ![Selezione filtri personalizzati](assets/schemas-custom-filters1.png)

1. Seleziona uno o più attributi e conferma.

   Puoi selezionare:

   * Attributo diretto dello schema, ad esempio un codice o una categoria.
   * Un attributo di collegamento, ad esempio un marchio collegato a un prodotto. In questo caso, il filtro utilizza un selettore di ricerca limitato allo schema collegato.
   * Un sottoattributo di un collegamento, ad esempio il nome completo di una cartella collegata o l’e-mail di un destinatario collegato.

   ![Selezione attributi che mostra gli attributi diretti e gli attributi secondari del collegamento](assets/schemas-custom-filters2.png)

1. Fai clic su **[!UICONTROL Salva]**. Puoi riordinare i filtri personalizzati utilizzando le frecce su e giù o trascinandoli, e rimuovere un filtro utilizzando l’icona del cestino sulla riga.

1. Individuare l&#39;elenco dei record per lo schema e aprire il riquadro Filtri. Gli attributi selezionati vengono visualizzati come **[!UICONTROL Filtri personalizzati]**, sopra il generatore di regole **[!UICONTROL Filtri avanzati]**.

   ![Filtri personalizzati visualizzati nel riquadro dei filtri](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Un filtro personalizzato basato su un attributo di data o data e ora viene visualizzato come selettore di intervalli di date.

1. Inserisci o seleziona un valore in uno dei filtri personalizzati per perfezionare l’elenco.

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->