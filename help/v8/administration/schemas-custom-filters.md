---
title: Aggiungere filtri personalizzati
description: Scopri come aggiungere filtri personalizzati come campi di accesso rapido nel riquadro dei filtri di una visualizzazione a elenco.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 3%

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

1. Fai clic su **[!UICONTROL Salva]**. Puoi riordinare i filtri personalizzati utilizzando le frecce su e giù o trascinandoli. Per rimuovere un filtro, fare clic sull&#39;icona con i puntini di sospensione nella riga corrispondente e selezionare **[!UICONTROL Elimina]**.

1. Individuare l&#39;elenco dei record per lo schema e aprire il riquadro Filtri. Gli attributi selezionati vengono visualizzati come **[!UICONTROL Filtri personalizzati]**, sopra il generatore di regole **[!UICONTROL Filtri avanzati]**.

   ![Filtri personalizzati visualizzati nel riquadro dei filtri](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Un filtro personalizzato basato su un attributo di data o data e ora viene visualizzato come selettore di intervalli di date.

1. Inserisci o seleziona un valore in uno dei filtri personalizzati per perfezionare l’elenco.

## Limita i valori per un filtro personalizzato di tipo collegamento {#settings}

Per un filtro personalizzato basato su un attributo di collegamento, puoi limitare i valori disponibili nel selettore.

>[!NOTE]
>
>L&#39;opzione **[!UICONTROL Modifica]** descritta di seguito è disponibile solo per i filtri personalizzati basati su un attributo di collegamento. I filtri personalizzati basati su altri tipi di attributi possono essere riordinati o rimossi solo.

1. Nella riga di un filtro personalizzato di tipo collegamento, fai clic sull&#39;icona dei puntini di sospensione e seleziona **[!UICONTROL Modifica]**.

   ![Modifica opzione su un filtro personalizzato di tipo collegamento](assets/schemas-custom-filters4.png)

1. Nella scheda **[!UICONTROL Impostazioni filtro]**, fare clic su **[!UICONTROL Modifica filtro]** e utilizzare il modellatore di query per definire una condizione che limita i valori disponibili nel selettore. Ad esempio, limita un filtro di consegna alle consegne che utilizzano il canale e-mail.

   ![Scheda Impostazioni filtro nella finestra di dialogo Impostazioni collegamento](assets/schemas-custom-filters5.png)

1. Conferma le modifiche.
