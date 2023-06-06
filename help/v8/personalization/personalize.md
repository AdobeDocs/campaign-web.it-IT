---
title: Personalizzare i contenuti in Campaign
description: Scopri come personalizzare i contenuti nell’interfaccia web di Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 48d5684201f006add0ceb467129dbbcf98465c5b
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 77%

---


# Personalizzare i contenuti{#add-personalization}

Per ottenere il massimo da ogni campagna di marketing, Adobe Campaign offre un modo per fornire contenuti personalizzati che parlano ai clienti a loro livello. In base ai dati del profilo, utilizza le funzionalità di personalizzazione per creare un’esperienza personalizzata per diversi gruppi e singoli utenti: puoi adattare i messaggi a ogni destinatario specifico sfruttando i dati e le informazioni di cui disponi su di essi. Può essere il nome, gli interessi, dove vivono, cosa hanno comprato, e molto altro.

Utilizza Campaign per creare contenuti dinamici e inviare messaggi personalizzati. Le funzionalità di personalizzazione possono essere combinate per migliorare i messaggi e creare un’esperienza utente personalizzata.

Puoi personalizzare il contenuto del messaggio in diversi modi:

* Inserendo **campi di personalizzazione** dinamici

   I campi di personalizzazione vengono utilizzati per la personalizzazione di primo livello dei messaggi. Puoi selezionare qualsiasi campo disponibile nel database dall’editor di personalizzazione. Per una consegna, puoi selezionare qualsiasi campo correlato al destinatario, al messaggio o alla consegna. Questi attributi di personalizzazione possono essere inseriti nella riga dell’oggetto o nel corpo dei messaggi.

   ![](assets/perso-subject-line.png)

   Per inserire nel contenuto la città del destinatario, utilizza la seguente sintassi: &lt;%= recipient.location.city %>.

* Inserimento di **blocchi di contenuto** predefiniti

   Campaign viene fornito con un set di blocchi di personalizzazione contenenti un rendering specifico da inserire nelle consegne. Ad esempio, puoi aggiungere un logo, un messaggio di saluto o un collegamento alla pagina speculare di un messaggio e-mail. I blocchi di contenuto sono disponibili da una voce dedicata nell’editor di personalizzazione.

   ![](assets/perso-content-blocks.png)

* Creare **contenuto condizionale**

   Configura il contenuto condizionale per aggiungere la personalizzazione dinamica, ad esempio in base al profilo del destinatario. I blocchi di testo e/o le immagini vengono inseriti quando viene soddisfatta una particolare condizione. Puoi definire la versione alternativa del contenuto quando la condizione non è true.


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

## Blocchi di contenuto incorporati {#ootb-content-blocks}

I blocchi di contenuto incorporati sono:

* **[!UICONTROL Enabled by Adobe Campaign]** : inserisce il logo “Enabled by Adobe Campaign”.
* **[!UICONTROL Funzione di formattazione per nomi propri]**: genera la funzione JavaScript **[!UICONTROL toSmartCase]**, che applica il maiuscolo alla prima lettera di ogni parola.
* **[!UICONTROL Saluti]**: inserisce i saluti con il nome completo del destinatario, seguito da una virgola. Esempio: “Ciao John Doe,” 
* **[!UICONTROL Inserisci logo]**: inserisce un logo definito nelle impostazioni dell’istanza.
* **[!UICONTROL Collegamento a una pagina mirror]**: inserisce un collegamento alla [pagina mirror](../content/mirror-page.md). Il formato predefinito è: “Se non riesci a visualizzare correttamente questo messaggio, fai clic qui”.
* **[!UICONTROL URL pagina mirror]**: inserisce l’URL della pagina mirror, consentendo ai designer della consegna di controllare il collegamento.
* **[!UICONTROL URL per accettazione offerta in modalità unitaria]**: inserisce un URL che consente di impostare un’offerta su **[!UICONTROL Accettata]**. Questo blocco è disponibile se il modulo di interazione è abilitato
* **[!UICONTROL Conferma registrazione]**: inserisce un collegamento che consente di confermare la registrazione o l’iscrizione.
* **[!UICONTROL Collegamento di registrazione]**: inserisce un collegamento per la registrazione o l’iscrizione. Questo collegamento è definito nelle impostazioni dell’istanza. Il contenuto predefinito è: “Per registrarti, fai clic qui.”
* **[!UICONTROL Collegamento di registrazione (con destinatario che inoltra)]**: inserisce un collegamento di registrazione o iscrizione che consente di identificare il visitatore e la consegna. Questo collegamento è definito nelle impostazioni dell’istanza.
* **[!UICONTROL URL pagina di registrazione]**: inserisce un URL per registrarsi o iscriversi
* **[!UICONTROL Stile e-mail di contenuto]** e **[!UICONTROL Stile notifica]**: genera il codice necessario per formattare un’e-mail con stili HTML predefiniti.
* **[!UICONTROL Collegamento annullamento iscrizione]**: inserisce un collegamento che consente di annullare l’iscrizione a tutte le consegne (elenco Bloccati). Il contenuto associato predefinito è: “Hai ricevuto questo messaggio perché sei stato in contatto con ***nome organizzazione*** o una sua filiale. Per non ricevere più messaggi da ***nome organizzazione***, fai clic qui.”
