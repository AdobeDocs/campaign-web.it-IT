---
audience: end-user
title: Utilizzare i componenti per contenuti di E-mail Designer
description: Scopri come utilizzare i componenti per contenuti nelle tue e-mail
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: 5b984089ea36b190cde1046c0d96734e848b5f67
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 96%

---

# Utilizzare i componenti per contenuti {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Informazioni sul contenuto"
>abstract="I componenti per contenuti sono dei segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di un’e-mail."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Informazioni sul contenuto"
>abstract="I componenti per contenuti sono dei segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di una pagina di destinazione."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Informazioni sul contenuto"
>abstract="I componenti per contenuti sono dei segnaposto di contenuto vuoti da utilizzare per creare il layout di un frammento di contenuto."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Informazioni sul contenuto"
>abstract="I componenti per contenuti sono dei segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di un modello."

Quando crei un contenuto e-mail da zero, i componenti per **[!UICONTROL Contenuto]** consentono di personalizzare ulteriormente l’e-mail con componenti vuoti e non elaborati che possono essere utilizzati una volta inseriti in un’e-mail.

Puoi aggiungere tutti i **[!UICONTROL Contenuti]** necessari all’interno di una **[!UICONTROL Struttura]** che definisce il layout dell’e-mail.

## Aggiungere componenti per contenuti {#add-content-components}

Per aggiungere componenti per contenuti all’e-mail e modificarli in base alle tue esigenze, segui i passaggi indicati di seguito:

1. In E-mail designer, utilizza un [contenuto esistente](existing-content.md) oppure trascina una **[!UICONTROL Struttura]** nel contenuto vuoto per definire il layout dell’e-mail. [Scopri come](create-email-content.md)

1. Trascina il **[!UICONTROL Contenuto]** desiderato all’interno delle strutture pertinenti.

   ![](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >È possibile aggiungere più componenti in una singola struttura e in ogni colonna di una struttura.

1. Regola le opzioni per ciascun componente utilizzando la scheda **[!UICONTROL Impostazioni]**. Ad esempio, puoi scegliere di visualizzarlo solo su desktop o dispositivi mobili, oppure su entrambi. Da questa scheda puoi anche gestire le opzioni di collegamento. [Ulteriori informazioni sulla gestione dei collegamenti](message-tracking.md)

1. Regola gli attributi di stile per ciascun componente utilizzando la scheda **[!UICONTROL Stile]**. Ad esempio, puoi modificare lo stile del testo, la spaziatura o il margine di ciascun componente. [Ulteriori informazioni su allineamento e spaziatura](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. Dal menu avanzato del **[!UICONTROL Contenuto]** nel riquadro a destra è possibile eliminare o duplicare facilmente qualsiasi componente per contenuti in base alle esigenze.

## Contenitore {#container}

Puoi aggiungere un contenitore semplice all’interno del quale aggiungere un altro componente di contenuto. In tal modo è possibile applicare uno stile specifico al contenitore, diverso dal componente utilizzato al suo interno.

Ad esempio, aggiungi un componente **[!UICONTROL Contenitore]** e quindi un componente [Pulsante](#button) all’interno del contenitore. Puoi utilizzare uno sfondo specifico per il contenitore e un altro per il pulsante.

![](assets/email_designer_container_component.png){zoomable="yes"}

## Pulsante {#buttons}

Utilizza il componente **[!UICONTROL Pulsante]** per inserire uno o più pulsanti nell’e-mail e reindirizzare il pubblico dell’e-mail a un’altra pagina.

1. Dall’elenco **[!UICONTROL Contenuti]**, trascina il componente **[!UICONTROL Pulsante]** in un componente **[!UICONTROL Struttura]**.

   ![](assets/email_designer_13.png){zoomable="yes"}

1. Fai clic sul pulsante appena aggiunto per personalizzare il testo e accedere alle schede **[!UICONTROL Impostazioni]** e **[!UICONTROL Stili]**.

   ![](assets/email_designer_14.png){zoomable="yes"}

1. Dalle schede **[!UICONTROL Impostazioni]**, nel campo **[!UICONTROL URL]**, aggiungi l’URL a cui desideri reindirizzare l’utente quando farà clic sul pulsante.

1. Con l’elenco a discesa **[!UICONTROL Target]** puoi scegliere in che modo viene visualizzato il contenuto:

   * **[!UICONTROL Nessuno]**: il collegamento viene aperto nello stesso frame in cui è stato fatto clic (impostazione predefinita).
   * **[!UICONTROL Vuoto]**: il collegamento viene aperto in una nuova finestra o scheda.
   * **[!UICONTROL Stesso]**: il collegamento viene aperto nello stesso frame in cui è stato fatto clic.
   * **[!UICONTROL Principale]**: il collegamento viene aperto nel frame principale.
   * **[!UICONTROL Superiore]**: il collegamento viene aperto nel corpo completo della finestra.

   ![](assets/email_designer_15.png){zoomable="yes"}

1. Puoi personalizzare ulteriormente il pulsante modificando gli attributi di stile, ad esempio **[!UICONTROL Bordo]**, **[!UICONTROL Dimensione]**, **[!UICONTROL Margine]**, ecc. dalla scheda **[!UICONTROL Stili]**.

## Testo {#text}

Utilizza il componente **[!UICONTROL Testo]** per inserire testo nell&#39;e-mail e modificare lo stile (bordo, dimensione, spaziatura interna, ecc.) utilizzando le schede **[!UICONTROL Impostazioni]** e **[!UICONTROL Stili]**.

1. Dal menu **[!UICONTROL Contenuti]**, trascina **[!UICONTROL Testo]** in un componente **[!UICONTROL Struttura]**.

   ![](assets/email_designer_11.png){zoomable="yes"}

1. Fai clic sul componente appena aggiunto per personalizzare il testo e accedere alle schede **[!UICONTROL Impostazioni]** e **[!UICONTROL Stili]**.

1. Modifica il testo con le seguenti opzioni disponibili nella barra degli strumenti contestuale:

   ![](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL Modifica stile di testo]**: applica al testo lo stile grassetto, corsivo, sottolineato o barrato.
   * **Modifica l’allineamento**: applica al testo l’allineamento a sinistra, a destra, centrato o giustificato.
   * **[!UICONTROL Crea elenco]**: aggiungi al testo un elenco puntato o numerato.
   * **[!UICONTROL Imposta il titolo]**: aggiungi al testo fino a sei livelli di titolo.
   * **Dimensione font**: seleziona la dimensione del font in pixel.
   * **[!UICONTROL Modifica immagine]**: aggiungi un’immagine o una risorsa al componente testo.
   * **[!UICONTROL Mostra il codice sorgente]**: visualizza il codice sorgente del testo. Non può essere modificato.
   * **[!UICONTROL Duplica]**: aggiungi una copia del componente di testo.
   * **[!UICONTROL Elimina]**: elimina dal messaggio e-mail il componente di testo selezionato.
   * **[!UICONTROL Aggiungi personalizzazione]**: aggiungi campi di personalizzazione per personalizzare il contenuto in base ai dati dei profili.
   * **[!UICONTROL Abilita contenuto condizionale]**: aggiungi contenuto condizionale per adattare il contenuto del componente ai profili target.

1. Regola gli altri attributi di stile quali colore del testo, famiglia di font, bordo, spaziatura, margine, ecc. dalla scheda **[!UICONTROL Stili]**.

   ![](assets/email_designer_12.png){zoomable="yes"}

## Divisore {#divider}

Utilizza il componente **[!UICONTROL Divisore]** per inserire una linea di divisione utile per organizzare il layout e il contenuto dell’e-mail.

È possibile regolare gli attributi di stile, ad esempio il colore, lo stile e lo spessore della linea, dalla scheda **[!UICONTROL Stili]**.

![](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

Utilizza il componente **[!UICONTROL HTML]** per copiare e incollare le diverse parti di un codice HTML esistente. Questo consente di creare componenti modulari HTML a forma libera in modo da riutilizzare dei contenuti esterni.

1. Da **[!UICONTROL Componenti]**, trascina e rilascia il componente **[!UICONTROL HTML]** in un componente **[!UICONTROL struttura]**.

   ![](assets/email_designer_22.png){zoomable="yes"}

1. Fai clic sul componente appena aggiunto, quindi seleziona **[!UICONTROL Mostra il codice sorgente]** dalla barra degli strumenti contestuale per aggiungere il codice HTML.

   ![](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>Per rendere semplicemente un contenuto esterno conforme a E-mail designer, Adobe consiglia di [creare un messaggio da zero](create-email-content.md) e di copiare il contenuto dell’e-mail esistente nei componenti.

## Immagine {#image}

>[!IMPORTANT]
>
>L’accesso al menu di Assets è limitato agli utenti con una licenza Adobe Experience Manager as a Cloud Service attiva. Se non si dispone di questa licenza, il menu Assets non sarà disponibile.

Utilizza il componente **[!UICONTROL Immagine]** per inserire nell’e-mail un file di immagine presente nel computer.

1. Dal menu **[!UICONTROL Contenuto]**, trascina e rilascia l’**[!UICONTROL Immagine]** in un componente **[!UICONTROL Struttura]**.

   ![](assets/email_designer_9.png){zoomable="yes"}

1. Fai clic su **[!UICONTROL Sfoglia]** per scegliere un file di immagine dalle risorse. Puoi anche scegliere di **[!UICONTROL Importare i contenuti multimediali]**.

   Per ulteriori informazioni su come caricare e aggiungere risorse in Adobe Experience Manager, consulta la [documentazione di Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html?lang=it).

   ![](assets/email_designer_28.png){zoomable="yes"}

1. Spostati all’interno delle cartelle per individuare la risorsa specifica necessaria oppure utilizza la barra di ricerca per trovarla in modo efficiente.

   Una volta trovata la risorsa che stai cercando, fai clic su **[!UICONTROL Seleziona]**.

   ![](assets/email_designer_29.png){zoomable="yes"}

1. Fai clic sul componente appena aggiunto e imposta le proprietà dell’immagine utilizzando la scheda **[!UICONTROL Impostazioni]**:

   * **[!UICONTROL Titolo immagine]** consente di definire il titolo da assegnare all’immagine.
   * **[!UICONTROL Testo Alt]** consente di definire la didascalia collegata all’immagine. Questo corrisponde all’attributo HTML “alt”.

   ![](assets/email_designer_10.png){zoomable="yes"}

1. È possibile aggiungere un collegamento per reindirizzare il pubblico a un altro contenuto. [Ulteriori informazioni](message-tracking.md)

1. Regola gli altri attributi di stile quali margine, bordo, ecc. utilizzando la scheda **[!UICONTROL Stili]**.

## Social {#social}

Utilizza il componente **[!UICONTROL Social]** per inserire nel contenuto dell’e-mail dei collegamenti a pagine social media.

1. Dal menu **[!UICONTROL Componenti]**, trascina il componente **[!UICONTROL Social]** in un componente **[!UICONTROL Struttura]**.

1. Fai clic sul componente appena aggiunto.

1. Nel campo **[!UICONTROL Social]** della scheda **[!UICONTROL Impostazioni]**, scegli i social media da aggiungere o rimuovere.

   ![](assets/email_designer_20.png){zoomable="yes"}

1. Scegli la dimensione delle icone nel campo **[!UICONTROL Dimensioni delle immagini]**.

1. Fai clic su ciascuna delle icone di social media per configurare l’**[!UICONTROL URL]** a cui il pubblico viene reindirizzato.

   ![](assets/email_designer_21.png){zoomable="yes"}

1. Se necessario, puoi anche modificare le icone di ciascuno dei social media mediante il campo **[!UICONTROL Origine]**.

1. Regola gli altri attributi quali stile, margine, bordo, ecc. dalla scheda **[!UICONTROL Stili]**.
