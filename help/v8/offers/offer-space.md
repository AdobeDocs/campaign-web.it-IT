---
audience: end-user
title: Creare e gestire gli spazi dell’offerta
description: Scopri come creare, configurare, distribuire e visualizzare in anteprima gli spazi delle offerte nel web di Campaign
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# Creare e gestire gli spazi dell’offerta {#offer-space}

Uno **spazio dell&#39;offerta** definisce dove e come un&#39;offerta viene esposta a un contatto: quale canale utilizza (e-mail, direct mail, SMS, web in entrata, ecc.), quali campi di contenuto può utilizzare l&#39;offerta e come viene creata la rappresentazione finale. Un singolo ambiente può contenere più spazi di offerta, uno per ogni punto di esposizione.

Uno spazio dell’offerta non è un canale di per sé. Rappresenta una posizione specifica in cui l’offerta viene visualizzata su un canale. Due banner sulla stessa pagina web corrispondono in genere a due spazi di offerta diversi. Per il modello concettuale completo, consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

## Creare o modificare uno spazio dell’offerta{#create-offer-space}

Gli spazi dell’offerta vengono memorizzati nella cartella dell’ambiente dell’offerta. Per sfogliare gli spazi delle offerte disponibili sulla piattaforma, apri **[!UICONTROL Explorer]**, accedi all&#39;ambiente delle offerte e seleziona la sottocartella che le contiene.

![Schermata che mostra l&#39;elenco degli spazi dell&#39;offerta.](assets/offers-space.png){zoomable="yes"}

Da qui, puoi aprire uno spazio delle offerte esistente o crearne uno nuovo facendo clic su **[!UICONTROL Crea spazio delle offerte]**.

![Schermata che mostra la schermata dello spazio dell&#39;offerta.](assets/offers-space-1.png){zoomable="yes"}

### Definire le proprietà {#properties}

Questa sezione consente di:

* Immetti un **[!UICONTROL Label]** per lo spazio dell&#39;offerta.
* Seleziona il **[!UICONTROL canale]** che corrisponde al punto di esposizione (e-mail, direct mailing, SMS, web, ecc.).
* Seleziona **[!UICONTROL Abilita modalità unitaria]** se questo spazio dell&#39;offerta deve supportare anche chiamate unitarie (in tempo reale, a offerta singola) al motore di offerta, oltre a chiamate di consegna in blocco.

### Definire i campi di contenuto {#content-fields}

Nei campi di contenuto sono elencati gli attributi che possono essere modificati a livello di offerta e riutilizzati dalla funzione di rendering. L&#39;ordine in cui si aggiungono i campi nello spazio delle offerte determina l&#39;ordine in cui sono esposti nella sezione **[!UICONTROL Contenuto]** dell&#39;offerta.

Per impostazione predefinita, ogni offerta include i seguenti campi di contenuto predefiniti: **[!UICONTROL Titolo]**, **[!UICONTROL URL di destinazione]**, **[!UICONTROL URL immagine]**, **[!UICONTROL Contenuto HTML]** e **[!UICONTROL Contenuto testo]**. Puoi estendere questo elenco con qualsiasi campo personalizzato di cui hai bisogno per il rendering, ad esempio un **contenuto breve**, un **URL tracciato** o qualsiasi attributo aggiunto tramite l&#39;estensione dello schema.

Fai clic su **[!UICONTROL Aggiungi campo di contenuto]**, quindi seleziona l&#39;attributo da esporre dallo schema dell&#39;offerta, oppure fai clic su **[!UICONTROL Modifica espressione]** per definire un&#39;espressione personalizzata.

>[!IMPORTANT]
>
>Per rendere modificabile un attributo personalizzato dalla sezione **[!UICONTROL Content]** dell&#39;offerta, l&#39;attributo deve essere dichiarato anche nella sezione **[!UICONTROL Offer content]** dello schema [!DNL nms:offer]. Ulteriori informazioni in [Utilizzare gli schemi](../administration/schemas.md).

### Configurare le funzioni di rendering {#rendering}

Le funzioni di rendering generano la rappresentazione finale dell’offerta dai campi di contenuto. È possibile scegliere tra il rendering predefinito, che restituisce semplicemente il contenuto così come è, o una funzione personalizzata che combina i campi con HTML, XML o testo.

Selezionare la scheda **[!UICONTROL Rendering HTML]**, **[!UICONTROL Rendering XML]** o **[!UICONTROL Rendering testo]** e abilitare **[!UICONTROL Sovraccaricare la funzione di rendering]** per attivarla.

Utilizza l’editor di espressioni per scrivere la funzione di rendering. Puoi fare riferimento ai campi di contenuto definiti nello spazio, negli attributi dell&#39;offerta e in qualsiasi funzione dall&#39;[editor espressioni](../query/expression-editor.md).

>[!NOTE]
>
>Se non è definita alcuna funzione di rendering, il contenuto dell’offerta viene restituito così come è utilizzando gli attributi predefiniti. La funzione di rendering XML può essere utilizzata solo quando nello spazio delle offerte è selezionato **[!UICONTROL Abilita modalità unitaria]**.

### Configurare lo stato dell’archiviazione e della proposta {#storage}

Questa sezione ti consente di controllare come vengono mantenute le proposte generate tramite questo spazio e come il loro stato evolve durante il loro ciclo di vita:

* **[!UICONTROL Disattiva l&#39;inserimento di proposte]** — impedisce l&#39;inserimento di proposte generate tramite questo spazio di offerta nella tabella di archiviazione delle proposte.

* **[!UICONTROL Stato]** della proposta — Stato applicato alla proposta nel momento in cui il motore di offerta la restituisce (in genere **[!UICONTROL Presentato]** per le consegne in uscita).

* **[!UICONTROL Stato]** all&#39;accettazione — Stato applicato quando il destinatario interagisce con l&#39;offerta (in genere **[!UICONTROL Accettato]**).

I valori di stato disponibili corrispondono all’elenco utilizzato dalla console client. Per ulteriori informazioni, consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"} nella documentazione della console.

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### Configurare le impostazioni avanzate {#advanced}

Questa sezione ti consente di definire l&#39;**[!UICONTROL identificazione Target]**. Fai clic su **[!UICONTROL Aggiungi]** e seleziona uno o più attributi **[!UICONTROL Destinatario]** oppure fai clic su **[!UICONTROL Modifica espressione]** per definire un&#39;espressione personalizzata. Questa impostazione è facoltativa per uno spazio dell’offerta di base. Per il riferimento e il comportamento completi, consulta la [documentazione di Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

Gli spazi dell&#39;offerta creati nel **canale Web in entrata** richiedono inoltre che il sito Web sia configurato per visualizzare l&#39;offerta e chiamare il motore di offerta. Questa integrazione viene eseguita nella console client. Vedere [Presentare le offerte in tempo reale](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"} e [Configurare l&#39;integrazione del motore di offerta](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"} nella documentazione di Campaign v8.

## Distribuire lo spazio dell’offerta {#deploy}

È necessario distribuire uno spazio dell’offerta prima di utilizzarlo in una consegna. Salva il tuo spazio delle offerte, quindi fai clic su **Distribuisci**. Lo stato della distribuzione si riflette sullo spazio dell’offerta.

![Schermata che mostra la distribuzione dell&#39;offerta.](assets/offers-space-2.png){zoomable="yes"}

## Visualizzare l’anteprima dello spazio dell’offerta {#preview}

L’anteprima consente di simulare la modalità di selezione e rendering di un’offerta per una determinata destinazione.

1. Nello spazio delle offerte, seleziona la scheda **[!UICONTROL Anteprima]** accanto a **[!UICONTROL Panoramica]**.

   ![Schermata che mostra l&#39;anteprima dell&#39;offerta.](assets/offers-space-3.png){zoomable="yes"}

1. Seleziona un profilo di destinazione ed esegui l’anteprima. Le offerte corrispondenti vengono restituite con la rappresentazione prodotta dalla funzione di rendering.

>[!NOTE]
>
>Se non vengono restituite proposte, controlla le regole di idoneità delle offerte e la configurazione dello spazio.

Quindi [crea un&#39;offerta](create-offer.md) nel catalogo e assegnala a questo spazio.
