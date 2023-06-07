---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 79%

---


# Personalizzare i contenuti{#add-personalization}

## Personalizzare l’oggetto di un messaggio {#personalize-subject-line}

Per aggiungere la personalizzazione nel campo **[!UICONTROL Oggetto]** del messaggio, segui i passaggi seguenti:

1. Apri una consegna e fai clic su **[!UICONTROL Modifica contenuto]**.
1. Fai clic su **[!UICONTROL Apri finestra di dialogo per personalizzazione]** a destra della **[!UICONTROL Oggetto]** campo per le e-mail, oppure **[!UICONTROL Titolo]** campi per le consegne push/SMS.

   ![](assets/perso-subject.png){width="600"}

1. Inserisci l’oggetto o il titolo, quindi seleziona gli attributi di personalizzazione da aggiungere.

1. Fai clic su **[!UICONTROL Conferma]**. Gli attributi di personalizzazione vengono aggiunti al contenuto.

## Personalizzare il contenuto delle e-mail {#personalize-emails}

Per personalizzare il contenuto dell’e-mail, apri il messaggio in E-mail Designer ed esegui le seguenti operazioni:

1. Fai clic all’interno di un blocco di testo.
1. Nella barra degli strumenti contestuale, seleziona **[!UICONTROL Aggiungi personalizzazione]**.

   ![](assets/perso-add-to-content.png)

1. Inserisci il nome del destinatario nell’editor di personalizzazione e conferma.

   ![](assets/perso-add-name.png)

   L’attributo di personalizzazione viene aggiunto al contenuto dell’e-mail.

   Puoi simulare il contenuto per controllarne il rendering. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Per aggiungere un blocco di contenuto all’e-mail, segui questi stessi passaggi e seleziona un blocco di contenuto dall’ultima icona:

   ![](assets/perso-insert-block.png)

1. Una volta inserito, il blocco di contenuto viene aggiunto al contenuto dell’e-mail e viene adattato automaticamente al profilo del destinatario quando viene generata la personalizzazione, nella fase di preparazione della consegna.

   ![](assets/perso-content-block-in-email.png)

## Personalizzare i collegamenti nelle e-mail {#personalize-links}

Per personalizzare un **collegamento**:

1. Seleziona un blocco di testo o un’immagine.
1. Nella barra degli strumenti contestuale, seleziona **Inserisci collegamento**.

   ![](assets/perso-link.png)

1. Immetti l’etichetta del collegamento e utilizza il pulsante **Inserisci collegamento** per personalizzare il collegamento.

   ![](assets/perso-link-insert-icon.png)

1. Utilizza l’editor di personalizzazione per definire e personalizzare il collegamento, quindi conferma.

   ![](assets/perso-link-edit.png)


## Personalizzare le offerte {#personalize-offers}

Puoi anche accedere all’editor di personalizzazione quando aggiungi contenuti testuali alle rappresentazioni delle offerte. Per ulteriori informazioni, consulta [questa sezione](../content/offers.md).

