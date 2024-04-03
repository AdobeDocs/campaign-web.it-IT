---
title: Creare contenuti condizionali
description: Scopri come definire le condizioni per personalizzare il contenuto in Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: c0b032539397d4f06c0e34981ed9e76bccb9cfd1
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 81%

---

# Generare contenuti condizionali{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Aggiungere contenuto condizionale"
>abstract="Configura i campi per contenuti condizionali per creare una personalizzazione dinamica avanzata in base ai dati del profilo del destinatario. I blocchi di testo, i collegamenti, l’oggetto e/o le immagini vengono sostituiti nel contenuto del messaggio quando viene soddisfatta una particolare condizione."

## Introduzione ai contenuti condizionali {#gs}

Il contenuto condizionale è una funzione potente che consente di creare una personalizzazione dinamica basata sui dati del profilo del destinatario, sostituendo automaticamente blocchi di testo e immagini quando vengono soddisfatte determinate condizioni. Con questa funzione puoi creare campagne più sofisticate e offrire al tuo pubblico esperienze altamente mirate e personalizzate.

Configurando i campi per contenuti condizionali, puoi creare ad esempio una personalizzazione dinamica avanzata in base al profilo del destinatario. I blocchi di testo, i collegamenti, l’oggetto e/o le immagini vengono sostituiti nel contenuto del messaggio quando viene soddisfatta una particolare condizione. Ad esempio, puoi visualizzare “Sig.” o “Sig.ra” in base al valore del campo Genere nel database di Adobe Campaign oppure includere un collegamento diverso in base alla lingua preferita del destinatario.

Per creare contenuti condizionali, è necessario creare condizioni nell’**editor di espressioni** tramite funzioni Helper specifiche. Questo metodo è disponibile per tutti i canali di consegna in qualsiasi campo in cui è possibile accedere all’editor di espressioni, ad esempio la riga dell’oggetto o i collegamenti e-mail e i componenti di contenuto di tipo testo o pulsante. [Scopri come accedere all’editor di espressioni](gs-personalization.md/#access)

Oltre all’editor di espressioni, puoi sfruttare una **generatore di contenuti condizionali** durante la progettazione di un’e-mail che ti consente di creare più varianti per un elemento del corpo dell’e-mail. [Scopri come creare contenuti condizionali nelle e-mail](#condition-condition-builder)

## Creare condizioni nell’editor di espressioni {#condition-perso-editor}

Per definire il contenuto condizionale di una consegna utilizzando l’editor di espressioni, segui questi passaggi. In questo esempio, vogliamo creare contenuti condizionali in base alla lingua dei destinatari (francese o inglese).

1. Apri una consegna e passa alla sezione di modifica del contenuto.

1. Individua il campo in cui desideri aggiungere i contenuti condizionali. Ad esempio, puoi aggiungere contenuti condizionali a un messaggio SMS.

1. Per aprire l’editor di espressioni fai clic sull’icona **[!UICONTROL Apri finestra di dialogo di personalizzazione]**, accanto al campo.

   ![](assets/open-perso-editor-sms.png){zoomable=&quot;yes&quot;}

1. Nell’editor di personalizzazione, passa a **[!UICONTROL Condizioni]** menu a sinistra.

1. Per iniziare a creare la condizione, fai clic sull’icona “+” accanto alla funzione **If** (se). La seguente riga viene aggiunta alla schermata centrale: `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Sostituisci `<FIELD>` con un campo di personalizzazione, ad esempio la lingua del destinatario: `recipient.language`.
   * Sostituisci `<VALUE>` con il valore da soddisfare. Ad esempio, `'French'`.
   * Sostituisci `Ìnsert content here` con il contenuto che desideri mostrare ai profili che soddisfano la condizione specificata.

     ![](assets/condition-sample1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Specifica il contenuto da visualizzare se i destinatari non soddisfano la condizione. Per eseguire questa operazione, utilizza una funzione Helper **else** (altrimenti):

   1. Posiziona il cursore prima del tag di chiusura dell’espressione `%>` e fai clic su `+` accanto alla funzione **Else**.

   1. Sostituisci `Ìnsert content here` con il contenuto che desideri mostrare ai profili che non soddisfano la condizione della funzione if.

   ![](assets/condition-sample2.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   È inoltre possibile utilizzare la funzione Helper **else if** per creare condizioni con più varianti di contenuto. Ad esempio, l’espressione seguente mostra tre varianti di un messaggio a seconda della lingua dei destinatari:

   ![](assets/condition-sample3.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   >[!NOTE]
   >
   >Ogni volta che viene aggiunta una funzione Helper, i tag di apertura (`<%`) e chiusura (`%>`) vengono aggiunti automaticamente prima e dopo la funzione.
   >
   >Ad esempio dopo l’aggiunta di una funzione Helper “Else” all’interno di un’espressione: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Assicurati di rimuovere questi tag per evitare errori di sintassi. In questo esempio, l’espressione corretta dopo la rimozione dei tag della funzione **else** è:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Una volta che la condizione è pronta, puoi salvare il contenuto e controllarne il risultato simulando il contenuto.

## Creare contenuti condizionali nelle e-mail {#condition-condition-builder}

Il contenuto condizionale nelle e-mail può essere creato in due modi:
* nell’editor di espressioni, creando una condizione con funzioni Helper;
* in un generatore di contenuti condizionali dedicato, accessibile durante la progettazione di un’e-mail.

La sezione seguente fornisce istruzioni dettagliate su come creare condizioni utilizzando la funzionalità di contenuto condizionale di E-mail Designer. Sono disponibili informazioni dettagliate su come creare condizioni utilizzando l’editor di espressioni [qui](#condition-perso-editor).

In questo esempio, vogliamo creare un messaggio e-mail con più varianti in base alla lingua dei destinatari. Segui questi passaggi:

1. Crea o apri una consegna e-mail, modificane il contenuto e fai clic su **[!UICONTROL Modifica corpo dell’e-mail]** per aprire l’area di lavoro di progettazione e-mail.

1. Seleziona un componente di contenuto e fai clic sull’icona **[!UICONTROL Abilita contenuto condizionale]**.

   ![](assets/condition-email-enable.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Sul lato sinistro della schermata, compare il riquadro **[!UICONTROL Contenuto condizionale]** . In questo riquadro, puoi utilizzare le condizioni per creare più varianti del componente di contenuto selezionato.

1. Configura la prima variante. Passa il cursore sopra **[!UICONTROL Variante - 1]** nel **[!UICONTROL Contenuto condizionale]** e fare clic sul pulsante **[!UICONTROL Aggiungi condizione]** pulsante.

   ![](assets/condition-add-condition.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Viene aperto Query Modeler. Ti consente di creare una condizione filtrando i dati del profilo del destinatario. [Scopri come utilizzare Query Modeler](../query/query-modeler-overview.md).

   Quando la condizione per la prima variante del messaggio è pronta, fai clic su **[!UICONTROL Conferma]**. In questo esempio, stiamo creando una regola destinata ai destinatari la cui lingua è “francese”.

   ![](assets/condition-example.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. La regola ora è associata alla variante. Per una migliore leggibilità, si consiglia di rinominare la variante facendo clic sul menu con i puntini di sospensione.

1. Configura il modo in cui il componente verrà visualizzato se la regola viene soddisfatta al momento dell’invio del messaggio. In questo esempio, se la lingua preferita del destinatario è il francese, il testo dovrà essere in francese.

   ![](assets/condition-email-variant1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Aggiungi tutte le varianti necessarie per il componente contenuto. In qualsiasi momento puoi passare da una variante all’altra per verificare come verrà visualizzato il componente contenuto in base alle relative regole condizionali.

   >[!NOTE]
   >Se nessuna delle regole definite nelle varianti è soddisfatta durante l’invio del messaggio, il componente contenuto visualizzerà il contenuto definito nella **[!UICONTROL Variante predefinita]**, nel riquadro **[!UICONTROL Contenuto condizionale]**.
