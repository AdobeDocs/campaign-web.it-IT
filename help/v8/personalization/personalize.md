---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 0d74cababf2b4d66d3b2ce9b0ae2a0f00cb1cdef
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Personalizzare i contenuti{#add-personalization}

![](../assets/do-not-localize/badge.png)

Puoi personalizzare il contenuto del messaggio:

* Inserimento dinamico **campi di personalizzazione**

   I campi di personalizzazione vengono utilizzati per la personalizzazione di primo livello dei messaggi. Puoi selezionare qualsiasi campo disponibile nel database dall’editor di personalizzazione. Per una consegna, puoi selezionare qualsiasi campo correlato al destinatario, al messaggio o alla consegna. Questi attributi di personalizzazione possono essere inseriti nella riga dell’oggetto o nel corpo dei messaggi.

   ![](assets/perso-subject-line.png)

   La sintassi seguente inserisce nel contenuto la città del destinatario: &lt;%= recipient.location.city %>.

* Inserimento di dati predefiniti **blocchi di contenuto**

   Campaign viene fornito con un set di blocchi di personalizzazione che contengono un rendering specifico che puoi inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di auguri o un collegamento alla pagina speculare del messaggio. I blocchi di contenuto sono disponibili da una voce dedicata nell’editor per la personalizzazione.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalizzare l’oggetto dell’e-mail {#personalize-subject-line}

Per aggiungere la personalizzazione nel **[!UICONTROL Linea oggetto]** nel campo del messaggio, segui i passaggi seguenti:

1. Fai clic sul pulsante **Apre la finestra di dialogo di personalizzazione** a destra **Linea oggetto** campo .
1. Inserisci il contenuto della riga oggetto e seleziona gli attributi di personalizzazione da aggiungere.
1. Fai clic su **Conferma** da convalidare. Gli attributi di personalizzazione vengono aggiunti alla riga dell’oggetto.

![](assets/perso-subject.png)

## Personalizzare il contenuto delle e-mail {#personalize-emails}

Per personalizzare il contenuto dell’e-mail, apri il messaggio nella finestra di progettazione e-mail e:

1. Fare clic all’interno di un blocco di testo.
1. Nella barra degli strumenti contestuale, seleziona **Aggiungi personalizzazione**.

   ![](assets/perso-add-to-content.png)

1. Inserisci il nome del destinatario nell’editor di personalizzazione e conferma.

   ![](assets/perso-add-name.png)

   L’attributo di personalizzazione viene aggiunto al contenuto dell’e-mail.

   Puoi simulare il contenuto per controllare il rendering. [Ulteriori informazioni](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Personalizzare i collegamenti nelle e-mail {#personalize-links}

Per personalizzare un **collegamento**:

1. Seleziona un blocco di testo o un’immagine.
1. Nella barra degli strumenti contestuale, seleziona **Aggiungi personalizzazione**.

   ![](assets/perso-link.png)

1. Utilizza l’editor di personalizzazione per definire e personalizzare il collegamento.

## Personalizzare le offerte {#personalize-offers}

Puoi anche accedere all’editor di personalizzazione quando aggiungi contenuto di tipo testo alle rappresentazioni delle offerte. Ulteriori informazioni in [questa sezione](../content/offers.md).
