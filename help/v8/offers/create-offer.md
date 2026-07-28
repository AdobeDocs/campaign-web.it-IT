---
audience: end-user
title: Creare e pubblicare un’offerta
description: Scopri come creare, configurare, approvare e distribuire un’offerta in Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 2%

---

# Creare e pubblicare un’offerta {#create-offer}

Una **offerta** è una singola proposta con un proprio periodo di idoneità, filtro di destinazione, peso e contenuto. Le offerte sono organizzate nel catalogo delle offerte tramite **categorie** e vengono presentate ai destinatari tramite uno **spazio delle offerte**.

Prima di creare un’offerta, assicurati che l’ambiente dell’offerta sia configurato e che sia pubblicato almeno uno spazio dell’offerta. Ulteriori informazioni sono disponibili in [Configurare un ambiente di offerta](offer-environment.md) e [Creare e gestire spazi di offerta](offer-space.md).

## Accedere al catalogo delle offerte {#access}

Per sfogliare e creare le offerte, seleziona **[!UICONTROL Offerte]** dalla barra di navigazione a sinistra. L’elenco mostra le offerte esistenti. Utilizza il campo di ricerca, il selettore di cartelle o [modeler di query](../query/query-modeler-overview.md) per filtrare l&#39;elenco.

![Schermata che mostra il catalogo delle offerte.](assets/offers-offer.png){zoomable="yes"}

Fai clic sul nome di un&#39;offerta per aprirla per l&#39;edizione oppure usa i tre punti accanto per **[!UICONTROL Duplicarla]** o **[!UICONTROL Eliminarla]**.

## Creare un’offerta {#create}

Per creare una nuova offerta:

1. Nell&#39;elenco delle offerte, fare clic su **[!UICONTROL Crea offerta]**.

1. Seleziona il **[!UICONTROL Modello]** da cui creare l&#39;offerta (ad esempio, un&#39;offerta vuota o un modello di offerta anonimo).

   ![Schermata che mostra la creazione dell&#39;offerta.](assets/offers-offer-1.png){zoomable="yes"}

1. Immetti un **[!UICONTROL Label]** e, facoltativamente, assegna l&#39;offerta a un operatore utilizzando **[!UICONTROL Assegnato a]** e/o immetti un **[!UICONTROL Codice offerta]**.

1. Espandi **[!UICONTROL Opzioni aggiuntive]** per modificare il **[!UICONTROL Nome interno]** generato automaticamente, seleziona la **[!UICONTROL Categoria]** in cui è memorizzata l&#39;offerta oppure aggiungi una descrizione. Questo passaggio è facoltativo.

1. Espandi **[!UICONTROL Approvazioni]** per assegnare gli approvatori ai gruppi **[!UICONTROL Approvazione idoneità]** e **[!UICONTROL Approvazione contenuto]**. Questo passaggio è facoltativo.

1. Espandi **[!UICONTROL Opzioni personalizzate]** per compilare eventuali campi aggiuntivi aggiunti dalla tua organizzazione allo schema dell&#39;offerta. I campi mostrati in questa sezione variano da un’istanza Campaign all’altra. Questo passaggio è facoltativo.

1. Fai clic su **[!UICONTROL Crea]**. Viene visualizzata la schermata completa delle impostazioni.

   ![Schermata che mostra la schermata delle impostazioni dell&#39;offerta.](assets/offers-offer-2.png){zoomable="yes"}

### Definire l’idoneità {#eligibility}

Questa sezione ti consente di controllare quando e a chi può essere presentata l’offerta. Sono disponibili le seguenti opzioni:

* **[!UICONTROL Pianificazione]** — Imposta le date di inizio e di fine tra le quali può essere presentata l&#39;offerta.

  >[!NOTE]
  >
  >Vengono prese in considerazione le intersezioni del periodo di idoneità con la categoria principale: anche se la pianificazione dell’offerta è più ampia, l’offerta viene presentata solo mentre è idonea anche la categoria principale.

* **[!UICONTROL Filtri sulla destinazione]** — Fare clic su **[!UICONTROL Crea filtro]** per aprire il generatore di regole e limitare l&#39;offerta a un pubblico specifico. Lascia il filtro vuoto per rendere l’offerta idonea per l’intero pubblico dell’ambiente. Per riutilizzare un **filtro predefinito** dichiarato a livello di piattaforma, consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}. I filtri predefiniti vengono creati dalla console client.

* **[!UICONTROL Gestione del peso dell&#39;offerta]** — Fare clic su **[!UICONTROL Visualizza peso offerta]**, quindi su **[!UICONTROL Aggiungi peso]** per influenzare la priorità dell&#39;offerta quando più offerte sono idonee contemporaneamente. Ogni peso ha una data di inizio, una data di fine e un filtro facoltativo.

>[!NOTE]
>
>Il motore di offerta ordina le offerte idonee in base al peso decrescente e restituisce per prime le proposte ponderate più alte. La logica di selezione, denominata **arbitraggio**, tiene conto anche delle regole di idoneità e dei pesi configurati per la categoria padre e per l&#39;ambiente. Ulteriori informazioni sul principio di arbitraggio sono disponibili nella [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=it){target="_blank"}.

### Definire il contenuto {#content}

Dall&#39;offerta, selezionare la scheda **[!UICONTROL Contenuto]**. Questa scheda definisce i valori che verranno esposti dalla funzione di rendering.

1. Compila gli attributi predefiniti: **[!UICONTROL Titolo]**, **[!UICONTROL URL di destinazione]**, **[!UICONTROL URL immagine]** ed eventuali attributi personalizzati dichiarati nello schema dell&#39;offerta.

1. Utilizza l&#39;[editor espressioni](../query/expression-editor.md) per personalizzare i valori con i dati di profilo, gli attributi di offerta o i campi della proposta.

1. Per i payload HTML e di testo, fare clic su **[!UICONTROL Modifica contenuto]** per aprire l&#39;editor di contenuto. Puoi progettare il contenuto da zero, programmare il tuo HTML o importare HTML esistente, facoltativamente partendo da un modello di esempio.

>[!IMPORTANT]
>
>Gli attributi disponibili nella sezione **[!UICONTROL Content]** dipendono dallo schema [!DNL nms:offer]. Per esporre gli attributi personalizzati, estendere lo schema e selezionarli nella sezione **[!UICONTROL Contenuto offerta]**. Ulteriori informazioni in [Utilizzare gli schemi](../administration/schemas.md).

## Visualizzare l’anteprima dell’offerta {#preview}

Puoi visualizzare in anteprima l’offerta prima di inviarla.

1. Dall&#39;offerta, selezionare la scheda **[!UICONTROL Anteprima]** accanto a **[!UICONTROL Panoramica]**.

   ![Schermata che mostra l&#39;anteprima dell&#39;offerta.](assets/offers-offer-3.png){zoomable="yes"}

1. Seleziona un profilo di destinazione e, se pertinente, lo spazio dell’offerta su cui eseguire l’anteprima.

   La funzione di rendering definita nello spazio dell’offerta viene applicata al contenuto dell’offerta e viene visualizzata la rappresentazione risultante.

>[!NOTE]
>
>Se l’anteprima restituisce un errore o nessun contenuto, controlla la funzione di rendering dello spazio dell’offerta, le regole di idoneità dell’offerta e che tutti i campi di contenuto obbligatori siano compilati.

## Approvare e distribuire l’offerta {#approve-deploy}

Le offerte non sono immediatamente disponibili nelle consegne: passano attraverso un ciclo di approvazione e distribuzione.

1. Dalla panoramica dell&#39;offerta, fai clic su **[!UICONTROL Approvazione]**.

   ![Schermata che mostra l&#39;approvazione dell&#39;offerta.](assets/offers-offer-4.png){zoomable="yes"}

1. Approva l&#39;idoneità **[!UICONTROL 1&rbrace; e il contenuto**&#x200B;[!UICONTROL &#x200B; 3&rbrace;. &#x200B;]&#x200B;**]** Il contenuto può essere approvato per ogni spazio dell’offerta, in modo da poterlo approvare per uno spazio dell’offerta lasciando gli altri in sospeso.

1. Dopo aver concesso entrambe le approvazioni, fai clic su **[!UICONTROL Distribuisci]** per pubblicare l&#39;offerta nell&#39;ambiente live.

1. Aggiorna la visualizzazione delle offerte per confermare che la rappresentazione **[!UICONTROL Live]** è aggiornata.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>L’approvazione dell’idoneità e del contenuto di un’offerta sono due azioni distinte. Un’offerta può essere approvata parzialmente (solo contenuto, ad esempio) e rimanere non disponibile per la consegna fino a quando non viene concessa anche l’approvazione dell’idoneità.

## Monitorare il dashboard delle offerte {#dashboard}

La scheda **[!UICONTROL Panoramica]** dell&#39;offerta riepiloga lo stato dell&#39;offerta in **[!UICONTROL Proprietà]**, **[!UICONTROL Contenuto]** e **[!UICONTROL Idoneità]** schede, ciascuna con un&#39;icona a forma di matita per tornare all&#39;edizione. Una scheda di **[!UICONTROL Rappresentazione]** elenca ogni spazio dell&#39;offerta a cui è collegata l&#39;offerta, insieme al relativo stato di progettazione corrente.

![Schermata che mostra il dashboard delle offerte.](assets/offers-offer-5.png){zoomable="yes"}

Fai clic su **[!UICONTROL Registri]** per accedere ai registri di distribuzione oppure sul menu **··** (**[!UICONTROL Altro]**) per **[!UICONTROL Duplicare]** o **[!UICONTROL Eliminare]** l&#39;offerta.

Una volta che un’offerta è attiva, la modifica di qualsiasi impostazione riporta l’offerta di progettazione a uno stato modificabile. La rappresentazione in tempo reale rimane invariata fino al successivo ciclo di approvazione e distribuzione.

## Utilizzare l’offerta in una consegna {#use-in-delivery}

Quando l’offerta è live, può essere selezionata da qualsiasi consegna che esegue il targeting dello spazio dell’offerta corrispondente. Scopri come impostare le offerte in una consegna in [Aggiungi offerte ai messaggi](../msg/offers.md).

Per l&#39;integrazione completa della consegna in uscita, tra cui la modalità di generazione della chiamata al motore e di applicazione del tracciamento ai collegamenti delle offerte, consulta la [documentazione di Campaign v8 nelle consegne in uscita](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html){target="_blank"}.

