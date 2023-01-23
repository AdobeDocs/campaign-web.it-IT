---
audience: end-user
title: Utilizzare i componenti contenuto di e-mail designer
description: Scopri come utilizzare i componenti di contenuto nelle e-mail
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# Utilizzare i componenti contenuto di E-mail designer {#content-components}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Informazioni sui componenti Contenuto"
>abstract="I componenti contenuto sono segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di un’e-mail."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Informazioni sui componenti Contenuto"
>abstract="I componenti contenuto sono segnaposto di contenuto vuoti che possono essere utilizzati per creare il layout di una pagina di destinazione."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Informazioni sui componenti Contenuto"
>abstract="I componenti contenuto sono segnaposto di contenuto vuoti che è possibile utilizzare per creare il layout di un frammento."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Informazioni sui componenti Contenuto"
>abstract="I componenti contenuto sono segnaposto di contenuto vuoti che è possibile utilizzare per creare il layout di un modello."

## Aggiungi componenti di contenuto {#add-content-components}

Per aggiungere componenti di contenuto all’e-mail e modificarli in base alle tue esigenze, segui la procedura seguente.

1. In E-mail Designer, utilizza un contenuto esistente o trascina e rilascia **[!UICONTROL Componenti struttura]** nel contenuto vuoto per definire il layout dell’e-mail. [Scopri come](create-email-content.md)

1. Per accedere al **[!UICONTROL Componenti contenuto]** selezionare il pulsante corrispondente dal riquadro a sinistra di E-mail Designer.

   ![](assets/email_designer_content_components.png)

1. Trascina e rilascia i componenti di contenuto desiderati all’interno dei componenti struttura pertinenti.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >È possibile aggiungere più componenti in un singolo componente struttura e in ogni colonna di un componente struttura.

1. Regolare gli attributi di stile per ciascun componente utilizzando **[!UICONTROL Impostazioni dei componenti]** a destra. Ad esempio, puoi modificare lo stile del testo, la spaziatura o il margine di ciascun componente. [Ulteriori informazioni su allineamento e spaziatura](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

Quando crei il tuo contenuto e-mail da zero, **[!UICONTROL Componenti contenuto]** consente di personalizzare ulteriormente l’e-mail con componenti vuoti e non elaborati che possono essere utilizzati una volta inseriti in un messaggio e-mail.
Puoi aggiungere più **[!UICONTROL Componenti contenuto]** come necessario all&#39;interno di un **[!UICONTROL Componente struttura]** che definisce il layout del messaggio e-mail.

## Contenitore {#container}

Puoi aggiungere un contenitore semplice all’interno del quale aggiungere un altro componente di contenuto. Questo consente di applicare uno stile specifico al contenitore, diverso dal componente utilizzato all’interno.

Ad esempio, aggiungi un **[!UICONTROL Contenitore]** e quindi aggiungi un [Pulsante](#button) all’interno del contenitore. Puoi utilizzare uno sfondo specifico per il contenitore e un altro per il pulsante.

![](assets/email_designer_container_component.png)

## Pulsante {#buttons}

Utilizza la **[!UICONTROL Pulsante]** per inserire uno o più pulsanti nell’e-mail e reindirizzare il pubblico dell’e-mail a un’altra pagina.

1. Da **[!UICONTROL Componenti contenuto]**, trascina e rilascia la **[!UICONTROL Pulsante]** in un **[!UICONTROL Componente struttura]**.

   ![](assets/email_designer_13.png)

1. Fai clic sul pulsante appena aggiunto per personalizzare il testo e avere accesso al **[!UICONTROL Impostazioni dei componenti]** nel riquadro a destra di E-mail Designer.

   ![](assets/email_designer_14.png)

1. In **[!UICONTROL Collegamento]** aggiungi l’URL a cui desideri reindirizzare quando fai clic sul pulsante .

1. Scegli in che modo il contenuto viene visualizzato con il **[!UICONTROL Target]** elenco a discesa:

   * **[!UICONTROL Nessuno]**: apre il collegamento nello stesso frame in cui è stato fatto clic (impostazione predefinita).
   * **[!UICONTROL Vuoto]**: apre il collegamento in una nuova finestra o scheda.
   * **[!UICONTROL Self]**: apre il collegamento nello stesso frame in cui è stato fatto clic.
   * **[!UICONTROL Elemento padre]**: apre il collegamento nel frame principale.
   * **[!UICONTROL Top]**: apre il collegamento nel corpo completo della finestra.

   ![](assets/email_designer_15.png)

1. Puoi personalizzare ulteriormente il pulsante modificando gli attributi di stile, ad esempio **[!UICONTROL Bordo]**, **[!UICONTROL Dimensione]**, **[!UICONTROL Margine]**, ecc. dal **[!UICONTROL Impostazioni dei componenti]** riquadro.

## Testo {#text}

Utilizza la **[!UICONTROL Testo]** per inserire testo nell’e-mail e regolare lo stile (bordo, dimensione, spaziatura, ecc.) utilizzando **[!UICONTROL Impostazioni dei componenti]** riquadro.

1. Da **[!UICONTROL Componenti contenuto]**, trascinamento **[!UICONTROL Testo]** in **[!UICONTROL Componente struttura]**.

   ![](assets/email_designer_11.png)

1. Fai clic sul componente appena aggiunto per personalizzare il testo e avere accesso al **[!UICONTROL Impostazioni dei componenti]** nel riquadro a destra della finestra di progettazione e-mail.

1. Modifica il testo con le seguenti opzioni disponibili nella barra degli strumenti:

   ![](assets/email_designer_27.png)

   * **[!UICONTROL Modificare lo stile del testo]**: applicare al testo in grassetto, corsivo, sottolineato o barrato.
   * **Modificare l’allineamento**: scegliere tra allineamento a sinistra, a destra, al centro o giustificato per il testo.
   * **[!UICONTROL Crea elenco]**: aggiungere al testo un elenco puntato o un elenco di numeri.
   * **[!UICONTROL Imposta intestazione]**: aggiungi fino a sei livelli di intestazione al testo.
   * **Dimensione font**: selezionare la dimensione del font del testo in pixel.
   * **[!UICONTROL Modifica immagine]**: aggiungi un’immagine o una risorsa al componente testo.
   * **[!UICONTROL Mostra il codice sorgente]**: visualizza il codice sorgente del testo. Non può essere modificato.
   * **[!UICONTROL Duplica]**: aggiungi una copia del componente testo.
   * **[!UICONTROL Elimina]**: elimina il componente di testo selezionato dal messaggio e-mail.
   * **[!UICONTROL Aggiungi personalizzazione]**: aggiungi campi di personalizzazione per personalizzare il contenuto dai dati dei profili.
   * **[!UICONTROL Abilitare il contenuto condizionale]**: aggiungi contenuto condizionale per adattare il contenuto del componente ai profili target.

1. Regolare gli altri attributi di stile quali colore del testo, famiglia di font, bordo, spaziatura, margine, ecc. dal **[!UICONTROL Impostazioni dei componenti]** riquadro.

   ![](assets/email_designer_12.png)

## Divisore {#divider}

Utilizza la **[!UICONTROL Divider]** per inserire una linea di divisione per organizzare il layout e il contenuto dell’e-mail.

È possibile regolare gli attributi di stile, ad esempio il colore della linea, lo stile e l’altezza dalla **[!UICONTROL Impostazioni dei componenti]** riquadro.

![](assets/email_designer_16.png)

## HTML {#HTML}

Utilizza la **[!UICONTROL HTML]** per copiare e incollare le diverse parti di HTML esistenti. Questo consente di creare componenti modulari HTML gratuiti per riutilizzare alcuni contenuti esterni.

1. Da **[!UICONTROL Componenti contenuto]**, trascina e rilascia la **[!UICONTROL HTML]** in un **[!UICONTROL Componente struttura]**.

   ![](assets/email_designer_22.png)

1. Fai clic sul componente appena aggiunto, quindi seleziona **[!UICONTROL Mostra il codice sorgente]** dalla barra degli strumenti contestuale per aggiungere il tuo HTML.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>Per rendere semplicemente un contenuto esterno conforme a E-mail Designer, Adobe consiglia di creare un messaggio da zero e di copiare il contenuto dell’e-mail esistente nei componenti.

## Immagine {#image}

Utilizza la **[!UICONTROL Immagine]** per inserire un file immagine dal computer nell’e-mail.

1. In **[!UICONTROL Componenti contenuto]**, trascinamento **[!UICONTROL Immagine]** in **[!UICONTROL Componente struttura]**.

   ![](assets/email_designer_9.png)

1. Fai clic su **[!UICONTROL Sfoglia]** per scegliere un file di immagine dalle risorse.

1. Fai clic sul componente appena aggiunto e imposta le proprietà dell’immagine utilizzando **[!UICONTROL Impostazioni dei componenti]** riquadro:

   * **[!UICONTROL Titolo immagine]** consente di definire un titolo per l’immagine.
   * **[!UICONTROL Testo alternativo]** consente di definire la didascalia collegata all’immagine. Questo corrisponde all’attributo alt HTML.

   ![](assets/email_designer_10.png)

1. Regolare gli altri attributi di stile quali margine, bordo, ecc. o aggiungendo un collegamento per reindirizzare il pubblico a un altro contenuto dalla pagina **[!UICONTROL Impostazioni dei componenti]** riquadro.

## Social {#social}

Utilizza la **[!UICONTROL Social]** per inserire i collegamenti alle pagine dei social media nel contenuto dell’e-mail.

1. Da **[!UICONTROL Componenti contenuto]**, trascina e rilascia la **[!UICONTROL Social]** in un **[!UICONTROL Componente struttura]**.

1. Fai clic sul componente appena aggiunto.

1. In **[!UICONTROL Social]** campo **[!UICONTROL Impostazioni dei componenti]** scegliere i social media da aggiungere o rimuovere.

   ![](assets/email_designer_20.png)

1. Scegli la dimensione delle icone nella **[!UICONTROL Dimensioni delle immagini]** campo .

1. Fai clic su ciascuna delle icone dei social media per configurare le **[!UICONTROL URL]** a cui il pubblico viene reindirizzato.

   ![](assets/email_designer_21.png)

1. Puoi anche modificare le icone di ciascuno dei tuoi social media, se necessario, in **[!UICONTROL Immagine]** campo .

1. Regolare gli altri attributi di stile quali stile, margine, bordo, ecc. dal **[!UICONTROL Impostazioni dei componenti]** riquadro.
