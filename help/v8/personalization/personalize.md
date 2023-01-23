---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 51bd6f405ad151e2264d69c57ffe5e1783077203
workflow-type: tm+mt
source-wordcount: '653'
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

Per aggiungere un blocco di contenuto all’e-mail, applica gli stessi passaggi e seleziona un blocco di contenuto dall’ultima icona:

![](assets/perso-insert-block.png)

Una volta inserito, il blocco di contenuto viene aggiunto al contenuto dell’e-mail, come mostrato di seguito. Viene automaticamente adattato al profilo del destinatario quando viene generata la personalizzazione, nella fase di preparazione della consegna.

![](assets/perso-content-block-in-email.png)


I blocchi di contenuto incorporati sono:
* **[!UICONTROL Abilitato da Adobe Campaign]** : inserisce il logo &quot;Abilitato da Adobe Campaign&quot;.
* **[!UICONTROL Funzione di formattazione per i sostantivi appropriati]** : genera **[!UICONTROL toSmartCase]** Funzione Javascript, che cambia in maiuscolo la prima lettera di ogni parola.
* **[!UICONTROL Saluti]** : inserisce i saluti con il nome del destinatario. Esempio: &quot;Ciao John Doe.&quot;
* **[!UICONTROL Inserisci logo]** : inserisce un logo definito nelle impostazioni dell’istanza.
* **[!UICONTROL Collegamento a una pagina speculare]** : inserisce un collegamento alla pagina speculare: &quot;Se non riesci a visualizzare correttamente questo messaggio, fai clic qui&quot;.
* **[!UICONTROL URL pagina speculare]** : inserisce l’URL della pagina speculare, consentendo a Progettazione consegne di controllare il collegamento.
* **[!UICONTROL URL di accettazione dell’offerta in modalità unitaria]** : inserisce un URL che consente di impostare un’offerta su **[!UICONTROL Accettato]**.
* **[!UICONTROL URL della pagina di registrazione]** : inserisce un URL di abbonamento.
* **[!UICONTROL Collegamento di registrazione]** : inserisce un collegamento di abbonamento. Questo collegamento è definito nelle impostazioni dell’istanza. Il contenuto predefinito è: &quot;Per registrarti clicca qui.&quot;
* **[!UICONTROL Collegamento di registrazione (con referrer)]** : inserisce un collegamento di abbonamento, che consente di identificare il visitatore e la consegna. Questo collegamento è definito nelle impostazioni dell’istanza.
* **[!UICONTROL Conferma della registrazione]** : inserisce un collegamento che consente di confermare l’abbonamento.
* **[!UICONTROL Collegamenti di condivisione social network]** : inserisce pulsanti che consentono al destinatario di condividere un collegamento al contenuto della pagina speculare.
* **[!UICONTROL Stile delle e-mail di contenuto]** e **[!UICONTROL Stile di notifica]** : genera codice che formatta un’e-mail con stili di HTML predefiniti.
* **[!UICONTROL Collegamento di annullamento dell’abbonamento]** : inserisce un collegamento che consente di annullare l’iscrizione a tutte le consegne (elenco Bloccati). Il contenuto associato predefinito è: &quot;Stai ricevendo questo messaggio perché sei stato in contatto con ***nome organizzazione*** o una filiale. Per non ricevere più messaggi da ***nome organizzazione*** clicca qui.&quot;


## Personalizzare i collegamenti nelle e-mail {#personalize-links}

Per personalizzare un **collegamento**:

1. Seleziona un blocco di testo o un’immagine.
1. Nella barra degli strumenti contestuale, seleziona **Inserisci collegamento**.

   ![](assets/perso-link.png)

1. Immetti l’etichetta del collegamento e utilizza il **Inserisci collegamento** per personalizzare il collegamento.

   ![](assets/perso-link-insert-icon.png)

1. Utilizza l’editor di personalizzazione per definire e personalizzare il collegamento e confermare.

   ![](assets/perso-link-edit.png)


## Personalizzare le offerte {#personalize-offers}

Puoi anche accedere all’editor di personalizzazione quando aggiungi contenuto di tipo testo alle rappresentazioni delle offerte. Ulteriori informazioni in [questa sezione](../content/offers.md).
